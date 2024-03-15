
# Results vs. 3.11.0

- fork: python
- ref: v3.10.4
- machine: linux-x86_64
- commit hash: 9d38120
- commit date: 2022-03-23
- overall geometric mean: 1.21x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 350 ms: 1.22x slower                                         |
| chameleon      | 7.92 ms                                                      | 9.44 ms: 1.19x slower                                        |
| docutils       | 2.85 sec                                                     | 3.41 sec: 1.20x slower                                       |
| html5lib       | 72.2 ms                                                      | 94.6 ms: 1.31x slower                                        |
| tornado_http   | 124 ms                                                       | 157 ms: 1.26x slower                                         |
| Geometric mean | (ref)                                                        | 1.24x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 936 ms: 1.24x slower                                         |
| async_tree_memoization  | 629 ms                                                       | 819 ms: 1.30x slower                                         |
| async_tree_none         | 518 ms                                                       | 692 ms: 1.34x slower                                         |
| async_tree_io           | 1.17 sec                                                     | 1.60 sec: 1.36x slower                                       |
| Geometric mean          | (ref)                                                        | 1.31x slower                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 271 ms: 1.08x slower                                         |
| nbody          | 92.9 ms                                                      | 134 ms: 1.44x slower                                         |
| float          | 74.9 ms                                                      | 111 ms: 1.48x slower                                         |
| Geometric mean | (ref)                                                        | 1.32x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.09 ms: 1.08x faster                                        |
| regex_v8       | 24.4 ms                                                      | 27.2 ms: 1.11x slower                                        |
| regex_dna      | 227 ms                                                       | 261 ms: 1.15x slower                                         |
| regex_compile  | 156 ms                                                       | 190 ms: 1.22x slower                                         |
| Geometric mean | (ref)                                                        | 1.09x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict          | 32.3 us                                                      | 29.5 us: 1.10x faster                                        |
| unpickle_list        | 4.60 us                                                      | 4.65 us: 1.01x slower                                        |
| unpickle             | 13.3 us                                                      | 13.5 us: 1.02x slower                                        |
| xml_etree_iterparse  | 107 ms                                                       | 110 ms: 1.03x slower                                         |
| xml_etree_parse      | 155 ms                                                       | 160 ms: 1.04x slower                                         |
| pickle_list          | 3.94 us                                                      | 4.12 us: 1.05x slower                                        |
| json_loads           | 28.9 us                                                      | 30.3 us: 1.05x slower                                        |
| json_dumps           | 13.3 ms                                                      | 14.5 ms: 1.10x slower                                        |
| xml_etree_generate   | 79.7 ms                                                      | 92.3 ms: 1.16x slower                                        |
| tomli_loads          | 2.25 sec                                                     | 2.92 sec: 1.30x slower                                       |
| unpickle_pure_python | 238 us                                                       | 312 us: 1.31x slower                                         |
| xml_etree_process    | 55.9 ms                                                      | 75.9 ms: 1.36x slower                                        |
| pickle_pure_python   | 316 us                                                       | 455 us: 1.44x slower                                         |
| Geometric mean       | (ref)                                                        | 1.12x slower                                                 |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.33 ms: 1.06x faster                                        |
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                        |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 63.3 ms: 1.11x slower                                        |
| genshi_text     | 25.5 ms                                                      | 31.4 ms: 1.23x slower                                        |
| django_template | 39.3 ms                                                      | 50.2 ms: 1.28x slower                                        |
| mako            | 11.0 ms                                                      | 14.7 ms: 1.34x slower                                        |
| Geometric mean  | (ref)                                                        | 1.24x slower                                                 |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| gc_traversal             | 4.15 ms                                                      | 3.42 ms: 1.21x faster                                        |
| pickle_dict              | 32.3 us                                                      | 29.5 us: 1.10x faster                                        |
| regex_effbot             | 3.34 ms                                                      | 3.09 ms: 1.08x faster                                        |
| python_startup_no_site   | 7.73 ms                                                      | 7.33 ms: 1.06x faster                                        |
| coverage                 | 66.1 ms                                                      | 63.3 ms: 1.04x faster                                        |
| typing_runtime_protocols | 532 us                                                       | 537 us: 1.01x slower                                         |
| unpickle_list            | 4.60 us                                                      | 4.65 us: 1.01x slower                                        |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 3.10 sec: 1.01x slower                                       |
| unpickle                 | 13.3 us                                                      | 13.5 us: 1.02x slower                                        |
| xml_etree_iterparse      | 107 ms                                                       | 110 ms: 1.03x slower                                         |
| xml_etree_parse          | 155 ms                                                       | 160 ms: 1.04x slower                                         |
| sympy_sum                | 186 ms                                                       | 193 ms: 1.04x slower                                         |
| asyncio_tcp              | 747 ms                                                       | 779 ms: 1.04x slower                                         |
| pickle_list              | 3.94 us                                                      | 4.12 us: 1.05x slower                                        |
| json_loads               | 28.9 us                                                      | 30.3 us: 1.05x slower                                        |
| generators               | 54.6 ms                                                      | 57.3 ms: 1.05x slower                                        |
| json                     | 5.58 ms                                                      | 5.86 ms: 1.05x slower                                        |
| meteor_contest           | 131 ms                                                       | 138 ms: 1.06x slower                                         |
| telco                    | 6.81 ms                                                      | 7.23 ms: 1.06x slower                                        |
| comprehensions           | 25.1 us                                                      | 26.7 us: 1.06x slower                                        |
| sympy_str                | 337 ms                                                       | 360 ms: 1.07x slower                                         |
| python_startup           | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                        |
| pidigits                 | 251 ms                                                       | 271 ms: 1.08x slower                                         |
| mdp                      | 2.77 sec                                                     | 3.01 sec: 1.08x slower                                       |
| sympy_expand             | 553 ms                                                       | 600 ms: 1.09x slower                                         |
| coroutines               | 27.8 ms                                                      | 30.3 ms: 1.09x slower                                        |
| sympy_integrate          | 25.8 ms                                                      | 28.2 ms: 1.09x slower                                        |
| json_dumps               | 13.3 ms                                                      | 14.5 ms: 1.10x slower                                        |
| pylint                   | 514 ms                                                       | 566 ms: 1.10x slower                                         |
| genshi_xml               | 57.1 ms                                                      | 63.3 ms: 1.11x slower                                        |
| regex_v8                 | 24.4 ms                                                      | 27.2 ms: 1.11x slower                                        |
| create_gc_cycles         | 1.58 ms                                                      | 1.76 ms: 1.12x slower                                        |
| nqueens                  | 103 ms                                                       | 115 ms: 1.12x slower                                         |
| pathlib                  | 18.9 ms                                                      | 21.4 ms: 1.13x slower                                        |
| flaskblogging            | 3.88 ms                                                      | 4.39 ms: 1.13x slower                                        |
| bench_thread_pool        | 1.00 ms                                                      | 1.14 ms: 1.14x slower                                        |
| regex_dna                | 227 ms                                                       | 261 ms: 1.15x slower                                         |
| sqlalchemy_imperative    | 19.8 ms                                                      | 22.7 ms: 1.15x slower                                        |
| dask                     | 410 ms                                                       | 472 ms: 1.15x slower                                         |
| xml_etree_generate       | 79.7 ms                                                      | 92.3 ms: 1.16x slower                                        |
| fannkuch                 | 416 ms                                                       | 483 ms: 1.16x slower                                         |
| deepcopy_reduce          | 3.40 us                                                      | 4.01 us: 1.18x slower                                        |
| sqlglot_normalize        | 122 ms                                                       | 144 ms: 1.18x slower                                         |
| sqlite_synth             | 2.52 us                                                      | 2.99 us: 1.19x slower                                        |
| sqlglot_optimize         | 59.0 ms                                                      | 70.1 ms: 1.19x slower                                        |
| chameleon                | 7.92 ms                                                      | 9.44 ms: 1.19x slower                                        |
| deepcopy                 | 391 us                                                       | 468 us: 1.20x slower                                         |
| docutils                 | 2.85 sec                                                     | 3.41 sec: 1.20x slower                                       |
| gunicorn                 | 966 us                                                       | 1.16 ms: 1.20x slower                                        |
| dulwich_log              | 67.4 ms                                                      | 81.1 ms: 1.20x slower                                        |
| aiohttp                  | 986 us                                                       | 1.19 ms: 1.21x slower                                        |
| regex_compile            | 156 ms                                                       | 190 ms: 1.22x slower                                         |
| 2to3                     | 287 ms                                                       | 350 ms: 1.22x slower                                         |
| mypy2                    | 762 ms                                                       | 933 ms: 1.22x slower                                         |
| logging_simple           | 7.24 us                                                      | 8.88 us: 1.23x slower                                        |
| sqlalchemy_declarative   | 154 ms                                                       | 190 ms: 1.23x slower                                         |
| genshi_text              | 25.5 ms                                                      | 31.4 ms: 1.23x slower                                        |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 936 ms: 1.24x slower                                         |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 5.08 ms: 1.25x slower                                        |
| logging_format           | 7.71 us                                                      | 9.64 us: 1.25x slower                                        |
| tornado_http             | 124 ms                                                       | 157 ms: 1.26x slower                                         |
| thrift                   | 931 us                                                       | 1.18 ms: 1.26x slower                                        |
| django_template          | 39.3 ms                                                      | 50.2 ms: 1.28x slower                                        |
| pycparser                | 1.31 sec                                                     | 1.67 sec: 1.28x slower                                       |
| scimark_fft              | 281 ms                                                       | 361 ms: 1.29x slower                                         |
| pprint_pformat           | 1.67 sec                                                     | 2.15 sec: 1.29x slower                                       |
| tomli_loads              | 2.25 sec                                                     | 2.92 sec: 1.30x slower                                       |
| async_tree_memoization   | 629 ms                                                       | 819 ms: 1.30x slower                                         |
| pprint_safe_repr         | 805 ms                                                       | 1.05 sec: 1.30x slower                                       |
| async_generators         | 322 ms                                                       | 421 ms: 1.31x slower                                         |
| unpickle_pure_python     | 238 us                                                       | 312 us: 1.31x slower                                         |
| html5lib                 | 72.2 ms                                                      | 94.6 ms: 1.31x slower                                        |
| unpack_sequence          | 45.7 ns                                                      | 59.9 ns: 1.31x slower                                        |
| deepcopy_memo            | 37.5 us                                                      | 49.8 us: 1.33x slower                                        |
| async_tree_none          | 518 ms                                                       | 692 ms: 1.34x slower                                         |
| mako                     | 11.0 ms                                                      | 14.7 ms: 1.34x slower                                        |
| hexiom                   | 6.98 ms                                                      | 9.42 ms: 1.35x slower                                        |
| bench_mp_pool            | 4.70 ms                                                      | 6.37 ms: 1.36x slower                                        |
| xml_etree_process        | 55.9 ms                                                      | 75.9 ms: 1.36x slower                                        |
| async_tree_io            | 1.17 sec                                                     | 1.60 sec: 1.36x slower                                       |
| sqlglot_transpile        | 1.91 ms                                                      | 2.68 ms: 1.40x slower                                        |
| richards_super           | 63.6 ms                                                      | 90.6 ms: 1.42x slower                                        |
| crypto_pyaes             | 83.3 ms                                                      | 119 ms: 1.43x slower                                         |
| pickle_pure_python       | 316 us                                                       | 455 us: 1.44x slower                                         |
| nbody                    | 92.9 ms                                                      | 134 ms: 1.44x slower                                         |
| chaos                    | 74.9 ms                                                      | 109 ms: 1.45x slower                                         |
| scimark_lu               | 114 ms                                                       | 167 ms: 1.46x slower                                         |
| spectral_norm            | 95.1 ms                                                      | 139 ms: 1.46x slower                                         |
| sqlglot_parse            | 1.51 ms                                                      | 2.24 ms: 1.48x slower                                        |
| float                    | 74.9 ms                                                      | 111 ms: 1.48x slower                                         |
| richards                 | 49.7 ms                                                      | 75.1 ms: 1.51x slower                                        |
| scimark_monte_carlo      | 69.8 ms                                                      | 107 ms: 1.54x slower                                         |
| raytrace                 | 309 ms                                                       | 489 ms: 1.58x slower                                         |
| pyflate                  | 449 ms                                                       | 733 ms: 1.63x slower                                         |
| scimark_sor              | 110 ms                                                       | 180 ms: 1.64x slower                                         |
| go                       | 158 ms                                                       | 262 ms: 1.66x slower                                         |
| logging_silent           | 100 ns                                                       | 167 ns: 1.67x slower                                         |
| deltablue                | 3.97 ms                                                      | 7.50 ms: 1.89x slower                                        |
| Geometric mean           | (ref)                                                        | 1.21x slower                                                 |

Benchmark hidden because not significant (2): pickle, asyncio_websockets
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.19x
- 95% likely to have a slowdown of 1.18x
- 99% likely to have a slowdown of 1.16x


# Memory

- memory change: 0.93x