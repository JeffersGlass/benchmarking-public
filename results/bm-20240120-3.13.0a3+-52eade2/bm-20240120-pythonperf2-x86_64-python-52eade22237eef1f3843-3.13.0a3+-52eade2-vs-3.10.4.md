
# Results vs. 3.10.4

- fork: python
- ref: 52eade22237eef1f3843
- machine: linux-x86_64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 293 ms: 1.19x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.16 ms: 1.32x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                                       |
| tornado_http   | 157 ms                                                       | 117 ms: 1.34x faster                                                         |
| Geometric mean | (ref)                                                        | 1.26x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 547 ms: 1.50x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 698 ms: 1.34x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.48x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 88.6 ms: 1.51x faster                                                        |
| float          | 111 ms                                                       | 79.9 ms: 1.39x faster                                                        |
| pidigits       | 271 ms                                                       | 264 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.29x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 140 ms: 1.36x faster                                                         |
| regex_dna      | 261 ms                                                       | 239 ms: 1.09x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 26.7 ms: 1.02x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.59 ms: 1.16x slower                                                        |
| Geometric mean | (ref)                                                        | 1.07x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 307 us: 1.48x faster                                                         |
| unpickle_pure_python | 312 us                                                       | 211 us: 1.48x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 57.3 ms: 1.32x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.31 sec: 1.26x faster                                                       |
| json_loads           | 30.3 us                                                      | 25.0 us: 1.21x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 84.7 ms: 1.09x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.03x faster                                                         |
| xml_etree_parse      | 160 ms                                                       | 156 ms: 1.02x faster                                                         |
| pickle_dict          | 29.5 us                                                      | 30.7 us: 1.04x slower                                                        |
| unpickle_list        | 4.65 us                                                      | 4.88 us: 1.05x slower                                                        |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.39 us: 1.06x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.4 ms: 1.42x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 114 us: 4.71x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 365 ms: 2.13x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.53 ms: 2.13x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 263 ms: 1.86x faster                                                         |
| chaos                    | 109 ms                                                       | 58.9 ms: 1.84x faster                                                        |
| logging_silent           | 167 ns                                                       | 95.8 ns: 1.75x faster                                                        |
| scimark_lu               | 167 ms                                                       | 96.1 ms: 1.74x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 70.0 ms: 1.70x faster                                                        |
| generators               | 57.3 ms                                                      | 33.8 ms: 1.70x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.36 ms: 1.65x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 66.3 ms: 1.62x faster                                                        |
| comprehensions           | 26.7 us                                                      | 16.5 us: 1.61x faster                                                        |
| async_tree_none          | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| go                       | 262 ms                                                       | 169 ms: 1.55x faster                                                         |
| richards_super           | 90.6 ms                                                      | 58.9 ms: 1.54x faster                                                        |
| spectral_norm            | 139 ms                                                       | 91.4 ms: 1.52x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.77 ms: 1.52x faster                                                        |
| nbody                    | 134 ms                                                       | 88.6 ms: 1.51x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 547 ms: 1.50x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| pickle_pure_python       | 455 us                                                       | 307 us: 1.48x faster                                                         |
| unpickle_pure_python     | 312 us                                                       | 211 us: 1.48x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 6.39 ms: 1.47x faster                                                        |
| richards                 | 75.1 ms                                                      | 52.2 ms: 1.44x faster                                                        |
| mako                     | 14.7 ms                                                      | 10.4 ms: 1.42x faster                                                        |
| pyflate                  | 733 ms                                                       | 518 ms: 1.41x faster                                                         |
| float                    | 111 ms                                                       | 79.9 ms: 1.39x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.04 us: 1.37x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.1 ms: 1.37x faster                                                        |
| logging_simple           | 8.88 us                                                      | 6.50 us: 1.37x faster                                                        |
| regex_compile            | 190 ms                                                       | 140 ms: 1.36x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.0 us: 1.35x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.74 ms: 1.34x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 698 ms: 1.34x faster                                                         |
| tornado_http             | 157 ms                                                       | 117 ms: 1.34x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.62 sec: 1.33x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 57.3 ms: 1.32x faster                                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 796 ms: 1.32x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.16 ms: 1.32x faster                                                        |
| nqueens                  | 115 ms                                                       | 87.6 ms: 1.31x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                                       |
| scimark_sor              | 180 ms                                                       | 141 ms: 1.28x faster                                                         |
| deepcopy                 | 468 us                                                       | 367 us: 1.28x faster                                                         |
| sympy_sum                | 193 ms                                                       | 152 ms: 1.27x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.01 ms: 1.27x faster                                                        |
| fannkuch                 | 483 ms                                                       | 382 ms: 1.26x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.31 sec: 1.26x faster                                                       |
| sqlglot_normalize        | 144 ms                                                       | 115 ms: 1.25x faster                                                         |
| sympy_str                | 360 ms                                                       | 290 ms: 1.24x faster                                                         |
| sympy_expand             | 600 ms                                                       | 491 ms: 1.22x faster                                                         |
| scimark_fft              | 361 ms                                                       | 296 ms: 1.22x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 23.1 ms: 1.22x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.47 sec: 1.22x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.30 us: 1.21x faster                                                        |
| json_loads               | 30.3 us                                                      | 25.0 us: 1.21x faster                                                        |
| docutils                 | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 58.6 ms: 1.20x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 67.9 ms: 1.20x faster                                                        |
| 2to3                     | 350 ms                                                       | 293 ms: 1.19x faster                                                         |
| dask                     | 472 ms                                                       | 396 ms: 1.19x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 964 us: 1.18x faster                                                         |
| async_generators         | 421 ms                                                       | 363 ms: 1.16x faster                                                         |
| unpack_sequence          | 59.9 ns                                                      | 52.1 ns: 1.15x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 18.7 ms: 1.14x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.56 ms: 1.13x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.70 us: 1.11x faster                                                        |
| json                     | 5.86 ms                                                      | 5.30 ms: 1.11x faster                                                        |
| regex_dna                | 261 ms                                                       | 239 ms: 1.09x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 84.7 ms: 1.09x faster                                                        |
| mypy2                    | 933 ms                                                       | 857 ms: 1.09x faster                                                         |
| meteor_contest           | 138 ms                                                       | 127 ms: 1.09x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.03x faster                                                         |
| pidigits                 | 271 ms                                                       | 264 ms: 1.03x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 156 ms: 1.02x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 26.7 ms: 1.02x faster                                                        |
| pickle_dict              | 29.5 us                                                      | 30.7 us: 1.04x slower                                                        |
| unpickle_list            | 4.65 us                                                      | 4.88 us: 1.05x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.39 us: 1.06x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.05 ms: 1.11x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.59 ms: 1.16x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 4.00 ms: 1.17x slower                                                        |
| coverage                 | 63.3 ms                                                      | 80.5 ms: 1.27x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.29x faster                                                                 |

Benchmark hidden because not significant (1): asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.07x