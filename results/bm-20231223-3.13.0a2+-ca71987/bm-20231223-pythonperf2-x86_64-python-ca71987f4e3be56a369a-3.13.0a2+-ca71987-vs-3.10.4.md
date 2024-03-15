
# Results vs. 3.10.4

- fork: python
- ref: ca71987f4e3be56a369a
- machine: linux-x86_64
- commit hash: ca71987
- commit date: 2023-12-23
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 294 ms: 1.19x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.37 ms: 1.28x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.81 sec: 1.21x faster                                                       |
| tornado_http   | 157 ms                                                       | 118 ms: 1.33x faster                                                         |
| Geometric mean | (ref)                                                        | 1.25x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 544 ms: 1.51x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.50x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 692 ms: 1.35x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.49x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 87.7 ms: 1.53x faster                                                        |
| float          | 111 ms                                                       | 79.4 ms: 1.40x faster                                                        |
| pidigits       | 271 ms                                                       | 264 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.30x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 142 ms: 1.34x faster                                                         |
| regex_dna      | 261 ms                                                       | 245 ms: 1.07x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.44 ms: 1.12x slower                                                        |
| Geometric mean | (ref)                                                        | 1.07x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 210 us: 1.48x faster                                                         |
| pickle_pure_python   | 455 us                                                       | 310 us: 1.47x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.21 sec: 1.32x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 59.4 ms: 1.28x faster                                                        |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.21x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 149 ms: 1.07x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 86.3 ms: 1.07x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.04x faster                                                         |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 30.4 us: 1.03x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.4 us: 1.07x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.4 ms: 1.41x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 120 us: 4.48x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 366 ms: 2.13x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.53 ms: 2.13x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 257 ms: 1.90x faster                                                         |
| chaos                    | 109 ms                                                       | 58.8 ms: 1.85x faster                                                        |
| logging_silent           | 167 ns                                                       | 96.3 ns: 1.74x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 69.6 ms: 1.71x faster                                                        |
| scimark_lu               | 167 ms                                                       | 99.0 ms: 1.69x faster                                                        |
| generators               | 57.3 ms                                                      | 34.0 ms: 1.69x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 65.3 ms: 1.64x faster                                                        |
| comprehensions           | 26.7 us                                                      | 16.4 us: 1.63x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.37 ms: 1.63x faster                                                        |
| async_tree_none          | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| go                       | 262 ms                                                       | 167 ms: 1.56x faster                                                         |
| richards_super           | 90.6 ms                                                      | 59.0 ms: 1.54x faster                                                        |
| spectral_norm            | 139 ms                                                       | 90.9 ms: 1.53x faster                                                        |
| nbody                    | 134 ms                                                       | 87.7 ms: 1.53x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.78 ms: 1.51x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 544 ms: 1.51x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.50x faster                                                       |
| hexiom                   | 9.42 ms                                                      | 6.33 ms: 1.49x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 210 us: 1.48x faster                                                         |
| pyflate                  | 733 ms                                                       | 500 ms: 1.47x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 310 us: 1.47x faster                                                         |
| mako                     | 14.7 ms                                                      | 10.4 ms: 1.41x faster                                                        |
| richards                 | 75.1 ms                                                      | 53.3 ms: 1.41x faster                                                        |
| float                    | 111 ms                                                       | 79.4 ms: 1.40x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.60 ms: 1.39x faster                                                        |
| logging_simple           | 8.88 us                                                      | 6.45 us: 1.38x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.1 ms: 1.37x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.06 us: 1.37x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 692 ms: 1.35x faster                                                         |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 44.8 ns: 1.34x faster                                                        |
| regex_compile            | 190 ms                                                       | 142 ms: 1.34x faster                                                         |
| tornado_http             | 157 ms                                                       | 118 ms: 1.33x faster                                                         |
| nqueens                  | 115 ms                                                       | 87.0 ms: 1.32x faster                                                        |
| tomli_loads              | 2.92 sec                                                     | 2.21 sec: 1.32x faster                                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.64 sec: 1.31x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 808 ms: 1.30x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 38.7 us: 1.29x faster                                                        |
| chameleon                | 9.44 ms                                                      | 7.37 ms: 1.28x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 59.4 ms: 1.28x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                                       |
| sympy_sum                | 193 ms                                                       | 152 ms: 1.26x faster                                                         |
| scimark_sor              | 180 ms                                                       | 143 ms: 1.26x faster                                                         |
| deepcopy                 | 468 us                                                       | 374 us: 1.25x faster                                                         |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                                         |
| sympy_str                | 360 ms                                                       | 292 ms: 1.23x faster                                                         |
| fannkuch                 | 483 ms                                                       | 392 ms: 1.23x faster                                                         |
| scimark_fft              | 361 ms                                                       | 296 ms: 1.22x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 23.1 ms: 1.22x faster                                                        |
| docutils                 | 3.41 sec                                                     | 2.81 sec: 1.21x faster                                                       |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.20 ms: 1.21x faster                                                        |
| json_loads               | 30.3 us                                                      | 25.2 us: 1.21x faster                                                        |
| sympy_expand             | 600 ms                                                       | 498 ms: 1.20x faster                                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.33 us: 1.20x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.50 sec: 1.20x faster                                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 58.5 ms: 1.20x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 67.7 ms: 1.20x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 957 us: 1.19x faster                                                         |
| dask                     | 472 ms                                                       | 396 ms: 1.19x faster                                                         |
| 2to3                     | 350 ms                                                       | 294 ms: 1.19x faster                                                         |
| async_generators         | 421 ms                                                       | 357 ms: 1.18x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 18.8 ms: 1.14x faster                                                        |
| json                     | 5.86 ms                                                      | 5.26 ms: 1.11x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.70 us: 1.11x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.60 ms: 1.10x faster                                                        |
| mypy2                    | 933 ms                                                       | 857 ms: 1.09x faster                                                         |
| meteor_contest           | 138 ms                                                       | 128 ms: 1.08x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 149 ms: 1.07x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 86.3 ms: 1.07x faster                                                        |
| regex_dna                | 261 ms                                                       | 245 ms: 1.07x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 264 ms: 1.03x faster                                                         |
| pickle                   | 9.89 us                                                      | 10.0 us: 1.01x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 30.4 us: 1.03x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.4 us: 1.07x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.74 ms: 1.10x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.44 ms: 1.12x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.16 ms: 1.13x slower                                                        |
| coverage                 | 63.3 ms                                                      | 78.4 ms: 1.24x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.29x faster                                                                 |

Benchmark hidden because not significant (2): asyncio_websockets, unpickle_list
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231223-3.13.0a2+-ca71987/bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.06x