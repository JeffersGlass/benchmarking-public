
# Results vs. 3.10.4

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 310 ms: 1.13x faster                                                         |
| chameleon      | 9.44 ms                                                      | 8.13 ms: 1.16x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.95 sec: 1.16x faster                                                       |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                                         |
| Geometric mean | (ref)                                                        | 1.18x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 450 ms: 1.54x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 561 ms: 1.46x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 714 ms: 1.31x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.44x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 105 ms: 1.06x faster                                                         |
| nbody          | 134 ms                                                       | 128 ms: 1.04x faster                                                         |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 172 ms: 1.11x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 25.5 ms: 1.06x faster                                                        |
| regex_dna      | 261 ms                                                       | 246 ms: 1.06x faster                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.80 ms: 1.23x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 309 us: 1.47x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 229 us: 1.36x faster                                                         |
| json_loads           | 30.3 us                                                      | 24.5 us: 1.24x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 62.3 ms: 1.22x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 150 ms: 1.07x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.80 sec: 1.04x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 91.8 ms: 1.00x faster                                                        |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 118 ms: 1.06x slower                                                         |
| pickle_dict          | 29.5 us                                                      | 31.6 us: 1.07x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.44 us: 1.08x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.9 us: 1.10x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.09x faster                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 14.9 ms: 1.01x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 127 us: 4.23x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 374 ms: 2.08x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                       |
| logging_silent           | 167 ns                                                       | 98.1 ns: 1.71x faster                                                        |
| generators               | 57.3 ms                                                      | 34.4 ms: 1.67x faster                                                        |
| raytrace                 | 489 ms                                                       | 299 ms: 1.64x faster                                                         |
| scimark_lu               | 167 ms                                                       | 107 ms: 1.55x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.44 ms: 1.55x faster                                                        |
| async_tree_none          | 692 ms                                                       | 450 ms: 1.54x faster                                                         |
| richards_super           | 90.6 ms                                                      | 60.3 ms: 1.50x faster                                                        |
| pickle_pure_python       | 455 us                                                       | 309 us: 1.47x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 561 ms: 1.46x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                       |
| sqlglot_transpile        | 2.68 ms                                                      | 1.86 ms: 1.44x faster                                                        |
| go                       | 262 ms                                                       | 183 ms: 1.43x faster                                                         |
| chaos                    | 109 ms                                                       | 76.2 ms: 1.42x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 85.1 ms: 1.40x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 43.5 ns: 1.38x faster                                                        |
| richards                 | 75.1 ms                                                      | 54.8 ms: 1.37x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| deltablue                | 7.50 ms                                                      | 5.49 ms: 1.37x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.68 ms: 1.36x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 229 us: 1.36x faster                                                         |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 714 ms: 1.31x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.83 us: 1.30x faster                                                        |
| pyflate                  | 733 ms                                                       | 572 ms: 1.28x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.52 us: 1.28x faster                                                        |
| scimark_sor              | 180 ms                                                       | 142 ms: 1.27x faster                                                         |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 39.6 us: 1.26x faster                                                        |
| deepcopy                 | 468 us                                                       | 377 us: 1.24x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 86.8 ms: 1.24x faster                                                        |
| json_loads               | 30.3 us                                                      | 24.5 us: 1.24x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.36 sec: 1.23x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 62.3 ms: 1.22x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 964 us: 1.18x faster                                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.40 us: 1.18x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 123 ms: 1.16x faster                                                         |
| chameleon                | 9.44 ms                                                      | 8.13 ms: 1.16x faster                                                        |
| docutils                 | 3.41 sec                                                     | 2.95 sec: 1.16x faster                                                       |
| dask                     | 472 ms                                                       | 409 ms: 1.15x faster                                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 911 ms: 1.15x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.88 sec: 1.14x faster                                                       |
| sympy_sum                | 193 ms                                                       | 169 ms: 1.14x faster                                                         |
| json                     | 5.86 ms                                                      | 5.19 ms: 1.13x faster                                                        |
| 2to3                     | 350 ms                                                       | 310 ms: 1.13x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.67 sec: 1.13x faster                                                       |
| dulwich_log              | 81.1 ms                                                      | 72.5 ms: 1.12x faster                                                        |
| sympy_integrate          | 28.2 ms                                                      | 25.2 ms: 1.12x faster                                                        |
| sympy_expand             | 600 ms                                                       | 540 ms: 1.11x faster                                                         |
| sympy_str                | 360 ms                                                       | 325 ms: 1.11x faster                                                         |
| async_generators         | 421 ms                                                       | 380 ms: 1.11x faster                                                         |
| regex_compile            | 190 ms                                                       | 172 ms: 1.11x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 63.6 ms: 1.10x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.61 ms: 1.10x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 19.5 ms: 1.09x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.76 us: 1.08x faster                                                        |
| comprehensions           | 26.7 us                                                      | 24.9 us: 1.07x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 150 ms: 1.07x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 25.5 ms: 1.06x faster                                                        |
| regex_dna                | 261 ms                                                       | 246 ms: 1.06x faster                                                         |
| float                    | 111 ms                                                       | 105 ms: 1.06x faster                                                         |
| nqueens                  | 115 ms                                                       | 110 ms: 1.04x faster                                                         |
| nbody                    | 134 ms                                                       | 128 ms: 1.04x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.80 sec: 1.04x faster                                                       |
| fannkuch                 | 483 ms                                                       | 468 ms: 1.03x faster                                                         |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| asyncio_websockets       | 390 ms                                                       | 387 ms: 1.01x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 91.8 ms: 1.00x faster                                                        |
| meteor_contest           | 138 ms                                                       | 139 ms: 1.01x slower                                                         |
| mako                     | 14.7 ms                                                      | 14.9 ms: 1.01x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| hexiom                   | 9.42 ms                                                      | 9.75 ms: 1.04x slower                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 118 ms: 1.06x slower                                                         |
| pickle_dict              | 29.5 us                                                      | 31.6 us: 1.07x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.44 us: 1.08x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.69 ms: 1.08x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.9 us: 1.10x slower                                                        |
| spectral_norm            | 139 ms                                                       | 161 ms: 1.16x slower                                                         |
| telco                    | 7.23 ms                                                      | 8.48 ms: 1.17x slower                                                        |
| scimark_fft              | 361 ms                                                       | 429 ms: 1.19x slower                                                         |
| regex_effbot             | 3.09 ms                                                      | 3.80 ms: 1.23x slower                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.68 ms: 1.31x slower                                                        |
| coverage                 | 63.3 ms                                                      | 84.5 ms: 1.34x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.18x faster                                                                 |

Benchmark hidden because not significant (2): mypy2, unpickle_list
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-2feec0f-PYTHON_UOPS/bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 1.07x