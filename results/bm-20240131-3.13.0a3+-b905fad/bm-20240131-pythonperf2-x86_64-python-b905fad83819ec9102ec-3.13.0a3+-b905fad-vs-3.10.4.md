
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 291 ms: 1.20x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.28 ms: 1.30x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.85 sec: 1.20x faster                                                       |
| tornado_http   | 157 ms                                                       | 121 ms: 1.29x faster                                                         |
| Geometric mean | (ref)                                                        | 1.25x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 428 ms: 1.61x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 541 ms: 1.51x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 693 ms: 1.35x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.49x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 85.6 ms: 1.57x faster                                                        |
| float          | 111 ms                                                       | 79.6 ms: 1.40x faster                                                        |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.31x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 139 ms: 1.36x faster                                                         |
| regex_dna      | 261 ms                                                       | 238 ms: 1.10x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 25.8 ms: 1.05x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.67 ms: 1.19x slower                                                        |
| Geometric mean | (ref)                                                        | 1.07x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 303 us: 1.50x faster                                                         |
| unpickle_pure_python | 312 us                                                       | 209 us: 1.49x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.23 sec: 1.30x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 58.8 ms: 1.29x faster                                                        |
| json_loads           | 30.3 us                                                      | 24.9 us: 1.22x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 84.4 ms: 1.09x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 109 ms: 1.01x faster                                                         |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 30.8 us: 1.05x slower                                                        |
| unpickle_list        | 4.65 us                                                      | 4.89 us: 1.05x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| unpickle             | 13.5 us                                                      | 15.4 us: 1.14x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.4 ms: 1.41x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 117 us: 4.59x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 366 ms: 2.13x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.58 ms: 2.10x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 258 ms: 1.89x faster                                                         |
| chaos                    | 109 ms                                                       | 59.0 ms: 1.84x faster                                                        |
| logging_silent           | 167 ns                                                       | 94.1 ns: 1.78x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 69.8 ms: 1.71x faster                                                        |
| generators               | 57.3 ms                                                      | 33.8 ms: 1.69x faster                                                        |
| scimark_lu               | 167 ms                                                       | 98.6 ms: 1.69x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 65.6 ms: 1.64x faster                                                        |
| comprehensions           | 26.7 us                                                      | 16.4 us: 1.63x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.38 ms: 1.62x faster                                                        |
| async_tree_none          | 692 ms                                                       | 428 ms: 1.61x faster                                                         |
| go                       | 262 ms                                                       | 166 ms: 1.57x faster                                                         |
| richards_super           | 90.6 ms                                                      | 57.6 ms: 1.57x faster                                                        |
| nbody                    | 134 ms                                                       | 85.6 ms: 1.57x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 541 ms: 1.51x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                                       |
| pickle_pure_python       | 455 us                                                       | 303 us: 1.50x faster                                                         |
| spectral_norm            | 139 ms                                                       | 92.6 ms: 1.50x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.79 ms: 1.50x faster                                                        |
| hexiom                   | 9.42 ms                                                      | 6.31 ms: 1.49x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 209 us: 1.49x faster                                                         |
| pyflate                  | 733 ms                                                       | 502 ms: 1.46x faster                                                         |
| richards                 | 75.1 ms                                                      | 51.6 ms: 1.45x faster                                                        |
| mako                     | 14.7 ms                                                      | 10.4 ms: 1.41x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.56 ms: 1.40x faster                                                        |
| float                    | 111 ms                                                       | 79.6 ms: 1.40x faster                                                        |
| coroutines               | 30.3 ms                                                      | 21.8 ms: 1.39x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                        |
| regex_compile            | 190 ms                                                       | 139 ms: 1.36x faster                                                         |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 693 ms: 1.35x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.59 us: 1.35x faster                                                        |
| deepcopy_memo            | 49.8 us                                                      | 37.2 us: 1.34x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.23 us: 1.33x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.26 sec: 1.33x faster                                                       |
| nqueens                  | 115 ms                                                       | 87.5 ms: 1.31x faster                                                        |
| tomli_loads              | 2.92 sec                                                     | 2.23 sec: 1.30x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 805 ms: 1.30x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.66 sec: 1.30x faster                                                       |
| chameleon                | 9.44 ms                                                      | 7.28 ms: 1.30x faster                                                        |
| tornado_http             | 157 ms                                                       | 121 ms: 1.29x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 58.8 ms: 1.29x faster                                                        |
| scimark_sor              | 180 ms                                                       | 141 ms: 1.28x faster                                                         |
| deepcopy                 | 468 us                                                       | 367 us: 1.27x faster                                                         |
| sympy_sum                | 193 ms                                                       | 151 ms: 1.27x faster                                                         |
| fannkuch                 | 483 ms                                                       | 385 ms: 1.25x faster                                                         |
| sympy_str                | 360 ms                                                       | 289 ms: 1.25x faster                                                         |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.12 ms: 1.23x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 48.8 ns: 1.23x faster                                                        |
| json_loads               | 30.3 us                                                      | 24.9 us: 1.22x faster                                                        |
| sympy_integrate          | 28.2 ms                                                      | 23.2 ms: 1.22x faster                                                        |
| sympy_expand             | 600 ms                                                       | 494 ms: 1.22x faster                                                         |
| scimark_fft              | 361 ms                                                       | 298 ms: 1.21x faster                                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.32 us: 1.21x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 67.2 ms: 1.21x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.49 sec: 1.21x faster                                                       |
| 2to3                     | 350 ms                                                       | 291 ms: 1.20x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 58.4 ms: 1.20x faster                                                        |
| docutils                 | 3.41 sec                                                     | 2.85 sec: 1.20x faster                                                       |
| dask                     | 472 ms                                                       | 397 ms: 1.19x faster                                                         |
| async_generators         | 421 ms                                                       | 360 ms: 1.17x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 975 us: 1.17x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 18.7 ms: 1.14x faster                                                        |
| json                     | 5.86 ms                                                      | 5.16 ms: 1.14x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.72 us: 1.10x faster                                                        |
| regex_dna                | 261 ms                                                       | 238 ms: 1.10x faster                                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.61 ms: 1.10x faster                                                        |
| xml_etree_generate       | 92.3 ms                                                      | 84.4 ms: 1.09x faster                                                        |
| meteor_contest           | 138 ms                                                       | 127 ms: 1.09x faster                                                         |
| mypy2                    | 933 ms                                                       | 859 ms: 1.09x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 25.8 ms: 1.05x faster                                                        |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 109 ms: 1.01x faster                                                         |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.51 ms: 1.03x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 30.8 us: 1.05x slower                                                        |
| unpickle_list            | 4.65 us                                                      | 4.89 us: 1.05x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.02 ms: 1.11x slower                                                        |
| unpickle                 | 13.5 us                                                      | 15.4 us: 1.14x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.67 ms: 1.19x slower                                                        |
| coverage                 | 63.3 ms                                                      | 78.7 ms: 1.24x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.30x faster                                                                 |

Benchmark hidden because not significant (1): asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.06x