
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 298 ms: 1.17x faster                                                          |
| chameleon      | 9.44 ms                                                      | 7.83 ms: 1.21x faster                                                         |
| docutils       | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                                        |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                                          |
| Geometric mean | (ref)                                                        | 1.21x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 434 ms: 1.59x faster                                                          |
| async_tree_memoization  | 819 ms                                                       | 549 ms: 1.49x faster                                                          |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.49x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 703 ms: 1.33x faster                                                          |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 79.4 ms: 1.40x faster                                                         |
| nbody          | 134 ms                                                       | 98.7 ms: 1.36x faster                                                         |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                          |
| Geometric mean | (ref)                                                        | 1.25x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 145 ms: 1.31x faster                                                          |
| regex_v8       | 27.2 ms                                                      | 26.2 ms: 1.04x faster                                                         |
| regex_dna      | 261 ms                                                       | 255 ms: 1.02x faster                                                          |
| regex_effbot   | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 314 us: 1.45x faster                                                          |
| json_dumps           | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.13 sec: 1.37x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 232 us: 1.34x faster                                                          |
| xml_etree_process    | 75.9 ms                                                      | 57.9 ms: 1.31x faster                                                         |
| json_loads           | 30.3 us                                                      | 25.3 us: 1.20x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 84.1 ms: 1.10x faster                                                         |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                          |
| xml_etree_iterparse  | 110 ms                                                       | 102 ms: 1.08x faster                                                          |
| unpickle_list        | 4.65 us                                                      | 4.77 us: 1.03x slower                                                         |
| pickle_list          | 4.12 us                                                      | 4.37 us: 1.06x slower                                                         |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                         |
| pickle_dict          | 29.5 us                                                      | 31.9 us: 1.08x slower                                                         |
| unpickle             | 13.5 us                                                      | 14.6 us: 1.08x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                         |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.6 ms: 1.39x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 121 us: 4.43x faster                                                          |
| asyncio_tcp              | 779 ms                                                       | 370 ms: 2.11x faster                                                          |
| deltablue                | 7.50 ms                                                      | 3.68 ms: 2.04x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                        |
| raytrace                 | 489 ms                                                       | 276 ms: 1.77x faster                                                          |
| logging_silent           | 167 ns                                                       | 95.9 ns: 1.74x faster                                                         |
| generators               | 57.3 ms                                                      | 33.9 ms: 1.69x faster                                                         |
| scimark_lu               | 167 ms                                                       | 101 ms: 1.65x faster                                                          |
| async_tree_none          | 692 ms                                                       | 434 ms: 1.59x faster                                                          |
| chaos                    | 109 ms                                                       | 68.3 ms: 1.59x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.41 ms: 1.58x faster                                                         |
| richards_super           | 90.6 ms                                                      | 57.4 ms: 1.58x faster                                                         |
| go                       | 262 ms                                                       | 168 ms: 1.56x faster                                                          |
| crypto_pyaes             | 119 ms                                                       | 77.4 ms: 1.54x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 549 ms: 1.49x faster                                                          |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.49x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.82 ms: 1.47x faster                                                         |
| richards                 | 75.1 ms                                                      | 51.5 ms: 1.46x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 314 us: 1.45x faster                                                          |
| pyflate                  | 733 ms                                                       | 522 ms: 1.40x faster                                                          |
| comprehensions           | 26.7 us                                                      | 19.0 us: 1.40x faster                                                         |
| json_dumps               | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                                         |
| float                    | 111 ms                                                       | 79.4 ms: 1.40x faster                                                         |
| spectral_norm            | 139 ms                                                       | 99.8 ms: 1.39x faster                                                         |
| mako                     | 14.7 ms                                                      | 10.6 ms: 1.39x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.13 sec: 1.37x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.2 ms: 1.36x faster                                                         |
| nbody                    | 134 ms                                                       | 98.7 ms: 1.36x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 79.2 ms: 1.36x faster                                                         |
| unpack_sequence          | 59.9 ns                                                      | 44.6 ns: 1.34x faster                                                         |
| unpickle_pure_python     | 312 us                                                       | 232 us: 1.34x faster                                                          |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 703 ms: 1.33x faster                                                          |
| bench_mp_pool            | 6.37 ms                                                      | 4.82 ms: 1.32x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.9 us: 1.31x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.76 us: 1.31x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 57.9 ms: 1.31x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.28 sec: 1.31x faster                                                        |
| regex_compile            | 190 ms                                                       | 145 ms: 1.31x faster                                                          |
| logging_format           | 9.64 us                                                      | 7.38 us: 1.31x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 7.33 ms: 1.28x faster                                                         |
| scimark_sor              | 180 ms                                                       | 142 ms: 1.27x faster                                                          |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                                          |
| pprint_pformat           | 2.15 sec                                                     | 1.71 sec: 1.26x faster                                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 837 ms: 1.25x faster                                                          |
| deepcopy                 | 468 us                                                       | 375 us: 1.25x faster                                                          |
| nqueens                  | 115 ms                                                       | 92.6 ms: 1.24x faster                                                         |
| fannkuch                 | 483 ms                                                       | 392 ms: 1.23x faster                                                          |
| sqlglot_normalize        | 144 ms                                                       | 118 ms: 1.22x faster                                                          |
| sympy_sum                | 193 ms                                                       | 159 ms: 1.21x faster                                                          |
| chameleon                | 9.44 ms                                                      | 7.83 ms: 1.21x faster                                                         |
| sympy_str                | 360 ms                                                       | 299 ms: 1.21x faster                                                          |
| json_loads               | 30.3 us                                                      | 25.3 us: 1.20x faster                                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.35 us: 1.20x faster                                                         |
| sympy_expand             | 600 ms                                                       | 504 ms: 1.19x faster                                                          |
| docutils                 | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 68.5 ms: 1.18x faster                                                         |
| 2to3                     | 350 ms                                                       | 298 ms: 1.17x faster                                                          |
| sympy_integrate          | 28.2 ms                                                      | 24.2 ms: 1.16x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.37 ms: 1.16x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 983 us: 1.16x faster                                                          |
| dask                     | 472 ms                                                       | 408 ms: 1.16x faster                                                          |
| sqlglot_optimize         | 70.1 ms                                                      | 60.6 ms: 1.16x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.60 sec: 1.16x faster                                                        |
| async_generators         | 421 ms                                                       | 368 ms: 1.14x faster                                                          |
| create_gc_cycles         | 1.76 ms                                                      | 1.54 ms: 1.14x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.13x faster                                                         |
| scimark_fft              | 361 ms                                                       | 325 ms: 1.11x faster                                                          |
| json                     | 5.86 ms                                                      | 5.29 ms: 1.11x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 84.1 ms: 1.10x faster                                                         |
| sqlite_synth             | 2.99 us                                                      | 2.72 us: 1.10x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                          |
| meteor_contest           | 138 ms                                                       | 128 ms: 1.08x faster                                                          |
| xml_etree_iterparse      | 110 ms                                                       | 102 ms: 1.08x faster                                                          |
| regex_v8                 | 27.2 ms                                                      | 26.2 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                          |
| regex_dna                | 261 ms                                                       | 255 ms: 1.02x faster                                                          |
| unpickle_list            | 4.65 us                                                      | 4.77 us: 1.03x slower                                                         |
| pickle_list              | 4.12 us                                                      | 4.37 us: 1.06x slower                                                         |
| pickle                   | 9.89 us                                                      | 10.6 us: 1.07x slower                                                         |
| pickle_dict              | 29.5 us                                                      | 31.9 us: 1.08x slower                                                         |
| unpickle                 | 13.5 us                                                      | 14.6 us: 1.08x slower                                                         |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                         |
| telco                    | 7.23 ms                                                      | 8.01 ms: 1.11x slower                                                         |
| regex_effbot             | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                                         |
| coverage                 | 63.3 ms                                                      | 81.8 ms: 1.29x slower                                                         |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.26x faster                                                                  |

Benchmark hidden because not significant (3): mypy2, asyncio_websockets, gc_traversal
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-6dafac2-JIT/bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.10x