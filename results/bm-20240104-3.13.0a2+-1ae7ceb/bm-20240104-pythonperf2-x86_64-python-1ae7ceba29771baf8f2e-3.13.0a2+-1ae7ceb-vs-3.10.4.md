
# Results vs. 3.10.4

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 292 ms: 1.20x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.53 ms: 1.25x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                                       |
| tornado_http   | 157 ms                                                       | 118 ms: 1.33x faster                                                         |
| Geometric mean | (ref)                                                        | 1.25x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 431 ms: 1.60x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 544 ms: 1.51x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.50x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 693 ms: 1.35x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.49x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 84.6 ms: 1.59x faster                                                        |
| float          | 111 ms                                                       | 78.5 ms: 1.42x faster                                                        |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.32x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 142 ms: 1.34x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 25.4 ms: 1.07x faster                                                        |
| regex_dna      | 261 ms                                                       | 247 ms: 1.06x faster                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.58 ms: 1.16x slower                                                        |
| Geometric mean | (ref)                                                        | 1.07x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 210 us: 1.49x faster                                                         |
| pickle_pure_python   | 455 us                                                       | 311 us: 1.46x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.38x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.22 sec: 1.32x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 59.3 ms: 1.28x faster                                                        |
| json_loads           | 30.3 us                                                      | 24.8 us: 1.22x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 87.1 ms: 1.06x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.04x faster                                                         |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 31.4 us: 1.07x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.40 us: 1.07x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.9 us: 1.10x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.3 ms: 1.42x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 116 us: 4.61x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 365 ms: 2.14x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.54 ms: 2.12x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| chaos                    | 109 ms                                                       | 58.8 ms: 1.85x faster                                                        |
| raytrace                 | 489 ms                                                       | 270 ms: 1.81x faster                                                         |
| scimark_lu               | 167 ms                                                       | 95.9 ms: 1.74x faster                                                        |
| logging_silent           | 167 ns                                                       | 97.6 ns: 1.71x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 70.0 ms: 1.70x faster                                                        |
| generators               | 57.3 ms                                                      | 34.2 ms: 1.68x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.39 ms: 1.61x faster                                                        |
| comprehensions           | 26.7 us                                                      | 16.6 us: 1.61x faster                                                        |
| async_tree_none          | 692 ms                                                       | 431 ms: 1.60x faster                                                         |
| nbody                    | 134 ms                                                       | 84.6 ms: 1.59x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 67.8 ms: 1.59x faster                                                        |
| go                       | 262 ms                                                       | 167 ms: 1.56x faster                                                         |
| richards_super           | 90.6 ms                                                      | 58.4 ms: 1.55x faster                                                        |
| spectral_norm            | 139 ms                                                       | 91.4 ms: 1.52x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 544 ms: 1.51x faster                                                         |
| sqlglot_transpile        | 2.68 ms                                                      | 1.79 ms: 1.50x faster                                                        |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.50x faster                                                       |
| hexiom                   | 9.42 ms                                                      | 6.31 ms: 1.49x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 210 us: 1.49x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 311 us: 1.46x faster                                                         |
| pyflate                  | 733 ms                                                       | 503 ms: 1.46x faster                                                         |
| richards                 | 75.1 ms                                                      | 52.3 ms: 1.44x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.46 ms: 1.43x faster                                                        |
| mako                     | 14.7 ms                                                      | 10.3 ms: 1.42x faster                                                        |
| float                    | 111 ms                                                       | 78.5 ms: 1.42x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.38x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                                        |
| logging_simple           | 8.88 us                                                      | 6.54 us: 1.36x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 693 ms: 1.35x faster                                                         |
| regex_compile            | 190 ms                                                       | 142 ms: 1.34x faster                                                         |
| nqueens                  | 115 ms                                                       | 86.6 ms: 1.33x faster                                                        |
| tornado_http             | 157 ms                                                       | 118 ms: 1.33x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.28 us: 1.32x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.27 sec: 1.32x faster                                                       |
| tomli_loads              | 2.92 sec                                                     | 2.22 sec: 1.32x faster                                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.67 sec: 1.29x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 59.3 ms: 1.28x faster                                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 821 ms: 1.28x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 39.0 us: 1.28x faster                                                        |
| sympy_sum                | 193 ms                                                       | 152 ms: 1.27x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.53 ms: 1.25x faster                                                        |
| fannkuch                 | 483 ms                                                       | 386 ms: 1.25x faster                                                         |
| scimark_sor              | 180 ms                                                       | 145 ms: 1.25x faster                                                         |
| deepcopy                 | 468 us                                                       | 377 us: 1.24x faster                                                         |
| sympy_str                | 360 ms                                                       | 290 ms: 1.24x faster                                                         |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                                         |
| json_loads               | 30.3 us                                                      | 24.8 us: 1.22x faster                                                        |
| sympy_integrate          | 28.2 ms                                                      | 23.1 ms: 1.22x faster                                                        |
| docutils                 | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                                       |
| scimark_fft              | 361 ms                                                       | 299 ms: 1.21x faster                                                         |
| sympy_expand             | 600 ms                                                       | 498 ms: 1.20x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.22 ms: 1.20x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 951 us: 1.20x faster                                                         |
| 2to3                     | 350 ms                                                       | 292 ms: 1.20x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.51 sec: 1.20x faster                                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 59.0 ms: 1.19x faster                                                        |
| dask                     | 472 ms                                                       | 398 ms: 1.19x faster                                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.38 us: 1.19x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 68.5 ms: 1.18x faster                                                        |
| async_generators         | 421 ms                                                       | 360 ms: 1.17x faster                                                         |
| unpack_sequence          | 59.9 ns                                                      | 53.2 ns: 1.13x faster                                                        |
| json                     | 5.86 ms                                                      | 5.25 ms: 1.12x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.70 us: 1.11x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                                        |
| mypy2                    | 933 ms                                                       | 859 ms: 1.09x faster                                                         |
| meteor_contest           | 138 ms                                                       | 128 ms: 1.08x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 25.4 ms: 1.07x faster                                                        |
| xml_etree_generate       | 92.3 ms                                                      | 87.1 ms: 1.06x faster                                                        |
| regex_dna                | 261 ms                                                       | 247 ms: 1.06x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                         |
| pickle                   | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.58 ms: 1.05x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 31.4 us: 1.07x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.40 us: 1.07x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.9 us: 1.10x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.58 ms: 1.16x slower                                                        |
| coverage                 | 63.3 ms                                                      | 78.4 ms: 1.24x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.29x faster                                                                 |

Benchmark hidden because not significant (2): asyncio_websockets, unpickle_list
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.06x