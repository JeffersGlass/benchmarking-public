
# Results vs. 3.10.4

- fork: python
- ref: v3.11.6
- machine: linux-x86_64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.22x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 285 ms: 1.23x faster                                         |
| chameleon      | 9.44 ms                                                      | 7.64 ms: 1.24x faster                                        |
| docutils       | 3.41 sec                                                     | 2.83 sec: 1.20x faster                                       |
| html5lib       | 94.6 ms                                                      | 71.9 ms: 1.32x faster                                        |
| tornado_http   | 157 ms                                                       | 123 ms: 1.28x faster                                         |
| Geometric mean | (ref)                                                        | 1.25x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                       |
| async_tree_none         | 692 ms                                                       | 519 ms: 1.33x faster                                         |
| async_tree_memoization  | 819 ms                                                       | 622 ms: 1.32x faster                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 751 ms: 1.25x faster                                         |
| Geometric mean          | (ref)                                                        | 1.32x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 111 ms                                                       | 76.4 ms: 1.46x faster                                        |
| nbody          | 134 ms                                                       | 96.9 ms: 1.38x faster                                        |
| pidigits       | 271 ms                                                       | 268 ms: 1.01x faster                                         |
| Geometric mean | (ref)                                                        | 1.27x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 157 ms: 1.21x faster                                         |
| regex_dna      | 261 ms                                                       | 220 ms: 1.19x faster                                         |
| regex_v8       | 27.2 ms                                                      | 23.2 ms: 1.17x faster                                        |
| regex_effbot   | 3.09 ms                                                      | 3.29 ms: 1.06x slower                                        |
| Geometric mean | (ref)                                                        | 1.12x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 315 us: 1.45x faster                                         |
| xml_etree_process    | 75.9 ms                                                      | 55.8 ms: 1.36x faster                                        |
| unpickle_pure_python | 312 us                                                       | 239 us: 1.31x faster                                         |
| tomli_loads          | 2.92 sec                                                     | 2.28 sec: 1.28x faster                                       |
| json_loads           | 30.3 us                                                      | 24.6 us: 1.23x faster                                        |
| xml_etree_generate   | 92.3 ms                                                      | 79.8 ms: 1.16x faster                                        |
| json_dumps           | 14.5 ms                                                      | 13.3 ms: 1.09x faster                                        |
| pickle_list          | 4.12 us                                                      | 3.77 us: 1.09x faster                                        |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.05x faster                                         |
| unpickle             | 13.5 us                                                      | 13.3 us: 1.02x faster                                        |
| unpickle_list        | 4.65 us                                                      | 4.69 us: 1.01x slower                                        |
| pickle               | 9.89 us                                                      | 9.99 us: 1.01x slower                                        |
| pickle_dict          | 29.5 us                                                      | 32.1 us: 1.09x slower                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                 |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.8 ms: 1.06x faster                                        |
| python_startup_no_site | 7.33 ms                                                      | 7.81 ms: 1.07x slower                                        |
| Geometric mean         | (ref)                                                        | 1.00x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.8 ms: 1.36x faster                                        |
| django_template | 50.2 ms                                                      | 40.5 ms: 1.24x faster                                        |
| genshi_text     | 31.4 ms                                                      | 25.4 ms: 1.24x faster                                        |
| genshi_xml      | 63.3 ms                                                      | 56.3 ms: 1.13x faster                                        |
| Geometric mean  | (ref)                                                        | 1.24x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| deltablue                | 7.50 ms                                                      | 3.97 ms: 1.89x faster                                        |
| pyflate                  | 733 ms                                                       | 442 ms: 1.66x faster                                         |
| logging_silent           | 167 ns                                                       | 101 ns: 1.65x faster                                         |
| raytrace                 | 489 ms                                                       | 301 ms: 1.63x faster                                         |
| go                       | 262 ms                                                       | 162 ms: 1.62x faster                                         |
| scimark_sor              | 180 ms                                                       | 112 ms: 1.61x faster                                         |
| scimark_monte_carlo      | 107 ms                                                       | 68.3 ms: 1.57x faster                                        |
| richards                 | 75.1 ms                                                      | 49.6 ms: 1.52x faster                                        |
| chaos                    | 109 ms                                                       | 73.4 ms: 1.48x faster                                        |
| scimark_lu               | 167 ms                                                       | 114 ms: 1.47x faster                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.53 ms: 1.46x faster                                        |
| float                    | 111 ms                                                       | 76.4 ms: 1.46x faster                                        |
| crypto_pyaes             | 119 ms                                                       | 82.4 ms: 1.45x faster                                        |
| pickle_pure_python       | 455 us                                                       | 315 us: 1.45x faster                                         |
| spectral_norm            | 139 ms                                                       | 97.3 ms: 1.43x faster                                        |
| richards_super           | 90.6 ms                                                      | 63.6 ms: 1.42x faster                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.91 ms: 1.40x faster                                        |
| nbody                    | 134 ms                                                       | 96.9 ms: 1.38x faster                                        |
| async_tree_io            | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                       |
| mako                     | 14.7 ms                                                      | 10.8 ms: 1.36x faster                                        |
| xml_etree_process        | 75.9 ms                                                      | 55.8 ms: 1.36x faster                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 775 ms: 1.35x faster                                         |
| hexiom                   | 9.42 ms                                                      | 6.97 ms: 1.35x faster                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.61 sec: 1.34x faster                                       |
| async_tree_none          | 692 ms                                                       | 519 ms: 1.33x faster                                         |
| async_generators         | 421 ms                                                       | 316 ms: 1.33x faster                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.5 us: 1.33x faster                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.82 ms: 1.32x faster                                        |
| async_tree_memoization   | 819 ms                                                       | 622 ms: 1.32x faster                                         |
| html5lib                 | 94.6 ms                                                      | 71.9 ms: 1.32x faster                                        |
| unpack_sequence          | 59.9 ns                                                      | 45.6 ns: 1.31x faster                                        |
| pycparser                | 1.67 sec                                                     | 1.28 sec: 1.31x faster                                       |
| unpickle_pure_python     | 312 us                                                       | 239 us: 1.31x faster                                         |
| tomli_loads              | 2.92 sec                                                     | 2.28 sec: 1.28x faster                                       |
| tornado_http             | 157 ms                                                       | 123 ms: 1.28x faster                                         |
| logging_simple           | 8.88 us                                                      | 6.96 us: 1.28x faster                                        |
| scimark_fft              | 361 ms                                                       | 286 ms: 1.26x faster                                         |
| logging_format           | 9.64 us                                                      | 7.66 us: 1.26x faster                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 751 ms: 1.25x faster                                         |
| dulwich_log              | 81.1 ms                                                      | 65.3 ms: 1.24x faster                                        |
| django_template          | 50.2 ms                                                      | 40.5 ms: 1.24x faster                                        |
| genshi_text              | 31.4 ms                                                      | 25.4 ms: 1.24x faster                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.11 ms: 1.24x faster                                        |
| chameleon                | 9.44 ms                                                      | 7.64 ms: 1.24x faster                                        |
| json_loads               | 30.3 us                                                      | 24.6 us: 1.23x faster                                        |
| thrift                   | 1.18 ms                                                      | 958 us: 1.23x faster                                         |
| 2to3                     | 350 ms                                                       | 285 ms: 1.23x faster                                         |
| sqlalchemy_declarative   | 190 ms                                                       | 155 ms: 1.22x faster                                         |
| deepcopy                 | 468 us                                                       | 383 us: 1.22x faster                                         |
| regex_compile            | 190 ms                                                       | 157 ms: 1.21x faster                                         |
| aiohttp                  | 1.19 ms                                                      | 984 us: 1.21x faster                                         |
| docutils                 | 3.41 sec                                                     | 2.83 sec: 1.20x faster                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 58.6 ms: 1.20x faster                                        |
| sqlite_synth             | 2.99 us                                                      | 2.50 us: 1.20x faster                                        |
| sqlglot_normalize        | 144 ms                                                       | 121 ms: 1.19x faster                                         |
| regex_dna                | 261 ms                                                       | 220 ms: 1.19x faster                                         |
| gunicorn                 | 1.16 ms                                                      | 977 us: 1.19x faster                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.39 us: 1.18x faster                                        |
| regex_v8                 | 27.2 ms                                                      | 23.2 ms: 1.17x faster                                        |
| dask                     | 472 ms                                                       | 407 ms: 1.16x faster                                         |
| xml_etree_generate       | 92.3 ms                                                      | 79.8 ms: 1.16x faster                                        |
| sqlalchemy_imperative    | 22.7 ms                                                      | 19.7 ms: 1.15x faster                                        |
| bench_thread_pool        | 1.14 ms                                                      | 1.00 ms: 1.14x faster                                        |
| nqueens                  | 115 ms                                                       | 101 ms: 1.13x faster                                         |
| flaskblogging            | 4.39 ms                                                      | 3.89 ms: 1.13x faster                                        |
| genshi_xml               | 63.3 ms                                                      | 56.3 ms: 1.13x faster                                        |
| json                     | 5.86 ms                                                      | 5.23 ms: 1.12x faster                                        |
| pathlib                  | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                        |
| fannkuch                 | 483 ms                                                       | 437 ms: 1.10x faster                                         |
| pylint                   | 566 ms                                                       | 514 ms: 1.10x faster                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.61 ms: 1.09x faster                                        |
| json_dumps               | 14.5 ms                                                      | 13.3 ms: 1.09x faster                                        |
| pickle_list              | 4.12 us                                                      | 3.77 us: 1.09x faster                                        |
| sympy_expand             | 600 ms                                                       | 550 ms: 1.09x faster                                         |
| sympy_integrate          | 28.2 ms                                                      | 25.9 ms: 1.09x faster                                        |
| coroutines               | 30.3 ms                                                      | 27.9 ms: 1.09x faster                                        |
| meteor_contest           | 138 ms                                                       | 128 ms: 1.08x faster                                         |
| sympy_str                | 360 ms                                                       | 335 ms: 1.08x faster                                         |
| comprehensions           | 26.7 us                                                      | 24.8 us: 1.07x faster                                        |
| python_startup           | 11.5 ms                                                      | 10.8 ms: 1.06x faster                                        |
| telco                    | 7.23 ms                                                      | 6.80 ms: 1.06x faster                                        |
| generators               | 57.3 ms                                                      | 54.3 ms: 1.06x faster                                        |
| mdp                      | 3.01 sec                                                     | 2.86 sec: 1.05x faster                                       |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.05x faster                                         |
| sympy_sum                | 193 ms                                                       | 184 ms: 1.05x faster                                         |
| asyncio_tcp              | 779 ms                                                       | 747 ms: 1.04x faster                                         |
| typing_runtime_protocols | 537 us                                                       | 519 us: 1.03x faster                                         |
| unpickle                 | 13.5 us                                                      | 13.3 us: 1.02x faster                                        |
| pidigits                 | 271 ms                                                       | 268 ms: 1.01x faster                                         |
| unpickle_list            | 4.65 us                                                      | 4.69 us: 1.01x slower                                        |
| pickle                   | 9.89 us                                                      | 9.99 us: 1.01x slower                                        |
| regex_effbot             | 3.09 ms                                                      | 3.29 ms: 1.06x slower                                        |
| python_startup_no_site   | 7.33 ms                                                      | 7.81 ms: 1.07x slower                                        |
| pickle_dict              | 29.5 us                                                      | 32.1 us: 1.09x slower                                        |
| gc_traversal             | 3.42 ms                                                      | 3.97 ms: 1.16x slower                                        |
| Geometric mean           | (ref)                                                        | 1.22x faster                                                 |

Benchmark hidden because not significant (2): xml_etree_parse, asyncio_tcp_ssl
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.10x