
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0rc2
- machine: linux-x86_64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 287 ms: 1.22x faster                                               |
| docutils       | 3.41 sec                                                     | 2.90 sec: 1.18x faster                                             |
| tornado_http   | 157 ms                                                       | 120 ms: 1.31x faster                                               |
| Geometric mean | (ref)                                                        | 1.24x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                             |
| async_tree_none         | 692 ms                                                       | 458 ms: 1.51x faster                                               |
| async_tree_memoization  | 819 ms                                                       | 552 ms: 1.48x faster                                               |
| async_tree_cpu_io_mixed | 936 ms                                                       | 702 ms: 1.33x faster                                               |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 87.5 ms: 1.53x faster                                              |
| float          | 111 ms                                                       | 79.6 ms: 1.40x faster                                              |
| pidigits       | 271 ms                                                       | 264 ms: 1.03x faster                                               |
| Geometric mean | (ref)                                                        | 1.30x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.30x faster                                               |
| regex_v8       | 27.2 ms                                                      | 23.8 ms: 1.14x faster                                              |
| regex_dna      | 261 ms                                                       | 238 ms: 1.10x faster                                               |
| regex_effbot   | 3.09 ms                                                      | 3.52 ms: 1.14x slower                                              |
| Geometric mean | (ref)                                                        | 1.09x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 212 us: 1.47x faster                                               |
| json_dumps           | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                              |
| pickle_pure_python   | 455 us                                                       | 326 us: 1.40x faster                                               |
| tomli_loads          | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                             |
| xml_etree_process    | 75.9 ms                                                      | 58.9 ms: 1.29x faster                                              |
| json_loads           | 30.3 us                                                      | 24.4 us: 1.24x faster                                              |
| xml_etree_parse      | 160 ms                                                       | 146 ms: 1.10x faster                                               |
| xml_etree_generate   | 92.3 ms                                                      | 85.8 ms: 1.08x faster                                              |
| xml_etree_iterparse  | 110 ms                                                       | 103 ms: 1.07x faster                                               |
| unpickle_list        | 4.65 us                                                      | 4.75 us: 1.02x slower                                              |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                              |
| pickle_list          | 4.12 us                                                      | 4.46 us: 1.08x slower                                              |
| unpickle             | 13.5 us                                                      | 14.7 us: 1.09x slower                                              |
| pickle_dict          | 29.5 us                                                      | 32.4 us: 1.10x slower                                              |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.7 ms: 1.02x slower                                              |
| python_startup_no_site | 7.33 ms                                                      | 8.67 ms: 1.18x slower                                              |
| Geometric mean         | (ref)                                                        | 1.10x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 9.92 ms: 1.48x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 149 us: 3.60x faster                                               |
| deltablue                | 7.50 ms                                                      | 3.29 ms: 2.28x faster                                              |
| asyncio_tcp              | 779 ms                                                       | 386 ms: 2.02x faster                                               |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                             |
| richards_super           | 90.6 ms                                                      | 50.5 ms: 1.80x faster                                              |
| go                       | 262 ms                                                       | 148 ms: 1.77x faster                                               |
| logging_silent           | 167 ns                                                       | 95.9 ns: 1.75x faster                                              |
| chaos                    | 109 ms                                                       | 62.3 ms: 1.74x faster                                              |
| scimark_lu               | 167 ms                                                       | 97.6 ms: 1.71x faster                                              |
| richards                 | 75.1 ms                                                      | 44.6 ms: 1.68x faster                                              |
| pyflate                  | 733 ms                                                       | 443 ms: 1.66x faster                                               |
| scimark_sor              | 180 ms                                                       | 111 ms: 1.63x faster                                               |
| raytrace                 | 489 ms                                                       | 308 ms: 1.59x faster                                               |
| sqlglot_parse            | 2.24 ms                                                      | 1.41 ms: 1.58x faster                                              |
| hexiom                   | 9.42 ms                                                      | 5.97 ms: 1.58x faster                                              |
| generators               | 57.3 ms                                                      | 36.7 ms: 1.56x faster                                              |
| scimark_monte_carlo      | 107 ms                                                       | 69.4 ms: 1.55x faster                                              |
| nbody                    | 134 ms                                                       | 87.5 ms: 1.53x faster                                              |
| spectral_norm            | 139 ms                                                       | 91.3 ms: 1.52x faster                                              |
| async_tree_io            | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                             |
| async_tree_none          | 692 ms                                                       | 458 ms: 1.51x faster                                               |
| async_tree_memoization   | 819 ms                                                       | 552 ms: 1.48x faster                                               |
| mako                     | 14.7 ms                                                      | 9.92 ms: 1.48x faster                                              |
| sqlglot_transpile        | 2.68 ms                                                      | 1.81 ms: 1.48x faster                                              |
| unpickle_pure_python     | 312 us                                                       | 212 us: 1.47x faster                                               |
| crypto_pyaes             | 119 ms                                                       | 81.5 ms: 1.46x faster                                              |
| fannkuch                 | 483 ms                                                       | 335 ms: 1.44x faster                                               |
| json_dumps               | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                              |
| pickle_pure_python       | 455 us                                                       | 326 us: 1.40x faster                                               |
| float                    | 111 ms                                                       | 79.6 ms: 1.40x faster                                              |
| pycparser                | 1.67 sec                                                     | 1.23 sec: 1.37x faster                                             |
| tomli_loads              | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                             |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 702 ms: 1.33x faster                                               |
| bench_mp_pool            | 6.37 ms                                                      | 4.79 ms: 1.33x faster                                              |
| deepcopy_memo            | 49.8 us                                                      | 37.7 us: 1.32x faster                                              |
| tornado_http             | 157 ms                                                       | 120 ms: 1.31x faster                                               |
| logging_format           | 9.64 us                                                      | 7.40 us: 1.30x faster                                              |
| regex_compile            | 190 ms                                                       | 146 ms: 1.30x faster                                               |
| coroutines               | 30.3 ms                                                      | 23.3 ms: 1.30x faster                                              |
| logging_simple           | 8.88 us                                                      | 6.84 us: 1.30x faster                                              |
| pprint_pformat           | 2.15 sec                                                     | 1.67 sec: 1.29x faster                                             |
| xml_etree_process        | 75.9 ms                                                      | 58.9 ms: 1.29x faster                                              |
| pprint_safe_repr         | 1.05 sec                                                     | 820 ms: 1.28x faster                                               |
| nqueens                  | 115 ms                                                       | 91.3 ms: 1.26x faster                                              |
| scimark_fft              | 361 ms                                                       | 288 ms: 1.26x faster                                               |
| dulwich_log              | 81.1 ms                                                      | 64.9 ms: 1.25x faster                                              |
| json_loads               | 30.3 us                                                      | 24.4 us: 1.24x faster                                              |
| deepcopy                 | 468 us                                                       | 382 us: 1.23x faster                                               |
| comprehensions           | 26.7 us                                                      | 21.8 us: 1.22x faster                                              |
| 2to3                     | 350 ms                                                       | 287 ms: 1.22x faster                                               |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.21 ms: 1.21x faster                                              |
| sqlglot_normalize        | 144 ms                                                       | 120 ms: 1.20x faster                                               |
| sqlglot_optimize         | 70.1 ms                                                      | 58.6 ms: 1.20x faster                                              |
| mdp                      | 3.01 sec                                                     | 2.52 sec: 1.19x faster                                             |
| docutils                 | 3.41 sec                                                     | 2.90 sec: 1.18x faster                                             |
| bench_thread_pool        | 1.14 ms                                                      | 975 us: 1.17x faster                                               |
| deepcopy_reduce          | 4.01 us                                                      | 3.45 us: 1.16x faster                                              |
| json                     | 5.86 ms                                                      | 5.12 ms: 1.14x faster                                              |
| regex_v8                 | 27.2 ms                                                      | 23.8 ms: 1.14x faster                                              |
| pathlib                  | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                              |
| unpack_sequence          | 59.9 ns                                                      | 53.7 ns: 1.12x faster                                              |
| async_generators         | 421 ms                                                       | 381 ms: 1.10x faster                                               |
| sqlite_synth             | 2.99 us                                                      | 2.72 us: 1.10x faster                                              |
| meteor_contest           | 138 ms                                                       | 126 ms: 1.10x faster                                               |
| xml_etree_parse          | 160 ms                                                       | 146 ms: 1.10x faster                                               |
| regex_dna                | 261 ms                                                       | 238 ms: 1.10x faster                                               |
| xml_etree_generate       | 92.3 ms                                                      | 85.8 ms: 1.08x faster                                              |
| xml_etree_iterparse      | 110 ms                                                       | 103 ms: 1.07x faster                                               |
| create_gc_cycles         | 1.76 ms                                                      | 1.66 ms: 1.06x faster                                              |
| telco                    | 7.23 ms                                                      | 6.99 ms: 1.03x faster                                              |
| pidigits                 | 271 ms                                                       | 264 ms: 1.03x faster                                               |
| python_startup           | 11.5 ms                                                      | 11.7 ms: 1.02x slower                                              |
| unpickle_list            | 4.65 us                                                      | 4.75 us: 1.02x slower                                              |
| gc_traversal             | 3.42 ms                                                      | 3.54 ms: 1.04x slower                                              |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                              |
| pickle_list              | 4.12 us                                                      | 4.46 us: 1.08x slower                                              |
| unpickle                 | 13.5 us                                                      | 14.7 us: 1.09x slower                                              |
| pickle_dict              | 29.5 us                                                      | 32.4 us: 1.10x slower                                              |
| regex_effbot             | 3.09 ms                                                      | 3.52 ms: 1.14x slower                                              |
| python_startup_no_site   | 7.33 ms                                                      | 8.67 ms: 1.18x slower                                              |
| dask                     | 472 ms                                                       | 566 ms: 1.20x slower                                               |
| coverage                 | 63.3 ms                                                      | 88.0 ms: 1.39x slower                                              |
| Geometric mean           | (ref)                                                        | 1.30x faster                                                       |
Ignored benchmarks (18) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.28x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.26x