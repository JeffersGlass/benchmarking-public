
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 302 ms: 1.16x faster                                                 |
| chameleon      | 9.44 ms                                                      | 7.78 ms: 1.21x faster                                                |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                               |
| tornado_http   | 157 ms                                                       | 121 ms: 1.29x faster                                                 |
| Geometric mean | (ref)                                                        | 1.21x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 447 ms: 1.55x faster                                                 |
| async_tree_memoization  | 819 ms                                                       | 559 ms: 1.47x faster                                                 |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                               |
| async_tree_cpu_io_mixed | 936 ms                                                       | 711 ms: 1.32x faster                                                 |
| Geometric mean          | (ref)                                                        | 1.44x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 111 ms                                                       | 82.2 ms: 1.35x faster                                                |
| nbody          | 134 ms                                                       | 108 ms: 1.24x faster                                                 |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                 |
| Geometric mean | (ref)                                                        | 1.20x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 150 ms: 1.27x faster                                                 |
| regex_v8       | 27.2 ms                                                      | 25.3 ms: 1.07x faster                                                |
| regex_dna      | 261 ms                                                       | 244 ms: 1.07x faster                                                 |
| regex_effbot   | 3.09 ms                                                      | 3.60 ms: 1.17x slower                                                |
| Geometric mean | (ref)                                                        | 1.06x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 313 us: 1.45x faster                                                 |
| unpickle_pure_python | 312 us                                                       | 221 us: 1.41x faster                                                 |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                |
| xml_etree_process    | 75.9 ms                                                      | 59.5 ms: 1.28x faster                                                |
| json_loads           | 30.3 us                                                      | 24.5 us: 1.24x faster                                                |
| tomli_loads          | 2.92 sec                                                     | 2.36 sec: 1.24x faster                                               |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                 |
| xml_etree_generate   | 92.3 ms                                                      | 88.0 ms: 1.05x faster                                                |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.03x faster                                                 |
| unpickle_list        | 4.65 us                                                      | 4.71 us: 1.01x slower                                                |
| pickle_list          | 4.12 us                                                      | 4.23 us: 1.03x slower                                                |
| unpickle             | 13.5 us                                                      | 14.8 us: 1.09x slower                                                |
| pickle_dict          | 29.5 us                                                      | 32.4 us: 1.10x slower                                                |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                         |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 12.0 ms: 1.22x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 120 us: 4.46x faster                                                 |
| asyncio_tcp              | 779 ms                                                       | 369 ms: 2.11x faster                                                 |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.96x faster                                               |
| deltablue                | 7.50 ms                                                      | 4.06 ms: 1.85x faster                                                |
| raytrace                 | 489 ms                                                       | 277 ms: 1.77x faster                                                 |
| logging_silent           | 167 ns                                                       | 99.2 ns: 1.69x faster                                                |
| generators               | 57.3 ms                                                      | 34.9 ms: 1.64x faster                                                |
| scimark_lu               | 167 ms                                                       | 103 ms: 1.62x faster                                                 |
| sqlglot_parse            | 2.24 ms                                                      | 1.41 ms: 1.59x faster                                                |
| richards_super           | 90.6 ms                                                      | 57.8 ms: 1.57x faster                                                |
| async_tree_none          | 692 ms                                                       | 447 ms: 1.55x faster                                                 |
| chaos                    | 109 ms                                                       | 71.2 ms: 1.53x faster                                                |
| go                       | 262 ms                                                       | 174 ms: 1.50x faster                                                 |
| sqlglot_transpile        | 2.68 ms                                                      | 1.82 ms: 1.47x faster                                                |
| async_tree_memoization   | 819 ms                                                       | 559 ms: 1.47x faster                                                 |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                               |
| pickle_pure_python       | 455 us                                                       | 313 us: 1.45x faster                                                 |
| richards                 | 75.1 ms                                                      | 51.7 ms: 1.45x faster                                                |
| crypto_pyaes             | 119 ms                                                       | 83.6 ms: 1.43x faster                                                |
| pyflate                  | 733 ms                                                       | 517 ms: 1.42x faster                                                 |
| unpickle_pure_python     | 312 us                                                       | 221 us: 1.41x faster                                                 |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                |
| unpack_sequence          | 59.9 ns                                                      | 44.0 ns: 1.36x faster                                                |
| scimark_monte_carlo      | 107 ms                                                       | 79.1 ms: 1.36x faster                                                |
| float                    | 111 ms                                                       | 82.2 ms: 1.35x faster                                                |
| coroutines               | 30.3 ms                                                      | 22.5 ms: 1.34x faster                                                |
| logging_simple           | 8.88 us                                                      | 6.61 us: 1.34x faster                                                |
| deepcopy_memo            | 49.8 us                                                      | 37.4 us: 1.33x faster                                                |
| logging_format           | 9.64 us                                                      | 7.24 us: 1.33x faster                                                |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 711 ms: 1.32x faster                                                 |
| pycparser                | 1.67 sec                                                     | 1.28 sec: 1.31x faster                                               |
| bench_mp_pool            | 6.37 ms                                                      | 4.90 ms: 1.30x faster                                                |
| tornado_http             | 157 ms                                                       | 121 ms: 1.29x faster                                                 |
| xml_etree_process        | 75.9 ms                                                      | 59.5 ms: 1.28x faster                                                |
| regex_compile            | 190 ms                                                       | 150 ms: 1.27x faster                                                 |
| comprehensions           | 26.7 us                                                      | 21.0 us: 1.27x faster                                                |
| deepcopy                 | 468 us                                                       | 371 us: 1.26x faster                                                 |
| scimark_sor              | 180 ms                                                       | 144 ms: 1.25x faster                                                 |
| nbody                    | 134 ms                                                       | 108 ms: 1.24x faster                                                 |
| json_loads               | 30.3 us                                                      | 24.5 us: 1.24x faster                                                |
| tomli_loads              | 2.92 sec                                                     | 2.36 sec: 1.24x faster                                               |
| mako                     | 14.7 ms                                                      | 12.0 ms: 1.22x faster                                                |
| pprint_safe_repr         | 1.05 sec                                                     | 861 ms: 1.22x faster                                                 |
| pprint_pformat           | 2.15 sec                                                     | 1.77 sec: 1.22x faster                                               |
| chameleon                | 9.44 ms                                                      | 7.78 ms: 1.21x faster                                                |
| sympy_sum                | 193 ms                                                       | 161 ms: 1.20x faster                                                 |
| sqlglot_normalize        | 144 ms                                                       | 120 ms: 1.20x faster                                                 |
| bench_thread_pool        | 1.14 ms                                                      | 958 us: 1.19x faster                                                 |
| dulwich_log              | 81.1 ms                                                      | 68.2 ms: 1.19x faster                                                |
| deepcopy_reduce          | 4.01 us                                                      | 3.37 us: 1.19x faster                                                |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                               |
| sympy_str                | 360 ms                                                       | 304 ms: 1.18x faster                                                 |
| hexiom                   | 9.42 ms                                                      | 7.96 ms: 1.18x faster                                                |
| sympy_expand             | 600 ms                                                       | 509 ms: 1.18x faster                                                 |
| dask                     | 472 ms                                                       | 406 ms: 1.16x faster                                                 |
| 2to3                     | 350 ms                                                       | 302 ms: 1.16x faster                                                 |
| sympy_integrate          | 28.2 ms                                                      | 24.4 ms: 1.15x faster                                                |
| mdp                      | 3.01 sec                                                     | 2.62 sec: 1.15x faster                                               |
| spectral_norm            | 139 ms                                                       | 121 ms: 1.15x faster                                                 |
| sqlglot_optimize         | 70.1 ms                                                      | 62.0 ms: 1.13x faster                                                |
| create_gc_cycles         | 1.76 ms                                                      | 1.56 ms: 1.13x faster                                                |
| nqueens                  | 115 ms                                                       | 102 ms: 1.12x faster                                                 |
| json                     | 5.86 ms                                                      | 5.25 ms: 1.12x faster                                                |
| pathlib                  | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                                |
| async_generators         | 421 ms                                                       | 380 ms: 1.11x faster                                                 |
| fannkuch                 | 483 ms                                                       | 439 ms: 1.10x faster                                                 |
| sqlite_synth             | 2.99 us                                                      | 2.73 us: 1.09x faster                                                |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                 |
| regex_v8                 | 27.2 ms                                                      | 25.3 ms: 1.07x faster                                                |
| regex_dna                | 261 ms                                                       | 244 ms: 1.07x faster                                                 |
| xml_etree_generate       | 92.3 ms                                                      | 88.0 ms: 1.05x faster                                                |
| meteor_contest           | 138 ms                                                       | 133 ms: 1.04x faster                                                 |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                 |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.03x faster                                                 |
| asyncio_websockets       | 390 ms                                                       | 385 ms: 1.01x faster                                                 |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.11 ms: 1.01x slower                                                |
| unpickle_list            | 4.65 us                                                      | 4.71 us: 1.01x slower                                                |
| scimark_fft              | 361 ms                                                       | 371 ms: 1.03x slower                                                 |
| pickle_list              | 4.12 us                                                      | 4.23 us: 1.03x slower                                                |
| unpickle                 | 13.5 us                                                      | 14.8 us: 1.09x slower                                                |
| pickle_dict              | 29.5 us                                                      | 32.4 us: 1.10x slower                                                |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                |
| telco                    | 7.23 ms                                                      | 8.25 ms: 1.14x slower                                                |
| regex_effbot             | 3.09 ms                                                      | 3.60 ms: 1.17x slower                                                |
| gc_traversal             | 3.42 ms                                                      | 4.10 ms: 1.20x slower                                                |
| coverage                 | 63.3 ms                                                      | 83.1 ms: 1.31x slower                                                |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                |
| Geometric mean           | (ref)                                                        | 1.24x faster                                                         |

Benchmark hidden because not significant (2): mypy2, pickle
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231219-3.13.0a2+-b63610e-JIT/bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.11x