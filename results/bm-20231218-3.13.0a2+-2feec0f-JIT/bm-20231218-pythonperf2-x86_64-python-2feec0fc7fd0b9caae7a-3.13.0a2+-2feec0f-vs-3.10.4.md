
# Results vs. 3.10.4

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 292 ms: 1.20x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.48 ms: 1.26x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.84 sec: 1.20x faster                                                       |
| tornado_http   | 157 ms                                                       | 119 ms: 1.32x faster                                                         |
| Geometric mean | (ref)                                                        | 1.25x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 430 ms: 1.61x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 543 ms: 1.51x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 696 ms: 1.34x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.49x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 86.7 ms: 1.55x faster                                                        |
| float          | 111 ms                                                       | 78.0 ms: 1.43x faster                                                        |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.31x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 141 ms: 1.35x faster                                                         |
| regex_dna      | 261 ms                                                       | 247 ms: 1.06x faster                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.53 ms: 1.14x slower                                                        |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                 |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 305 us: 1.49x faster                                                         |
| unpickle_pure_python | 312 us                                                       | 212 us: 1.47x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.35 sec: 1.24x faster                                                       |
| json_loads           | 30.3 us                                                      | 24.6 us: 1.23x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 85.1 ms: 1.08x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 149 ms: 1.07x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.04x faster                                                         |
| pickle               | 9.89 us                                                      | 10.1 us: 1.03x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.6 us: 1.08x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 33.0 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.3 ms: 1.42x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 116 us: 4.62x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.55 ms: 2.11x faster                                                        |
| asyncio_tcp              | 779 ms                                                       | 369 ms: 2.11x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 264 ms: 1.85x faster                                                         |
| chaos                    | 109 ms                                                       | 61.0 ms: 1.78x faster                                                        |
| generators               | 57.3 ms                                                      | 33.6 ms: 1.70x faster                                                        |
| logging_silent           | 167 ns                                                       | 98.4 ns: 1.70x faster                                                        |
| scimark_lu               | 167 ms                                                       | 98.6 ms: 1.69x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 71.1 ms: 1.68x faster                                                        |
| comprehensions           | 26.7 us                                                      | 16.4 us: 1.63x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.38 ms: 1.62x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 66.4 ms: 1.62x faster                                                        |
| async_tree_none          | 692 ms                                                       | 430 ms: 1.61x faster                                                         |
| nbody                    | 134 ms                                                       | 86.7 ms: 1.55x faster                                                        |
| go                       | 262 ms                                                       | 169 ms: 1.55x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 543 ms: 1.51x faster                                                         |
| sqlglot_transpile        | 2.68 ms                                                      | 1.78 ms: 1.51x faster                                                        |
| spectral_norm            | 139 ms                                                       | 92.6 ms: 1.50x faster                                                        |
| richards_super           | 90.6 ms                                                      | 60.6 ms: 1.50x faster                                                        |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| pickle_pure_python       | 455 us                                                       | 305 us: 1.49x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 6.37 ms: 1.48x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 212 us: 1.47x faster                                                         |
| pyflate                  | 733 ms                                                       | 505 ms: 1.45x faster                                                         |
| float                    | 111 ms                                                       | 78.0 ms: 1.43x faster                                                        |
| mako                     | 14.7 ms                                                      | 10.3 ms: 1.42x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.58 ms: 1.39x faster                                                        |
| richards                 | 75.1 ms                                                      | 54.4 ms: 1.38x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| logging_simple           | 8.88 us                                                      | 6.53 us: 1.36x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                        |
| regex_compile            | 190 ms                                                       | 141 ms: 1.35x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.16 us: 1.35x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 696 ms: 1.34x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.5 us: 1.33x faster                                                        |
| tornado_http             | 157 ms                                                       | 119 ms: 1.32x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.66 sec: 1.30x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 812 ms: 1.29x faster                                                         |
| nqueens                  | 115 ms                                                       | 88.9 ms: 1.29x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 46.4 ns: 1.29x faster                                                        |
| deepcopy                 | 468 us                                                       | 364 us: 1.29x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.32 sec: 1.27x faster                                                       |
| sympy_sum                | 193 ms                                                       | 152 ms: 1.27x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.48 ms: 1.26x faster                                                        |
| scimark_sor              | 180 ms                                                       | 143 ms: 1.26x faster                                                         |
| fannkuch                 | 483 ms                                                       | 387 ms: 1.25x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.35 sec: 1.24x faster                                                       |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                                         |
| sympy_str                | 360 ms                                                       | 292 ms: 1.23x faster                                                         |
| json_loads               | 30.3 us                                                      | 24.6 us: 1.23x faster                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.13 ms: 1.23x faster                                                        |
| sympy_integrate          | 28.2 ms                                                      | 23.1 ms: 1.22x faster                                                        |
| scimark_fft              | 361 ms                                                       | 297 ms: 1.22x faster                                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.30 us: 1.21x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.49 sec: 1.21x faster                                                       |
| sympy_expand             | 600 ms                                                       | 498 ms: 1.21x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.84 sec: 1.20x faster                                                       |
| 2to3                     | 350 ms                                                       | 292 ms: 1.20x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 67.6 ms: 1.20x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 954 us: 1.20x faster                                                         |
| dask                     | 472 ms                                                       | 395 ms: 1.20x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 59.2 ms: 1.19x faster                                                        |
| async_generators         | 421 ms                                                       | 366 ms: 1.15x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 18.8 ms: 1.13x faster                                                        |
| json                     | 5.86 ms                                                      | 5.26 ms: 1.12x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.71 us: 1.10x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.61 ms: 1.09x faster                                                        |
| mypy2                    | 933 ms                                                       | 858 ms: 1.09x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 85.1 ms: 1.08x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 149 ms: 1.07x faster                                                         |
| meteor_contest           | 138 ms                                                       | 129 ms: 1.07x faster                                                         |
| regex_dna                | 261 ms                                                       | 247 ms: 1.06x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 106 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                         |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.03x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.56 ms: 1.04x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.6 us: 1.08x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.5 ms: 1.09x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.04 ms: 1.11x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 33.0 us: 1.12x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.53 ms: 1.14x slower                                                        |
| coverage                 | 63.3 ms                                                      | 80.8 ms: 1.28x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.29x faster                                                                 |

Benchmark hidden because not significant (3): regex_v8, asyncio_websockets, unpickle_list
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-2feec0f-JIT/bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.06x