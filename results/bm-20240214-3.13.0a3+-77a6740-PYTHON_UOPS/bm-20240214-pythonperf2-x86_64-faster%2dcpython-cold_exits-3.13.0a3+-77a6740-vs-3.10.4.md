
# Results vs. 3.10.4

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 77a6740
- commit date: 2024-02-14
- overall geometric mean: 1.15x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 319 ms: 1.10x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.97 ms: 1.19x faster                                                        |
| docutils       | 3.41 sec                                                     | 3.06 sec: 1.11x faster                                                       |
| tornado_http   | 157 ms                                                       | 126 ms: 1.24x faster                                                         |
| Geometric mean | (ref)                                                        | 1.16x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 450 ms: 1.54x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 563 ms: 1.45x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.45x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 717 ms: 1.31x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.43x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 123 ms: 1.09x faster                                                         |
| float          | 111 ms                                                       | 102 ms: 1.09x faster                                                         |
| pidigits       | 271 ms                                                       | 266 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.07x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 261 ms                                                       | 235 ms: 1.11x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 26.4 ms: 1.03x faster                                                        |
| regex_compile  | 190 ms                                                       | 192 ms: 1.01x slower                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.58 ms: 1.16x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 314 us: 1.45x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.34x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 62.5 ms: 1.21x faster                                                        |
| json_loads           | 30.3 us                                                      | 25.1 us: 1.21x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.87 sec: 1.02x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 91.2 ms: 1.01x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 310 us: 1.01x faster                                                         |
| unpickle_list        | 4.65 us                                                      | 4.74 us: 1.02x slower                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 116 ms: 1.05x slower                                                         |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 33.6 us: 1.14x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.05x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 14.1 ms: 1.04x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 124 us: 4.32x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 374 ms: 2.08x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                       |
| deltablue                | 7.50 ms                                                      | 4.05 ms: 1.85x faster                                                        |
| generators               | 57.3 ms                                                      | 34.0 ms: 1.68x faster                                                        |
| logging_silent           | 167 ns                                                       | 99.8 ns: 1.68x faster                                                        |
| async_tree_none          | 692 ms                                                       | 450 ms: 1.54x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.53 ms: 1.46x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 563 ms: 1.45x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.45x faster                                                       |
| pickle_pure_python       | 455 us                                                       | 314 us: 1.45x faster                                                         |
| raytrace                 | 489 ms                                                       | 339 ms: 1.44x faster                                                         |
| chaos                    | 109 ms                                                       | 75.5 ms: 1.44x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 86.8 ms: 1.37x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.96 ms: 1.37x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.67 ms: 1.36x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.34x faster                                                        |
| go                       | 262 ms                                                       | 197 ms: 1.33x faster                                                         |
| richards_super           | 90.6 ms                                                      | 68.5 ms: 1.32x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 717 ms: 1.31x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.91 us: 1.28x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.56 us: 1.28x faster                                                        |
| tornado_http             | 157 ms                                                       | 126 ms: 1.24x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 62.5 ms: 1.21x faster                                                        |
| richards                 | 75.1 ms                                                      | 62.0 ms: 1.21x faster                                                        |
| json_loads               | 30.3 us                                                      | 25.1 us: 1.21x faster                                                        |
| deepcopy                 | 468 us                                                       | 387 us: 1.21x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 41.7 us: 1.19x faster                                                        |
| scimark_lu               | 167 ms                                                       | 140 ms: 1.19x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.97 ms: 1.19x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 123 ms: 1.17x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.43 sec: 1.17x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.48 us: 1.15x faster                                                        |
| dask                     | 472 ms                                                       | 411 ms: 1.15x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 996 us: 1.15x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.64 sec: 1.14x faster                                                       |
| sympy_sum                | 193 ms                                                       | 172 ms: 1.12x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 25.3 ms: 1.12x faster                                                        |
| docutils                 | 3.41 sec                                                     | 3.06 sec: 1.11x faster                                                       |
| regex_dna                | 261 ms                                                       | 235 ms: 1.11x faster                                                         |
| scimark_sor              | 180 ms                                                       | 163 ms: 1.11x faster                                                         |
| async_generators         | 421 ms                                                       | 381 ms: 1.10x faster                                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 952 ms: 1.10x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 19.4 ms: 1.10x faster                                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.96 sec: 1.10x faster                                                       |
| json                     | 5.86 ms                                                      | 5.34 ms: 1.10x faster                                                        |
| 2to3                     | 350 ms                                                       | 319 ms: 1.10x faster                                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.61 ms: 1.10x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| nbody                    | 134 ms                                                       | 123 ms: 1.09x faster                                                         |
| sympy_str                | 360 ms                                                       | 330 ms: 1.09x faster                                                         |
| comprehensions           | 26.7 us                                                      | 24.5 us: 1.09x faster                                                        |
| float                    | 111 ms                                                       | 102 ms: 1.09x faster                                                         |
| pyflate                  | 733 ms                                                       | 676 ms: 1.08x faster                                                         |
| sympy_expand             | 600 ms                                                       | 559 ms: 1.07x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 76.0 ms: 1.07x faster                                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 66.0 ms: 1.06x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.85 us: 1.05x faster                                                        |
| mako                     | 14.7 ms                                                      | 14.1 ms: 1.04x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 104 ms: 1.03x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 26.4 ms: 1.03x faster                                                        |
| pidigits                 | 271 ms                                                       | 266 ms: 1.02x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.87 sec: 1.02x faster                                                       |
| xml_etree_generate       | 92.3 ms                                                      | 91.2 ms: 1.01x faster                                                        |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| nqueens                  | 115 ms                                                       | 114 ms: 1.01x faster                                                         |
| unpickle_pure_python     | 312 us                                                       | 310 us: 1.01x faster                                                         |
| meteor_contest           | 138 ms                                                       | 139 ms: 1.01x slower                                                         |
| regex_compile            | 190 ms                                                       | 192 ms: 1.01x slower                                                         |
| unpickle_list            | 4.65 us                                                      | 4.74 us: 1.02x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.57 ms: 1.04x slower                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 116 ms: 1.05x slower                                                         |
| fannkuch                 | 483 ms                                                       | 512 ms: 1.06x slower                                                         |
| pickle                   | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| spectral_norm            | 139 ms                                                       | 149 ms: 1.07x slower                                                         |
| pickle_list              | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                        |
| hexiom                   | 9.42 ms                                                      | 10.5 ms: 1.11x slower                                                        |
| unpack_sequence          | 59.9 ns                                                      | 66.9 ns: 1.12x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 33.6 us: 1.14x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.38 ms: 1.16x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.58 ms: 1.16x slower                                                        |
| scimark_fft              | 361 ms                                                       | 420 ms: 1.16x slower                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.22 ms: 1.22x slower                                                        |
| coverage                 | 63.3 ms                                                      | 80.0 ms: 1.26x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.15x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-77a6740-PYTHON_UOPS/bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: 1.08x