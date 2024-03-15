
# Results vs. 3.10.4

- fork: python
- ref: 35ef8cb25917bfd6cbbd
- machine: linux-x86_64
- commit hash: 35ef8cb
- commit date: 2024-01-04
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 311 ms: 1.13x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.82 ms: 1.21x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                       |
| tornado_http   | 157 ms                                                       | 122 ms: 1.28x faster                                                         |
| Geometric mean | (ref)                                                        | 1.19x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 449 ms: 1.54x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 563 ms: 1.46x faster                                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 716 ms: 1.31x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.44x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 102 ms: 1.09x faster                                                         |
| nbody          | 134 ms                                                       | 126 ms: 1.06x faster                                                         |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 261 ms                                                       | 236 ms: 1.10x faster                                                         |
| regex_compile  | 190 ms                                                       | 173 ms: 1.10x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 24.9 ms: 1.09x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.44 ms: 1.11x slower                                                        |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 309 us: 1.47x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.9 ms: 1.34x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 241 us: 1.29x faster                                                         |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.21x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 63.0 ms: 1.20x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.81 sec: 1.04x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.57 us: 1.02x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 92.8 ms: 1.01x slower                                                        |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 30.5 us: 1.03x slower                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 116 ms: 1.05x slower                                                         |
| pickle_list          | 4.12 us                                                      | 4.35 us: 1.06x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.7 us: 1.09x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.09x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 127 us: 4.24x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 372 ms: 2.10x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                       |
| generators               | 57.3 ms                                                      | 33.8 ms: 1.70x faster                                                        |
| logging_silent           | 167 ns                                                       | 99.7 ns: 1.68x faster                                                        |
| raytrace                 | 489 ms                                                       | 300 ms: 1.63x faster                                                         |
| scimark_lu               | 167 ms                                                       | 106 ms: 1.58x faster                                                         |
| async_tree_none          | 692 ms                                                       | 449 ms: 1.54x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.46 ms: 1.53x faster                                                        |
| richards_super           | 90.6 ms                                                      | 59.6 ms: 1.52x faster                                                        |
| pickle_pure_python       | 455 us                                                       | 309 us: 1.47x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                       |
| async_tree_memoization   | 819 ms                                                       | 563 ms: 1.46x faster                                                         |
| go                       | 262 ms                                                       | 180 ms: 1.45x faster                                                         |
| sqlglot_transpile        | 2.68 ms                                                      | 1.87 ms: 1.43x faster                                                        |
| richards                 | 75.1 ms                                                      | 52.8 ms: 1.42x faster                                                        |
| chaos                    | 109 ms                                                       | 77.2 ms: 1.41x faster                                                        |
| deltablue                | 7.50 ms                                                      | 5.37 ms: 1.40x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 86.1 ms: 1.38x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.0 ms: 1.38x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.75 ms: 1.34x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.9 ms: 1.34x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 716 ms: 1.31x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.80 us: 1.30x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 241 us: 1.29x faster                                                         |
| unpack_sequence          | 59.9 ns                                                      | 46.6 ns: 1.29x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.49 us: 1.29x faster                                                        |
| tornado_http             | 157 ms                                                       | 122 ms: 1.28x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.32 sec: 1.27x faster                                                       |
| deepcopy_memo            | 49.8 us                                                      | 39.8 us: 1.25x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 86.7 ms: 1.24x faster                                                        |
| deepcopy                 | 468 us                                                       | 381 us: 1.23x faster                                                         |
| pyflate                  | 733 ms                                                       | 597 ms: 1.23x faster                                                         |
| scimark_sor              | 180 ms                                                       | 148 ms: 1.22x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.82 ms: 1.21x faster                                                        |
| json_loads               | 30.3 us                                                      | 25.2 us: 1.21x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 63.0 ms: 1.20x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.36 us: 1.19x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 974 us: 1.17x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                       |
| sqlglot_normalize        | 144 ms                                                       | 124 ms: 1.16x faster                                                         |
| dask                     | 472 ms                                                       | 409 ms: 1.15x faster                                                         |
| sympy_sum                | 193 ms                                                       | 169 ms: 1.14x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.64 sec: 1.14x faster                                                       |
| async_generators         | 421 ms                                                       | 370 ms: 1.14x faster                                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 929 ms: 1.13x faster                                                         |
| 2to3                     | 350 ms                                                       | 311 ms: 1.13x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.92 sec: 1.12x faster                                                       |
| json                     | 5.86 ms                                                      | 5.24 ms: 1.12x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 72.4 ms: 1.12x faster                                                        |
| sympy_integrate          | 28.2 ms                                                      | 25.3 ms: 1.11x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                                        |
| sympy_expand             | 600 ms                                                       | 543 ms: 1.11x faster                                                         |
| regex_dna                | 261 ms                                                       | 236 ms: 1.10x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 63.6 ms: 1.10x faster                                                        |
| sympy_str                | 360 ms                                                       | 327 ms: 1.10x faster                                                         |
| regex_compile            | 190 ms                                                       | 173 ms: 1.10x faster                                                         |
| float                    | 111 ms                                                       | 102 ms: 1.09x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 24.9 ms: 1.09x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.63 ms: 1.08x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| sqlite_synth             | 2.99 us                                                      | 2.79 us: 1.07x faster                                                        |
| comprehensions           | 26.7 us                                                      | 25.0 us: 1.07x faster                                                        |
| nbody                    | 134 ms                                                       | 126 ms: 1.06x faster                                                         |
| nqueens                  | 115 ms                                                       | 110 ms: 1.05x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.81 sec: 1.04x faster                                                       |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| unpickle_list            | 4.65 us                                                      | 4.57 us: 1.02x faster                                                        |
| asyncio_websockets       | 390 ms                                                       | 384 ms: 1.02x faster                                                         |
| fannkuch                 | 483 ms                                                       | 475 ms: 1.02x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 92.8 ms: 1.01x slower                                                        |
| meteor_contest           | 138 ms                                                       | 140 ms: 1.01x slower                                                         |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 30.5 us: 1.03x slower                                                        |
| hexiom                   | 9.42 ms                                                      | 9.85 ms: 1.05x slower                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 116 ms: 1.05x slower                                                         |
| pickle_list              | 4.12 us                                                      | 4.35 us: 1.06x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.7 us: 1.09x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.79 ms: 1.11x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.44 ms: 1.11x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.49 ms: 1.17x slower                                                        |
| scimark_fft              | 361 ms                                                       | 429 ms: 1.19x slower                                                         |
| spectral_norm            | 139 ms                                                       | 172 ms: 1.23x slower                                                         |
| coverage                 | 63.3 ms                                                      | 79.9 ms: 1.26x slower                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.52 ms: 1.28x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.18x faster                                                                 |

Benchmark hidden because not significant (2): mypy2, mako
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-35ef8cb-PYTHON_UOPS/bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 1.07x