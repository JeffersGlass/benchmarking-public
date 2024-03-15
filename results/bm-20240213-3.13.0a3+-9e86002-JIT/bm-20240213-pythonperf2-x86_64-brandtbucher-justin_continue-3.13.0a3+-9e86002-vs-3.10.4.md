
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 300 ms: 1.17x faster                                                          |
| chameleon      | 9.44 ms                                                      | 7.81 ms: 1.21x faster                                                         |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                                        |
| tornado_http   | 157 ms                                                       | 126 ms: 1.25x faster                                                          |
| Geometric mean | (ref)                                                        | 1.20x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 442 ms: 1.56x faster                                                          |
| async_tree_memoization  | 819 ms                                                       | 555 ms: 1.48x faster                                                          |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 708 ms: 1.32x faster                                                          |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 80.4 ms: 1.38x faster                                                         |
| nbody          | 134 ms                                                       | 104 ms: 1.29x faster                                                          |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                          |
| Geometric mean | (ref)                                                        | 1.23x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.30x faster                                                          |
| regex_dna      | 261 ms                                                       | 238 ms: 1.10x faster                                                          |
| regex_v8       | 27.2 ms                                                      | 26.0 ms: 1.04x faster                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.41 ms: 1.10x slower                                                         |
| Geometric mean | (ref)                                                        | 1.08x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 314 us: 1.45x faster                                                          |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.38x faster                                                         |
| unpickle_pure_python | 312 us                                                       | 233 us: 1.34x faster                                                          |
| xml_etree_process    | 75.9 ms                                                      | 58.6 ms: 1.30x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.27 sec: 1.28x faster                                                        |
| json_loads           | 30.3 us                                                      | 25.0 us: 1.21x faster                                                         |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                          |
| xml_etree_generate   | 92.3 ms                                                      | 84.6 ms: 1.09x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.06x faster                                                          |
| unpickle_list        | 4.65 us                                                      | 4.83 us: 1.04x slower                                                         |
| pickle_dict          | 29.5 us                                                      | 30.8 us: 1.04x slower                                                         |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                         |
| pickle_list          | 4.12 us                                                      | 4.40 us: 1.07x slower                                                         |
| unpickle             | 13.5 us                                                      | 15.2 us: 1.13x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                         |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.0 ms: 1.34x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|--------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 120 us: 4.45x faster                                                          |
| asyncio_tcp              | 779 ms                                                       | 368 ms: 2.12x faster                                                          |
| deltablue                | 7.50 ms                                                      | 3.70 ms: 2.03x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                        |
| raytrace                 | 489 ms                                                       | 276 ms: 1.77x faster                                                          |
| logging_silent           | 167 ns                                                       | 95.8 ns: 1.75x faster                                                         |
| scimark_lu               | 167 ms                                                       | 99.9 ms: 1.67x faster                                                         |
| generators               | 57.3 ms                                                      | 34.6 ms: 1.66x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.40 ms: 1.59x faster                                                         |
| richards_super           | 90.6 ms                                                      | 57.4 ms: 1.58x faster                                                         |
| async_tree_none          | 692 ms                                                       | 442 ms: 1.56x faster                                                          |
| chaos                    | 109 ms                                                       | 70.9 ms: 1.53x faster                                                         |
| crypto_pyaes             | 119 ms                                                       | 78.3 ms: 1.52x faster                                                         |
| go                       | 262 ms                                                       | 172 ms: 1.52x faster                                                          |
| richards                 | 75.1 ms                                                      | 50.6 ms: 1.48x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 555 ms: 1.48x faster                                                          |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.83 ms: 1.46x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 314 us: 1.45x faster                                                          |
| pyflate                  | 733 ms                                                       | 514 ms: 1.43x faster                                                          |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.38x faster                                                         |
| float                    | 111 ms                                                       | 80.4 ms: 1.38x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 77.8 ms: 1.38x faster                                                         |
| coroutines               | 30.3 ms                                                      | 22.2 ms: 1.36x faster                                                         |
| comprehensions           | 26.7 us                                                      | 19.9 us: 1.34x faster                                                         |
| unpickle_pure_python     | 312 us                                                       | 233 us: 1.34x faster                                                          |
| mako                     | 14.7 ms                                                      | 11.0 ms: 1.34x faster                                                         |
| unpack_sequence          | 59.9 ns                                                      | 44.9 ns: 1.33x faster                                                         |
| bench_mp_pool            | 6.37 ms                                                      | 4.80 ms: 1.33x faster                                                         |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 708 ms: 1.32x faster                                                          |
| regex_compile            | 190 ms                                                       | 146 ms: 1.30x faster                                                          |
| logging_simple           | 8.88 us                                                      | 6.83 us: 1.30x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 38.3 us: 1.30x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 58.6 ms: 1.30x faster                                                         |
| nbody                    | 134 ms                                                       | 104 ms: 1.29x faster                                                          |
| spectral_norm            | 139 ms                                                       | 108 ms: 1.28x faster                                                          |
| tomli_loads              | 2.92 sec                                                     | 2.27 sec: 1.28x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.53 us: 1.28x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                        |
| scimark_sor              | 180 ms                                                       | 144 ms: 1.25x faster                                                          |
| pprint_safe_repr         | 1.05 sec                                                     | 840 ms: 1.25x faster                                                          |
| tornado_http             | 157 ms                                                       | 126 ms: 1.25x faster                                                          |
| pprint_pformat           | 2.15 sec                                                     | 1.72 sec: 1.25x faster                                                        |
| hexiom                   | 9.42 ms                                                      | 7.56 ms: 1.24x faster                                                         |
| deepcopy                 | 468 us                                                       | 385 us: 1.21x faster                                                          |
| json_loads               | 30.3 us                                                      | 25.0 us: 1.21x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.81 ms: 1.21x faster                                                         |
| sympy_str                | 360 ms                                                       | 300 ms: 1.20x faster                                                          |
| sqlglot_normalize        | 144 ms                                                       | 120 ms: 1.20x faster                                                          |
| sympy_sum                | 193 ms                                                       | 161 ms: 1.20x faster                                                          |
| nqueens                  | 115 ms                                                       | 96.3 ms: 1.19x faster                                                         |
| fannkuch                 | 483 ms                                                       | 405 ms: 1.19x faster                                                          |
| sympy_expand             | 600 ms                                                       | 503 ms: 1.19x faster                                                          |
| mdp                      | 3.01 sec                                                     | 2.53 sec: 1.19x faster                                                        |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 968 us: 1.18x faster                                                          |
| deepcopy_reduce          | 4.01 us                                                      | 3.41 us: 1.18x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 69.1 ms: 1.17x faster                                                         |
| 2to3                     | 350 ms                                                       | 300 ms: 1.17x faster                                                          |
| sympy_integrate          | 28.2 ms                                                      | 24.4 ms: 1.15x faster                                                         |
| dask                     | 472 ms                                                       | 411 ms: 1.15x faster                                                          |
| async_generators         | 421 ms                                                       | 367 ms: 1.15x faster                                                          |
| sqlglot_optimize         | 70.1 ms                                                      | 61.2 ms: 1.15x faster                                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.55 ms: 1.14x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 18.9 ms: 1.13x faster                                                         |
| json                     | 5.86 ms                                                      | 5.29 ms: 1.11x faster                                                         |
| regex_dna                | 261 ms                                                       | 238 ms: 1.10x faster                                                          |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                          |
| sqlite_synth             | 2.99 us                                                      | 2.74 us: 1.09x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 84.6 ms: 1.09x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.06x faster                                                          |
| meteor_contest           | 138 ms                                                       | 132 ms: 1.05x faster                                                          |
| regex_v8                 | 27.2 ms                                                      | 26.0 ms: 1.04x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.89 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                          |
| scimark_fft              | 361 ms                                                       | 354 ms: 1.02x faster                                                          |
| asyncio_websockets       | 390 ms                                                       | 385 ms: 1.01x faster                                                          |
| unpickle_list            | 4.65 us                                                      | 4.83 us: 1.04x slower                                                         |
| pickle_dict              | 29.5 us                                                      | 30.8 us: 1.04x slower                                                         |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                                         |
| pickle_list              | 4.12 us                                                      | 4.40 us: 1.07x slower                                                         |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                         |
| regex_effbot             | 3.09 ms                                                      | 3.41 ms: 1.10x slower                                                         |
| telco                    | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                         |
| unpickle                 | 13.5 us                                                      | 15.2 us: 1.13x slower                                                         |
| gc_traversal             | 3.42 ms                                                      | 3.90 ms: 1.14x slower                                                         |
| coverage                 | 63.3 ms                                                      | 78.3 ms: 1.24x slower                                                         |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.25x faster                                                                  |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240213-3.13.0a3+-9e86002-JIT/bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.10x