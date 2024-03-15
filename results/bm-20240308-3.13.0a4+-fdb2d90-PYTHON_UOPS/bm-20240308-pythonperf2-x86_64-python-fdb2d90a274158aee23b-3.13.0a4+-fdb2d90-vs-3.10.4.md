# Results vs. 3.10.4

- fork: python
- ref: fdb2d90a274158aee23b
- machine: linux-x86_64
- commit hash: fdb2d90
- commit date: 2024-03-08
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 322 ms: 1.09x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.57 ms: 1.25x faster                                                        |
| docutils       | 3.41 sec                                                     | 3.07 sec: 1.11x faster                                                       |
| html5lib       | 94.6 ms                                                      | 78.5 ms: 1.21x faster                                                        |
| tornado_http   | 157 ms                                                       | 129 ms: 1.22x faster                                                         |
| Geometric mean | (ref)                                                        | 1.17x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 446 ms: 1.55x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 559 ms: 1.47x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 712 ms: 1.32x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.44x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 105 ms: 1.06x faster                                                         |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| nbody          | 134 ms                                                       | 132 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 261 ms                                                       | 249 ms: 1.05x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 26.4 ms: 1.03x faster                                                        |
| regex_compile  | 190 ms                                                       | 203 ms: 1.07x slower                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.58 ms: 1.16x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 315 us: 1.44x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.38x faster                                                        |
| json_loads           | 30.3 us                                                      | 24.8 us: 1.23x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 62.1 ms: 1.22x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 145 ms: 1.10x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 90.6 ms: 1.02x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.59 us: 1.01x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 309 us: 1.01x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 113 ms: 1.03x slower                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.99 sec: 1.03x slower                                                       |
| pickle_list          | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| pickle               | 9.89 us                                                      | 10.8 us: 1.09x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 32.8 us: 1.11x slower                                                        |
| unpickle             | 13.5 us                                                      | 15.0 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.8 ms: 1.11x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 50.2 ms                                                      | 39.6 ms: 1.27x faster                                                        |
| genshi_text     | 31.4 ms                                                      | 30.0 ms: 1.05x faster                                                        |
| mako            | 14.7 ms                                                      | 14.1 ms: 1.04x faster                                                        |
| genshi_xml      | 63.3 ms                                                      | 62.8 ms: 1.01x faster                                                        |
| Geometric mean  | (ref)                                                        | 1.09x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 123 us: 4.36x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 375 ms: 2.08x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                       |
| deltablue                | 7.50 ms                                                      | 4.10 ms: 1.83x faster                                                        |
| generators               | 57.3 ms                                                      | 34.1 ms: 1.68x faster                                                        |
| logging_silent           | 167 ns                                                       | 101 ns: 1.65x faster                                                         |
| async_tree_none          | 692 ms                                                       | 446 ms: 1.55x faster                                                         |
| pylint                   | 566 ms                                                       | 368 ms: 1.54x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 559 ms: 1.47x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                       |
| pickle_pure_python       | 455 us                                                       | 315 us: 1.44x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.55 ms: 1.44x faster                                                        |
| richards_super           | 90.6 ms                                                      | 64.6 ms: 1.40x faster                                                        |
| chaos                    | 109 ms                                                       | 77.6 ms: 1.40x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.38x faster                                                        |
| raytrace                 | 489 ms                                                       | 357 ms: 1.37x faster                                                         |
| thrift                   | 1.18 ms                                                      | 868 us: 1.35x faster                                                         |
| crypto_pyaes             | 119 ms                                                       | 88.4 ms: 1.35x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.99 ms: 1.35x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.6 ms: 1.34x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.80 ms: 1.33x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 712 ms: 1.32x faster                                                         |
| go                       | 262 ms                                                       | 200 ms: 1.31x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.87 us: 1.29x faster                                                        |
| richards                 | 75.1 ms                                                      | 58.4 ms: 1.29x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.51 us: 1.28x faster                                                        |
| django_template          | 50.2 ms                                                      | 39.6 ms: 1.27x faster                                                        |
| chameleon                | 9.44 ms                                                      | 7.57 ms: 1.25x faster                                                        |
| json_loads               | 30.3 us                                                      | 24.8 us: 1.23x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 62.1 ms: 1.22x faster                                                        |
| deepcopy                 | 468 us                                                       | 383 us: 1.22x faster                                                         |
| tornado_http             | 157 ms                                                       | 129 ms: 1.22x faster                                                         |
| html5lib                 | 94.6 ms                                                      | 78.5 ms: 1.21x faster                                                        |
| scimark_lu               | 167 ms                                                       | 140 ms: 1.19x faster                                                         |
| sqlglot_normalize        | 144 ms                                                       | 122 ms: 1.18x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 42.3 us: 1.18x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.42 us: 1.17x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.45 sec: 1.16x faster                                                       |
| bench_thread_pool        | 1.14 ms                                                      | 1.00 ms: 1.14x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.68 sec: 1.12x faster                                                       |
| scimark_sor              | 180 ms                                                       | 162 ms: 1.12x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 25.3 ms: 1.11x faster                                                        |
| docutils                 | 3.41 sec                                                     | 3.07 sec: 1.11x faster                                                       |
| sympy_sum                | 193 ms                                                       | 174 ms: 1.11x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 145 ms: 1.10x faster                                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.61 ms: 1.10x faster                                                        |
| 2to3                     | 350 ms                                                       | 322 ms: 1.09x faster                                                         |
| json                     | 5.86 ms                                                      | 5.41 ms: 1.08x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 75.6 ms: 1.07x faster                                                        |
| async_generators         | 421 ms                                                       | 393 ms: 1.07x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 2.02 sec: 1.07x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 982 ms: 1.07x faster                                                         |
| sympy_str                | 360 ms                                                       | 337 ms: 1.07x faster                                                         |
| gunicorn                 | 1.16 ms                                                      | 1.09 ms: 1.07x faster                                                        |
| aiohttp                  | 1.19 ms                                                      | 1.11 ms: 1.07x faster                                                        |
| comprehensions           | 26.7 us                                                      | 25.2 us: 1.06x faster                                                        |
| float                    | 111 ms                                                       | 105 ms: 1.06x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 20.2 ms: 1.06x faster                                                        |
| pyflate                  | 733 ms                                                       | 695 ms: 1.05x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 66.5 ms: 1.05x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.84 us: 1.05x faster                                                        |
| regex_dna                | 261 ms                                                       | 249 ms: 1.05x faster                                                         |
| sympy_expand             | 600 ms                                                       | 573 ms: 1.05x faster                                                         |
| genshi_text              | 31.4 ms                                                      | 30.0 ms: 1.05x faster                                                        |
| mako                     | 14.7 ms                                                      | 14.1 ms: 1.04x faster                                                        |
| regex_v8                 | 27.2 ms                                                      | 26.4 ms: 1.03x faster                                                        |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 105 ms: 1.02x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 90.6 ms: 1.02x faster                                                        |
| nbody                    | 134 ms                                                       | 132 ms: 1.02x faster                                                         |
| unpickle_list            | 4.65 us                                                      | 4.59 us: 1.01x faster                                                        |
| asyncio_websockets       | 390 ms                                                       | 387 ms: 1.01x faster                                                         |
| unpickle_pure_python     | 312 us                                                       | 309 us: 1.01x faster                                                         |
| genshi_xml               | 63.3 ms                                                      | 62.8 ms: 1.01x faster                                                        |
| nqueens                  | 115 ms                                                       | 117 ms: 1.01x slower                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 113 ms: 1.03x slower                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.99 sec: 1.03x slower                                                       |
| meteor_contest           | 138 ms                                                       | 143 ms: 1.03x slower                                                         |
| gc_traversal             | 3.42 ms                                                      | 3.61 ms: 1.06x slower                                                        |
| regex_compile            | 190 ms                                                       | 203 ms: 1.07x slower                                                         |
| pickle_list              | 4.12 us                                                      | 4.45 us: 1.08x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.8 us: 1.09x slower                                                        |
| spectral_norm            | 139 ms                                                       | 152 ms: 1.09x slower                                                         |
| unpack_sequence          | 59.9 ns                                                      | 65.7 ns: 1.10x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.8 ms: 1.11x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 32.8 us: 1.11x slower                                                        |
| unpickle                 | 13.5 us                                                      | 15.0 us: 1.12x slower                                                        |
| fannkuch                 | 483 ms                                                       | 543 ms: 1.12x slower                                                         |
| hexiom                   | 9.42 ms                                                      | 10.7 ms: 1.13x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.28 ms: 1.15x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.58 ms: 1.16x slower                                                        |
| scimark_fft              | 361 ms                                                       | 430 ms: 1.19x slower                                                         |
| dask                     | 472 ms                                                       | 591 ms: 1.25x slower                                                         |
| coverage                 | 63.3 ms                                                      | 82.4 ms: 1.30x slower                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.71 ms: 1.32x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.14x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240308-3.13.0a4+-fdb2d90-PYTHON_UOPS/bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 1.08x