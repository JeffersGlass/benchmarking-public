
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0
- machine: linux-x86_64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.21x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 287 ms: 1.22x faster                                         |
| chameleon      | 9.44 ms                                                      | 7.92 ms: 1.19x faster                                        |
| docutils       | 3.41 sec                                                     | 2.85 sec: 1.20x faster                                       |
| html5lib       | 94.6 ms                                                      | 72.2 ms: 1.31x faster                                        |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                         |
| Geometric mean | (ref)                                                        | 1.24x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                       |
| async_tree_none         | 692 ms                                                       | 518 ms: 1.34x faster                                         |
| async_tree_memoization  | 819 ms                                                       | 629 ms: 1.30x faster                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 753 ms: 1.24x faster                                         |
| Geometric mean          | (ref)                                                        | 1.31x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 111 ms                                                       | 74.9 ms: 1.48x faster                                        |
| nbody          | 134 ms                                                       | 92.9 ms: 1.44x faster                                        |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                         |
| Geometric mean | (ref)                                                        | 1.32x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 156 ms: 1.22x faster                                         |
| regex_dna      | 261 ms                                                       | 227 ms: 1.15x faster                                         |
| regex_v8       | 27.2 ms                                                      | 24.4 ms: 1.11x faster                                        |
| regex_effbot   | 3.09 ms                                                      | 3.34 ms: 1.08x slower                                        |
| Geometric mean | (ref)                                                        | 1.09x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 316 us: 1.44x faster                                         |
| xml_etree_process    | 75.9 ms                                                      | 55.9 ms: 1.36x faster                                        |
| unpickle_pure_python | 312 us                                                       | 238 us: 1.31x faster                                         |
| tomli_loads          | 2.92 sec                                                     | 2.25 sec: 1.30x faster                                       |
| xml_etree_generate   | 92.3 ms                                                      | 79.7 ms: 1.16x faster                                        |
| json_dumps           | 14.5 ms                                                      | 13.3 ms: 1.10x faster                                        |
| json_loads           | 30.3 us                                                      | 28.9 us: 1.05x faster                                        |
| pickle_list          | 4.12 us                                                      | 3.94 us: 1.05x faster                                        |
| xml_etree_parse      | 160 ms                                                       | 155 ms: 1.04x faster                                         |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.03x faster                                         |
| unpickle             | 13.5 us                                                      | 13.3 us: 1.02x faster                                        |
| unpickle_list        | 4.65 us                                                      | 4.60 us: 1.01x faster                                        |
| pickle_dict          | 29.5 us                                                      | 32.3 us: 1.10x slower                                        |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                 |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.7 ms: 1.07x faster                                        |
| python_startup_no_site | 7.33 ms                                                      | 7.73 ms: 1.06x slower                                        |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 11.0 ms: 1.34x faster                                        |
| django_template | 50.2 ms                                                      | 39.3 ms: 1.28x faster                                        |
| genshi_text     | 31.4 ms                                                      | 25.5 ms: 1.23x faster                                        |
| genshi_xml      | 63.3 ms                                                      | 57.1 ms: 1.11x faster                                        |
| Geometric mean  | (ref)                                                        | 1.24x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| deltablue                | 7.50 ms                                                      | 3.97 ms: 1.89x faster                                        |
| logging_silent           | 167 ns                                                       | 100 ns: 1.67x faster                                         |
| go                       | 262 ms                                                       | 158 ms: 1.66x faster                                         |
| scimark_sor              | 180 ms                                                       | 110 ms: 1.64x faster                                         |
| pyflate                  | 733 ms                                                       | 449 ms: 1.63x faster                                         |
| raytrace                 | 489 ms                                                       | 309 ms: 1.58x faster                                         |
| scimark_monte_carlo      | 107 ms                                                       | 69.8 ms: 1.54x faster                                        |
| richards                 | 75.1 ms                                                      | 49.7 ms: 1.51x faster                                        |
| float                    | 111 ms                                                       | 74.9 ms: 1.48x faster                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.51 ms: 1.48x faster                                        |
| spectral_norm            | 139 ms                                                       | 95.1 ms: 1.46x faster                                        |
| scimark_lu               | 167 ms                                                       | 114 ms: 1.46x faster                                         |
| chaos                    | 109 ms                                                       | 74.9 ms: 1.45x faster                                        |
| nbody                    | 134 ms                                                       | 92.9 ms: 1.44x faster                                        |
| pickle_pure_python       | 455 us                                                       | 316 us: 1.44x faster                                         |
| crypto_pyaes             | 119 ms                                                       | 83.3 ms: 1.43x faster                                        |
| richards_super           | 90.6 ms                                                      | 63.6 ms: 1.42x faster                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.91 ms: 1.40x faster                                        |
| async_tree_io            | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                       |
| xml_etree_process        | 75.9 ms                                                      | 55.9 ms: 1.36x faster                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.70 ms: 1.36x faster                                        |
| hexiom                   | 9.42 ms                                                      | 6.98 ms: 1.35x faster                                        |
| mako                     | 14.7 ms                                                      | 11.0 ms: 1.34x faster                                        |
| async_tree_none          | 692 ms                                                       | 518 ms: 1.34x faster                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.5 us: 1.33x faster                                        |
| unpack_sequence          | 59.9 ns                                                      | 45.7 ns: 1.31x faster                                        |
| html5lib                 | 94.6 ms                                                      | 72.2 ms: 1.31x faster                                        |
| unpickle_pure_python     | 312 us                                                       | 238 us: 1.31x faster                                         |
| async_generators         | 421 ms                                                       | 322 ms: 1.31x faster                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 805 ms: 1.30x faster                                         |
| async_tree_memoization   | 819 ms                                                       | 629 ms: 1.30x faster                                         |
| tomli_loads              | 2.92 sec                                                     | 2.25 sec: 1.30x faster                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.67 sec: 1.29x faster                                       |
| scimark_fft              | 361 ms                                                       | 281 ms: 1.29x faster                                         |
| pycparser                | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                       |
| django_template          | 50.2 ms                                                      | 39.3 ms: 1.28x faster                                        |
| thrift                   | 1.18 ms                                                      | 931 us: 1.26x faster                                         |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                         |
| logging_format           | 9.64 us                                                      | 7.71 us: 1.25x faster                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.06 ms: 1.25x faster                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 753 ms: 1.24x faster                                         |
| genshi_text              | 31.4 ms                                                      | 25.5 ms: 1.23x faster                                        |
| sqlalchemy_declarative   | 190 ms                                                       | 154 ms: 1.23x faster                                         |
| logging_simple           | 8.88 us                                                      | 7.24 us: 1.23x faster                                        |
| mypy2                    | 933 ms                                                       | 762 ms: 1.22x faster                                         |
| 2to3                     | 350 ms                                                       | 287 ms: 1.22x faster                                         |
| regex_compile            | 190 ms                                                       | 156 ms: 1.22x faster                                         |
| aiohttp                  | 1.19 ms                                                      | 986 us: 1.21x faster                                         |
| dulwich_log              | 81.1 ms                                                      | 67.4 ms: 1.20x faster                                        |
| gunicorn                 | 1.16 ms                                                      | 966 us: 1.20x faster                                         |
| docutils                 | 3.41 sec                                                     | 2.85 sec: 1.20x faster                                       |
| deepcopy                 | 468 us                                                       | 391 us: 1.20x faster                                         |
| chameleon                | 9.44 ms                                                      | 7.92 ms: 1.19x faster                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 59.0 ms: 1.19x faster                                        |
| sqlite_synth             | 2.99 us                                                      | 2.52 us: 1.19x faster                                        |
| sqlglot_normalize        | 144 ms                                                       | 122 ms: 1.18x faster                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.40 us: 1.18x faster                                        |
| fannkuch                 | 483 ms                                                       | 416 ms: 1.16x faster                                         |
| xml_etree_generate       | 92.3 ms                                                      | 79.7 ms: 1.16x faster                                        |
| dask                     | 472 ms                                                       | 410 ms: 1.15x faster                                         |
| sqlalchemy_imperative    | 22.7 ms                                                      | 19.8 ms: 1.15x faster                                        |
| regex_dna                | 261 ms                                                       | 227 ms: 1.15x faster                                         |
| bench_thread_pool        | 1.14 ms                                                      | 1.00 ms: 1.14x faster                                        |
| flaskblogging            | 4.39 ms                                                      | 3.88 ms: 1.13x faster                                        |
| pathlib                  | 21.4 ms                                                      | 18.9 ms: 1.13x faster                                        |
| nqueens                  | 115 ms                                                       | 103 ms: 1.12x faster                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.58 ms: 1.12x faster                                        |
| regex_v8                 | 27.2 ms                                                      | 24.4 ms: 1.11x faster                                        |
| genshi_xml               | 63.3 ms                                                      | 57.1 ms: 1.11x faster                                        |
| pylint                   | 566 ms                                                       | 514 ms: 1.10x faster                                         |
| json_dumps               | 14.5 ms                                                      | 13.3 ms: 1.10x faster                                        |
| sympy_integrate          | 28.2 ms                                                      | 25.8 ms: 1.09x faster                                        |
| coroutines               | 30.3 ms                                                      | 27.8 ms: 1.09x faster                                        |
| sympy_expand             | 600 ms                                                       | 553 ms: 1.09x faster                                         |
| mdp                      | 3.01 sec                                                     | 2.77 sec: 1.08x faster                                       |
| pidigits                 | 271 ms                                                       | 251 ms: 1.08x faster                                         |
| python_startup           | 11.5 ms                                                      | 10.7 ms: 1.07x faster                                        |
| sympy_str                | 360 ms                                                       | 337 ms: 1.07x faster                                         |
| comprehensions           | 26.7 us                                                      | 25.1 us: 1.06x faster                                        |
| telco                    | 7.23 ms                                                      | 6.81 ms: 1.06x faster                                        |
| meteor_contest           | 138 ms                                                       | 131 ms: 1.06x faster                                         |
| json                     | 5.86 ms                                                      | 5.58 ms: 1.05x faster                                        |
| generators               | 57.3 ms                                                      | 54.6 ms: 1.05x faster                                        |
| json_loads               | 30.3 us                                                      | 28.9 us: 1.05x faster                                        |
| pickle_list              | 4.12 us                                                      | 3.94 us: 1.05x faster                                        |
| asyncio_tcp              | 779 ms                                                       | 747 ms: 1.04x faster                                         |
| sympy_sum                | 193 ms                                                       | 186 ms: 1.04x faster                                         |
| xml_etree_parse          | 160 ms                                                       | 155 ms: 1.04x faster                                         |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.03x faster                                         |
| unpickle                 | 13.5 us                                                      | 13.3 us: 1.02x faster                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 3.07 sec: 1.01x faster                                       |
| unpickle_list            | 4.65 us                                                      | 4.60 us: 1.01x faster                                        |
| typing_runtime_protocols | 537 us                                                       | 532 us: 1.01x faster                                         |
| coverage                 | 63.3 ms                                                      | 66.1 ms: 1.04x slower                                        |
| python_startup_no_site   | 7.33 ms                                                      | 7.73 ms: 1.06x slower                                        |
| regex_effbot             | 3.09 ms                                                      | 3.34 ms: 1.08x slower                                        |
| pickle_dict              | 29.5 us                                                      | 32.3 us: 1.10x slower                                        |
| gc_traversal             | 3.42 ms                                                      | 4.15 ms: 1.21x slower                                        |
| Geometric mean           | (ref)                                                        | 1.21x faster                                                 |

Benchmark hidden because not significant (2): asyncio_websockets, pickle
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.08x