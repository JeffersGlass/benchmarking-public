
# Results vs. 3.10.4

- fork: python
- ref: v3.12.1
- machine: linux-x86_64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.31x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 281 ms: 1.25x faster                                         |
| chameleon      | 9.44 ms                                                      | 7.31 ms: 1.29x faster                                        |
| docutils       | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                       |
| tornado_http   | 157 ms                                                       | 118 ms: 1.32x faster                                         |
| Geometric mean | (ref)                                                        | 1.27x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 450 ms: 1.54x faster                                         |
| async_tree_io           | 1.60 sec                                                     | 1.04 sec: 1.53x faster                                       |
| async_tree_memoization  | 819 ms                                                       | 544 ms: 1.51x faster                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 693 ms: 1.35x faster                                         |
| Geometric mean          | (ref)                                                        | 1.48x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 85.5 ms: 1.57x faster                                        |
| float          | 111 ms                                                       | 77.0 ms: 1.44x faster                                        |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                         |
| Geometric mean | (ref)                                                        | 1.32x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 138 ms: 1.37x faster                                         |
| regex_v8       | 27.2 ms                                                      | 23.5 ms: 1.15x faster                                        |
| regex_dna      | 261 ms                                                       | 244 ms: 1.07x faster                                         |
| regex_effbot   | 3.09 ms                                                      | 3.54 ms: 1.15x slower                                        |
| Geometric mean | (ref)                                                        | 1.10x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 205 us: 1.52x faster                                         |
| pickle_pure_python   | 455 us                                                       | 320 us: 1.42x faster                                         |
| json_dumps           | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                        |
| tomli_loads          | 2.92 sec                                                     | 2.14 sec: 1.36x faster                                       |
| xml_etree_process    | 75.9 ms                                                      | 58.0 ms: 1.31x faster                                        |
| json_loads           | 30.3 us                                                      | 24.6 us: 1.23x faster                                        |
| xml_etree_parse      | 160 ms                                                       | 145 ms: 1.10x faster                                         |
| xml_etree_generate   | 92.3 ms                                                      | 84.6 ms: 1.09x faster                                        |
| xml_etree_iterparse  | 110 ms                                                       | 102 ms: 1.09x faster                                         |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                        |
| unpickle_list        | 4.65 us                                                      | 4.82 us: 1.04x slower                                        |
| pickle_dict          | 29.5 us                                                      | 31.2 us: 1.06x slower                                        |
| pickle_list          | 4.12 us                                                      | 4.46 us: 1.08x slower                                        |
| unpickle             | 13.5 us                                                      | 15.2 us: 1.13x slower                                        |
| Geometric mean       | (ref)                                                        | 1.14x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.5 ms: 1.00x slower                                        |
| python_startup_no_site | 7.33 ms                                                      | 8.53 ms: 1.16x slower                                        |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.1 ms: 1.46x faster                                        |
| django_template | 50.2 ms                                                      | 37.5 ms: 1.34x faster                                        |
| Geometric mean  | (ref)                                                        | 1.40x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 122 us: 4.40x faster                                         |
| deltablue                | 7.50 ms                                                      | 3.24 ms: 2.31x faster                                        |
| asyncio_tcp              | 779 ms                                                       | 374 ms: 2.08x faster                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.98x faster                                       |
| richards_super           | 90.6 ms                                                      | 50.7 ms: 1.79x faster                                        |
| go                       | 262 ms                                                       | 149 ms: 1.76x faster                                         |
| chaos                    | 109 ms                                                       | 62.1 ms: 1.75x faster                                        |
| logging_silent           | 167 ns                                                       | 95.8 ns: 1.75x faster                                        |
| scimark_lu               | 167 ms                                                       | 97.5 ms: 1.71x faster                                        |
| richards                 | 75.1 ms                                                      | 44.5 ms: 1.69x faster                                        |
| pyflate                  | 733 ms                                                       | 441 ms: 1.66x faster                                         |
| scimark_sor              | 180 ms                                                       | 108 ms: 1.66x faster                                         |
| raytrace                 | 489 ms                                                       | 299 ms: 1.63x faster                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.38 ms: 1.62x faster                                        |
| hexiom                   | 9.42 ms                                                      | 5.91 ms: 1.59x faster                                        |
| scimark_monte_carlo      | 107 ms                                                       | 67.7 ms: 1.59x faster                                        |
| nbody                    | 134 ms                                                       | 85.5 ms: 1.57x faster                                        |
| generators               | 57.3 ms                                                      | 37.1 ms: 1.55x faster                                        |
| async_tree_none          | 692 ms                                                       | 450 ms: 1.54x faster                                         |
| async_tree_io            | 1.60 sec                                                     | 1.04 sec: 1.53x faster                                       |
| unpickle_pure_python     | 312 us                                                       | 205 us: 1.52x faster                                         |
| crypto_pyaes             | 119 ms                                                       | 78.7 ms: 1.51x faster                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.78 ms: 1.51x faster                                        |
| async_tree_memoization   | 819 ms                                                       | 544 ms: 1.51x faster                                         |
| spectral_norm            | 139 ms                                                       | 92.6 ms: 1.50x faster                                        |
| mako                     | 14.7 ms                                                      | 10.1 ms: 1.46x faster                                        |
| float                    | 111 ms                                                       | 77.0 ms: 1.44x faster                                        |
| pickle_pure_python       | 455 us                                                       | 320 us: 1.42x faster                                         |
| json_dumps               | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                        |
| fannkuch                 | 483 ms                                                       | 348 ms: 1.39x faster                                         |
| pycparser                | 1.67 sec                                                     | 1.22 sec: 1.37x faster                                       |
| regex_compile            | 190 ms                                                       | 138 ms: 1.37x faster                                         |
| logging_simple           | 8.88 us                                                      | 6.49 us: 1.37x faster                                        |
| tomli_loads              | 2.92 sec                                                     | 2.14 sec: 1.36x faster                                       |
| logging_format           | 9.64 us                                                      | 7.11 us: 1.36x faster                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 693 ms: 1.35x faster                                         |
| bench_mp_pool            | 6.37 ms                                                      | 4.75 ms: 1.34x faster                                        |
| django_template          | 50.2 ms                                                      | 37.5 ms: 1.34x faster                                        |
| coroutines               | 30.3 ms                                                      | 22.7 ms: 1.34x faster                                        |
| deepcopy_memo            | 49.8 us                                                      | 37.4 us: 1.33x faster                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 791 ms: 1.33x faster                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.62 sec: 1.33x faster                                       |
| tornado_http             | 157 ms                                                       | 118 ms: 1.32x faster                                         |
| xml_etree_process        | 75.9 ms                                                      | 58.0 ms: 1.31x faster                                        |
| mypy2                    | 933 ms                                                       | 720 ms: 1.30x faster                                         |
| chameleon                | 9.44 ms                                                      | 7.31 ms: 1.29x faster                                        |
| comprehensions           | 26.7 us                                                      | 20.8 us: 1.28x faster                                        |
| nqueens                  | 115 ms                                                       | 90.0 ms: 1.28x faster                                        |
| deepcopy                 | 468 us                                                       | 368 us: 1.27x faster                                         |
| dulwich_log              | 81.1 ms                                                      | 64.2 ms: 1.26x faster                                        |
| sympy_expand             | 600 ms                                                       | 479 ms: 1.25x faster                                         |
| 2to3                     | 350 ms                                                       | 281 ms: 1.25x faster                                         |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                         |
| json_loads               | 30.3 us                                                      | 24.6 us: 1.23x faster                                        |
| sympy_sum                | 193 ms                                                       | 158 ms: 1.22x faster                                         |
| unpack_sequence          | 59.9 ns                                                      | 49.1 ns: 1.22x faster                                        |
| sqlalchemy_imperative    | 22.7 ms                                                      | 18.6 ms: 1.22x faster                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 57.6 ms: 1.22x faster                                        |
| scimark_fft              | 361 ms                                                       | 297 ms: 1.22x faster                                         |
| sympy_str                | 360 ms                                                       | 297 ms: 1.21x faster                                         |
| docutils                 | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                       |
| dask                     | 472 ms                                                       | 390 ms: 1.21x faster                                         |
| sympy_integrate          | 28.2 ms                                                      | 23.3 ms: 1.21x faster                                        |
| bench_thread_pool        | 1.14 ms                                                      | 945 us: 1.21x faster                                         |
| mdp                      | 3.01 sec                                                     | 2.52 sec: 1.19x faster                                       |
| sqlalchemy_declarative   | 190 ms                                                       | 160 ms: 1.19x faster                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.38 us: 1.19x faster                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.31 ms: 1.18x faster                                        |
| aiohttp                  | 1.19 ms                                                      | 1.02 ms: 1.17x faster                                        |
| gunicorn                 | 1.16 ms                                                      | 992 us: 1.17x faster                                         |
| regex_v8                 | 27.2 ms                                                      | 23.5 ms: 1.15x faster                                        |
| pathlib                  | 21.4 ms                                                      | 18.9 ms: 1.13x faster                                        |
| json                     | 5.86 ms                                                      | 5.19 ms: 1.13x faster                                        |
| sqlite_synth             | 2.99 us                                                      | 2.69 us: 1.11x faster                                        |
| async_generators         | 421 ms                                                       | 379 ms: 1.11x faster                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.60 ms: 1.10x faster                                        |
| xml_etree_parse          | 160 ms                                                       | 145 ms: 1.10x faster                                         |
| xml_etree_generate       | 92.3 ms                                                      | 84.6 ms: 1.09x faster                                        |
| xml_etree_iterparse      | 110 ms                                                       | 102 ms: 1.09x faster                                         |
| regex_dna                | 261 ms                                                       | 244 ms: 1.07x faster                                         |
| meteor_contest           | 138 ms                                                       | 131 ms: 1.06x faster                                         |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                         |
| python_startup           | 11.5 ms                                                      | 11.5 ms: 1.00x slower                                        |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.02x slower                                        |
| telco                    | 7.23 ms                                                      | 7.47 ms: 1.03x slower                                        |
| unpickle_list            | 4.65 us                                                      | 4.82 us: 1.04x slower                                        |
| pickle_dict              | 29.5 us                                                      | 31.2 us: 1.06x slower                                        |
| coverage                 | 63.3 ms                                                      | 67.6 ms: 1.07x slower                                        |
| pickle_list              | 4.12 us                                                      | 4.46 us: 1.08x slower                                        |
| unpickle                 | 13.5 us                                                      | 15.2 us: 1.13x slower                                        |
| regex_effbot             | 3.09 ms                                                      | 3.54 ms: 1.15x slower                                        |
| python_startup_no_site   | 7.33 ms                                                      | 8.53 ms: 1.16x slower                                        |
| gc_traversal             | 3.42 ms                                                      | 4.10 ms: 1.20x slower                                        |
| Geometric mean           | (ref)                                                        | 1.31x faster                                                 |

Benchmark hidden because not significant (1): asyncio_websockets
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20231207-3.12.1-2305ca5/bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.10x