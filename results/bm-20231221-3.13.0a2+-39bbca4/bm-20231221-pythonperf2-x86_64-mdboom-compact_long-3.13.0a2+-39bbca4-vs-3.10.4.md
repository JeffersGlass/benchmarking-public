
# Results vs. 3.10.4

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 294 ms: 1.19x faster                                                 |
| chameleon      | 9.44 ms                                                      | 7.36 ms: 1.28x faster                                                |
| docutils       | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                               |
| tornado_http   | 157 ms                                                       | 118 ms: 1.32x faster                                                 |
| Geometric mean | (ref)                                                        | 1.25x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 437 ms: 1.58x faster                                                 |
| async_tree_memoization  | 819 ms                                                       | 547 ms: 1.50x faster                                                 |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                               |
| async_tree_cpu_io_mixed | 936 ms                                                       | 713 ms: 1.31x faster                                                 |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 84.3 ms: 1.59x faster                                                |
| float          | 111 ms                                                       | 76.8 ms: 1.45x faster                                                |
| pidigits       | 271 ms                                                       | 267 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                        | 1.33x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.31x faster                                                 |
| regex_v8       | 27.2 ms                                                      | 24.7 ms: 1.10x faster                                                |
| regex_dna      | 261 ms                                                       | 240 ms: 1.09x faster                                                 |
| regex_effbot   | 3.09 ms                                                      | 3.44 ms: 1.11x slower                                                |
| Geometric mean | (ref)                                                        | 1.09x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 211 us: 1.48x faster                                                 |
| pickle_pure_python   | 455 us                                                       | 308 us: 1.48x faster                                                 |
| json_dumps           | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                |
| xml_etree_process    | 75.9 ms                                                      | 58.7 ms: 1.29x faster                                                |
| tomli_loads          | 2.92 sec                                                     | 2.35 sec: 1.24x faster                                               |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.20x faster                                                |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                 |
| xml_etree_generate   | 92.3 ms                                                      | 85.0 ms: 1.09x faster                                                |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.06x faster                                                 |
| unpickle_list        | 4.65 us                                                      | 4.54 us: 1.02x faster                                                |
| pickle               | 9.89 us                                                      | 9.98 us: 1.01x slower                                                |
| pickle_list          | 4.12 us                                                      | 4.34 us: 1.05x slower                                                |
| pickle_dict          | 29.5 us                                                      | 31.6 us: 1.07x slower                                                |
| unpickle             | 13.5 us                                                      | 14.6 us: 1.08x slower                                                |
| Geometric mean       | (ref)                                                        | 1.14x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.8 ms: 1.11x slower                                                |
| python_startup_no_site | 7.33 ms                                                      | 11.3 ms: 1.54x slower                                                |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.3 ms: 1.43x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 122 us: 4.39x faster                                                 |
| asyncio_tcp              | 779 ms                                                       | 369 ms: 2.11x faster                                                 |
| deltablue                | 7.50 ms                                                      | 3.64 ms: 2.06x faster                                                |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                               |
| raytrace                 | 489 ms                                                       | 270 ms: 1.81x faster                                                 |
| chaos                    | 109 ms                                                       | 60.2 ms: 1.80x faster                                                |
| logging_silent           | 167 ns                                                       | 95.6 ns: 1.75x faster                                                |
| scimark_lu               | 167 ms                                                       | 99.5 ms: 1.68x faster                                                |
| scimark_monte_carlo      | 107 ms                                                       | 65.0 ms: 1.65x faster                                                |
| generators               | 57.3 ms                                                      | 34.8 ms: 1.65x faster                                                |
| sqlglot_parse            | 2.24 ms                                                      | 1.39 ms: 1.61x faster                                                |
| comprehensions           | 26.7 us                                                      | 16.6 us: 1.61x faster                                                |
| nbody                    | 134 ms                                                       | 84.3 ms: 1.59x faster                                                |
| crypto_pyaes             | 119 ms                                                       | 74.9 ms: 1.59x faster                                                |
| async_tree_none          | 692 ms                                                       | 437 ms: 1.58x faster                                                 |
| go                       | 262 ms                                                       | 169 ms: 1.55x faster                                                 |
| spectral_norm            | 139 ms                                                       | 91.5 ms: 1.52x faster                                                |
| richards_super           | 90.6 ms                                                      | 60.3 ms: 1.50x faster                                                |
| async_tree_memoization   | 819 ms                                                       | 547 ms: 1.50x faster                                                 |
| sqlglot_transpile        | 2.68 ms                                                      | 1.79 ms: 1.50x faster                                                |
| unpickle_pure_python     | 312 us                                                       | 211 us: 1.48x faster                                                 |
| pickle_pure_python       | 455 us                                                       | 308 us: 1.48x faster                                                 |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                               |
| hexiom                   | 9.42 ms                                                      | 6.41 ms: 1.47x faster                                                |
| float                    | 111 ms                                                       | 76.8 ms: 1.45x faster                                                |
| pyflate                  | 733 ms                                                       | 507 ms: 1.45x faster                                                 |
| mako                     | 14.7 ms                                                      | 10.3 ms: 1.43x faster                                                |
| bench_mp_pool            | 6.37 ms                                                      | 4.48 ms: 1.42x faster                                                |
| coroutines               | 30.3 ms                                                      | 22.0 ms: 1.38x faster                                                |
| richards                 | 75.1 ms                                                      | 54.6 ms: 1.37x faster                                                |
| json_dumps               | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                |
| logging_simple           | 8.88 us                                                      | 6.54 us: 1.36x faster                                                |
| deepcopy_memo            | 49.8 us                                                      | 37.3 us: 1.33x faster                                                |
| logging_format           | 9.64 us                                                      | 7.27 us: 1.33x faster                                                |
| tornado_http             | 157 ms                                                       | 118 ms: 1.32x faster                                                 |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 713 ms: 1.31x faster                                                 |
| pprint_pformat           | 2.15 sec                                                     | 1.64 sec: 1.31x faster                                               |
| nqueens                  | 115 ms                                                       | 87.9 ms: 1.31x faster                                                |
| pprint_safe_repr         | 1.05 sec                                                     | 804 ms: 1.31x faster                                                 |
| regex_compile            | 190 ms                                                       | 146 ms: 1.31x faster                                                 |
| xml_etree_process        | 75.9 ms                                                      | 58.7 ms: 1.29x faster                                                |
| chameleon                | 9.44 ms                                                      | 7.36 ms: 1.28x faster                                                |
| sympy_sum                | 193 ms                                                       | 150 ms: 1.28x faster                                                 |
| deepcopy                 | 468 us                                                       | 368 us: 1.27x faster                                                 |
| fannkuch                 | 483 ms                                                       | 380 ms: 1.27x faster                                                 |
| pycparser                | 1.67 sec                                                     | 1.32 sec: 1.27x faster                                               |
| scimark_sor              | 180 ms                                                       | 144 ms: 1.25x faster                                                 |
| sqlglot_normalize        | 144 ms                                                       | 115 ms: 1.25x faster                                                 |
| tomli_loads              | 2.92 sec                                                     | 2.35 sec: 1.24x faster                                               |
| sympy_str                | 360 ms                                                       | 291 ms: 1.24x faster                                                 |
| sympy_integrate          | 28.2 ms                                                      | 23.0 ms: 1.22x faster                                                |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.16 ms: 1.22x faster                                                |
| sqlglot_optimize         | 70.1 ms                                                      | 57.7 ms: 1.22x faster                                                |
| sympy_expand             | 600 ms                                                       | 496 ms: 1.21x faster                                                 |
| bench_thread_pool        | 1.14 ms                                                      | 945 us: 1.21x faster                                                 |
| scimark_fft              | 361 ms                                                       | 299 ms: 1.21x faster                                                 |
| docutils                 | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                               |
| json_loads               | 30.3 us                                                      | 25.2 us: 1.20x faster                                                |
| deepcopy_reduce          | 4.01 us                                                      | 3.33 us: 1.20x faster                                                |
| dulwich_log              | 81.1 ms                                                      | 68.0 ms: 1.19x faster                                                |
| 2to3                     | 350 ms                                                       | 294 ms: 1.19x faster                                                 |
| mdp                      | 3.01 sec                                                     | 2.53 sec: 1.19x faster                                               |
| async_generators         | 421 ms                                                       | 362 ms: 1.16x faster                                                 |
| unpack_sequence          | 59.9 ns                                                      | 51.7 ns: 1.16x faster                                                |
| sqlite_synth             | 2.99 us                                                      | 2.68 us: 1.11x faster                                                |
| json                     | 5.86 ms                                                      | 5.27 ms: 1.11x faster                                                |
| pathlib                  | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                                |
| create_gc_cycles         | 1.76 ms                                                      | 1.59 ms: 1.11x faster                                                |
| regex_v8                 | 27.2 ms                                                      | 24.7 ms: 1.10x faster                                                |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                 |
| regex_dna                | 261 ms                                                       | 240 ms: 1.09x faster                                                 |
| mypy2                    | 933 ms                                                       | 858 ms: 1.09x faster                                                 |
| xml_etree_generate       | 92.3 ms                                                      | 85.0 ms: 1.09x faster                                                |
| meteor_contest           | 138 ms                                                       | 130 ms: 1.06x faster                                                 |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.06x faster                                                 |
| unpickle_list            | 4.65 us                                                      | 4.54 us: 1.02x faster                                                |
| pidigits                 | 271 ms                                                       | 267 ms: 1.01x faster                                                 |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                 |
| pickle                   | 9.89 us                                                      | 9.98 us: 1.01x slower                                                |
| gc_traversal             | 3.42 ms                                                      | 3.57 ms: 1.05x slower                                                |
| pickle_list              | 4.12 us                                                      | 4.34 us: 1.05x slower                                                |
| pickle_dict              | 29.5 us                                                      | 31.6 us: 1.07x slower                                                |
| unpickle                 | 13.5 us                                                      | 14.6 us: 1.08x slower                                                |
| regex_effbot             | 3.09 ms                                                      | 3.44 ms: 1.11x slower                                                |
| python_startup           | 11.5 ms                                                      | 12.8 ms: 1.11x slower                                                |
| telco                    | 7.23 ms                                                      | 8.11 ms: 1.12x slower                                                |
| coverage                 | 63.3 ms                                                      | 79.4 ms: 1.25x slower                                                |
| python_startup_no_site   | 7.33 ms                                                      | 11.3 ms: 1.54x slower                                                |
| Geometric mean           | (ref)                                                        | 1.29x faster                                                         |
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231221-3.13.0a2+-39bbca4/bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.06x