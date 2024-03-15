
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 299 ms: 1.17x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.69 ms: 1.23x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.89 sec: 1.18x faster                                                       |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                                         |
| Geometric mean | (ref)                                                        | 1.21x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 438 ms: 1.58x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 550 ms: 1.49x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 700 ms: 1.34x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 81.7 ms: 1.36x faster                                                        |
| nbody          | 134 ms                                                       | 107 ms: 1.26x faster                                                         |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.21x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 147 ms: 1.29x faster                                                         |
| regex_dna      | 261 ms                                                       | 232 ms: 1.12x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 24.4 ms: 1.11x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                                        |
| Geometric mean | (ref)                                                        | 1.10x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 308 us: 1.48x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 232 us: 1.35x faster                                                         |
| xml_etree_process    | 75.9 ms                                                      | 59.6 ms: 1.27x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.35 sec: 1.24x faster                                                       |
| json_loads           | 30.3 us                                                      | 25.1 us: 1.21x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 86.6 ms: 1.07x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.04x faster                                                         |
| unpickle_list        | 4.65 us                                                      | 4.77 us: 1.03x slower                                                        |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 32.8 us: 1.11x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.62 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 12.0 ms: 1.22x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 119 us: 4.51x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 372 ms: 2.10x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                       |
| deltablue                | 7.50 ms                                                      | 4.03 ms: 1.86x faster                                                        |
| logging_silent           | 167 ns                                                       | 94.9 ns: 1.76x faster                                                        |
| raytrace                 | 489 ms                                                       | 281 ms: 1.74x faster                                                         |
| scimark_lu               | 167 ms                                                       | 101 ms: 1.65x faster                                                         |
| generators               | 57.3 ms                                                      | 35.6 ms: 1.61x faster                                                        |
| richards_super           | 90.6 ms                                                      | 56.9 ms: 1.59x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.41 ms: 1.59x faster                                                        |
| async_tree_none          | 692 ms                                                       | 438 ms: 1.58x faster                                                         |
| go                       | 262 ms                                                       | 169 ms: 1.55x faster                                                         |
| chaos                    | 109 ms                                                       | 71.6 ms: 1.52x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 550 ms: 1.49x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| richards                 | 75.1 ms                                                      | 50.8 ms: 1.48x faster                                                        |
| pickle_pure_python       | 455 us                                                       | 308 us: 1.48x faster                                                         |
| crypto_pyaes             | 119 ms                                                       | 81.5 ms: 1.46x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.84 ms: 1.46x faster                                                        |
| pyflate                  | 733 ms                                                       | 520 ms: 1.41x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 79.0 ms: 1.36x faster                                                        |
| float                    | 111 ms                                                       | 81.7 ms: 1.36x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.5 ms: 1.35x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 232 us: 1.35x faster                                                         |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 700 ms: 1.34x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.70 us: 1.32x faster                                                        |
| deepcopy_memo            | 49.8 us                                                      | 37.6 us: 1.32x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 45.9 ns: 1.31x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.28 sec: 1.30x faster                                                       |
| regex_compile            | 190 ms                                                       | 147 ms: 1.29x faster                                                         |
| comprehensions           | 26.7 us                                                      | 20.7 us: 1.29x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 59.6 ms: 1.27x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.58 us: 1.27x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 5.02 ms: 1.27x faster                                                        |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                                         |
| nbody                    | 134 ms                                                       | 107 ms: 1.26x faster                                                         |
| scimark_sor              | 180 ms                                                       | 144 ms: 1.25x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.35 sec: 1.24x faster                                                       |
| deepcopy                 | 468 us                                                       | 378 us: 1.24x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.69 ms: 1.23x faster                                                        |
| mako                     | 14.7 ms                                                      | 12.0 ms: 1.22x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 119 ms: 1.21x faster                                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 865 ms: 1.21x faster                                                         |
| sympy_sum                | 193 ms                                                       | 159 ms: 1.21x faster                                                         |
| json_loads               | 30.3 us                                                      | 25.1 us: 1.21x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.33 us: 1.20x faster                                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.79 sec: 1.20x faster                                                       |
| sympy_str                | 360 ms                                                       | 300 ms: 1.20x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 7.86 ms: 1.20x faster                                                        |
| spectral_norm            | 139 ms                                                       | 116 ms: 1.20x faster                                                         |
| sympy_expand             | 600 ms                                                       | 505 ms: 1.19x faster                                                         |
| nqueens                  | 115 ms                                                       | 96.9 ms: 1.19x faster                                                        |
| docutils                 | 3.41 sec                                                     | 2.89 sec: 1.18x faster                                                       |
| dulwich_log              | 81.1 ms                                                      | 68.7 ms: 1.18x faster                                                        |
| 2to3                     | 350 ms                                                       | 299 ms: 1.17x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 979 us: 1.17x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.58 sec: 1.16x faster                                                       |
| dask                     | 472 ms                                                       | 406 ms: 1.16x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 24.2 ms: 1.16x faster                                                        |
| fannkuch                 | 483 ms                                                       | 415 ms: 1.16x faster                                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.54 ms: 1.15x faster                                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 61.5 ms: 1.14x faster                                                        |
| async_generators         | 421 ms                                                       | 374 ms: 1.13x faster                                                         |
| regex_dna                | 261 ms                                                       | 232 ms: 1.12x faster                                                         |
| json                     | 5.86 ms                                                      | 5.24 ms: 1.12x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                                        |
| regex_v8                 | 27.2 ms                                                      | 24.4 ms: 1.11x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.72 us: 1.10x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 86.6 ms: 1.07x faster                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 106 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| meteor_contest           | 138 ms                                                       | 134 ms: 1.03x faster                                                         |
| scimark_fft              | 361 ms                                                       | 365 ms: 1.01x slower                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.14 ms: 1.01x slower                                                        |
| unpickle_list            | 4.65 us                                                      | 4.77 us: 1.03x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.65 ms: 1.07x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 32.8 us: 1.11x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.62 us: 1.12x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.34 ms: 1.15x slower                                                        |
| coverage                 | 63.3 ms                                                      | 86.7 ms: 1.37x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.24x faster                                                                 |

Benchmark hidden because not significant (2): mypy2, asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.11x