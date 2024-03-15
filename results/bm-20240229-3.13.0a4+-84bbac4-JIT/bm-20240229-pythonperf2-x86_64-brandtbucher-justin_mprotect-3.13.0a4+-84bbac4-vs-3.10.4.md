# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.35x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 305 ms: 1.15x faster                                                          |
| chameleon      | 9.44 ms                                                      | 7.52 ms: 1.26x faster                                                         |
| docutils       | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                        |
| tornado_http   | 157 ms                                                       | 125 ms: 1.25x faster                                                          |
| Geometric mean | (ref)                                                        | 1.20x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 435 ms: 1.59x faster                                                          |
| async_tree_memoization  | 819 ms                                                       | 549 ms: 1.49x faster                                                          |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 701 ms: 1.33x faster                                                          |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 78.5 ms: 1.42x faster                                                         |
| nbody          | 134 ms                                                       | 98.0 ms: 1.37x faster                                                         |
| pidigits       | 271 ms                                                       | 261 ms: 1.04x faster                                                          |
| Geometric mean | (ref)                                                        | 1.26x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 147 ms: 1.29x faster                                                          |
| regex_dna      | 261 ms                                                       | 248 ms: 1.05x faster                                                          |
| regex_v8       | 27.2 ms                                                      | 26.0 ms: 1.04x faster                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.63 ms: 1.17x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 319 us: 1.43x faster                                                          |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 234 us: 1.34x faster                                                          |
| xml_etree_process    | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                                         |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.21x faster                                                         |
| xml_etree_parse      | 160 ms                                                       | 145 ms: 1.11x faster                                                          |
| xml_etree_generate   | 92.3 ms                                                      | 84.4 ms: 1.09x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 102 ms: 1.08x faster                                                          |
| unpickle_list        | 4.65 us                                                      | 4.58 us: 1.02x faster                                                         |
| pickle               | 9.89 us                                                      | 10.1 us: 1.03x slower                                                         |
| pickle_dict          | 29.5 us                                                      | 30.6 us: 1.04x slower                                                         |
| pickle_list          | 4.12 us                                                      | 4.43 us: 1.07x slower                                                         |
| unpickle             | 13.5 us                                                      | 14.9 us: 1.11x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 14.8 ms: 1.29x slower                                                         |
| python_startup_no_site | 7.33 ms                                                      | 13.3 ms: 1.81x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.53x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 9.96 ms: 1.48x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|--------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 119 us: 4.50x faster                                                          |
| asyncio_tcp              | 779 ms                                                       | 371 ms: 2.10x faster                                                          |
| deltablue                | 7.50 ms                                                      | 3.77 ms: 1.99x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                        |
| logging_silent           | 167 ns                                                       | 97.7 ns: 1.71x faster                                                         |
| generators               | 57.3 ms                                                      | 33.8 ms: 1.70x faster                                                         |
| raytrace                 | 489 ms                                                       | 303 ms: 1.62x faster                                                          |
| chaos                    | 109 ms                                                       | 67.8 ms: 1.60x faster                                                         |
| async_tree_none          | 692 ms                                                       | 435 ms: 1.59x faster                                                          |
| richards_super           | 90.6 ms                                                      | 57.3 ms: 1.58x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.42 ms: 1.57x faster                                                         |
| crypto_pyaes             | 119 ms                                                       | 77.8 ms: 1.53x faster                                                         |
| go                       | 262 ms                                                       | 171 ms: 1.53x faster                                                          |
| spectral_norm            | 139 ms                                                       | 92.7 ms: 1.50x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 549 ms: 1.49x faster                                                          |
| richards                 | 75.1 ms                                                      | 50.4 ms: 1.49x faster                                                         |
| mako                     | 14.7 ms                                                      | 9.96 ms: 1.48x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.86 ms: 1.45x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 319 us: 1.43x faster                                                          |
| pyflate                  | 733 ms                                                       | 517 ms: 1.42x faster                                                          |
| float                    | 111 ms                                                       | 78.5 ms: 1.42x faster                                                         |
| comprehensions           | 26.7 us                                                      | 19.0 us: 1.40x faster                                                         |
| scimark_lu               | 167 ms                                                       | 121 ms: 1.37x faster                                                          |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.47 us: 1.37x faster                                                         |
| nbody                    | 134 ms                                                       | 98.0 ms: 1.37x faster                                                         |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.18 us: 1.34x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 80.0 ms: 1.34x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.77 ms: 1.34x faster                                                         |
| unpickle_pure_python     | 312 us                                                       | 234 us: 1.34x faster                                                          |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 701 ms: 1.33x faster                                                          |
| deepcopy_memo            | 49.8 us                                                      | 38.0 us: 1.31x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                                         |
| regex_compile            | 190 ms                                                       | 147 ms: 1.29x faster                                                          |
| pycparser                | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 827 ms: 1.27x faster                                                          |
| hexiom                   | 9.42 ms                                                      | 7.43 ms: 1.27x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.70 sec: 1.27x faster                                                        |
| chameleon                | 9.44 ms                                                      | 7.52 ms: 1.26x faster                                                         |
| tornado_http             | 157 ms                                                       | 125 ms: 1.25x faster                                                          |
| deepcopy                 | 468 us                                                       | 374 us: 1.25x faster                                                          |
| fannkuch                 | 483 ms                                                       | 387 ms: 1.25x faster                                                          |
| json_loads               | 30.3 us                                                      | 25.2 us: 1.21x faster                                                         |
| sympy_sum                | 193 ms                                                       | 160 ms: 1.20x faster                                                          |
| sqlglot_normalize        | 144 ms                                                       | 120 ms: 1.20x faster                                                          |
| deepcopy_reduce          | 4.01 us                                                      | 3.37 us: 1.19x faster                                                         |
| sympy_str                | 360 ms                                                       | 305 ms: 1.18x faster                                                          |
| scimark_sor              | 180 ms                                                       | 153 ms: 1.18x faster                                                          |
| dulwich_log              | 81.1 ms                                                      | 68.8 ms: 1.18x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.57 sec: 1.17x faster                                                        |
| sympy_expand             | 600 ms                                                       | 515 ms: 1.17x faster                                                          |
| docutils                 | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 991 us: 1.15x faster                                                          |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.42 ms: 1.15x faster                                                         |
| 2to3                     | 350 ms                                                       | 305 ms: 1.15x faster                                                          |
| sympy_integrate          | 28.2 ms                                                      | 24.6 ms: 1.14x faster                                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.56 ms: 1.13x faster                                                         |
| nqueens                  | 115 ms                                                       | 102 ms: 1.13x faster                                                          |
| scimark_fft              | 361 ms                                                       | 324 ms: 1.12x faster                                                          |
| sqlite_synth             | 2.99 us                                                      | 2.69 us: 1.11x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 63.4 ms: 1.11x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 145 ms: 1.11x faster                                                          |
| async_generators         | 421 ms                                                       | 381 ms: 1.11x faster                                                          |
| json                     | 5.86 ms                                                      | 5.31 ms: 1.10x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 84.4 ms: 1.09x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 102 ms: 1.08x faster                                                          |
| regex_dna                | 261 ms                                                       | 248 ms: 1.05x faster                                                          |
| meteor_contest           | 138 ms                                                       | 131 ms: 1.05x faster                                                          |
| regex_v8                 | 27.2 ms                                                      | 26.0 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 261 ms: 1.04x faster                                                          |
| unpickle_list            | 4.65 us                                                      | 4.58 us: 1.02x faster                                                         |
| asyncio_websockets       | 390 ms                                                       | 387 ms: 1.01x faster                                                          |
| unpack_sequence          | 59.9 ns                                                      | 61.4 ns: 1.02x slower                                                         |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.03x slower                                                         |
| pickle_dict              | 29.5 us                                                      | 30.6 us: 1.04x slower                                                         |
| pickle_list              | 4.12 us                                                      | 4.43 us: 1.07x slower                                                         |
| gc_traversal             | 3.42 ms                                                      | 3.75 ms: 1.10x slower                                                         |
| unpickle                 | 13.5 us                                                      | 14.9 us: 1.11x slower                                                         |
| telco                    | 7.23 ms                                                      | 8.04 ms: 1.11x slower                                                         |
| regex_effbot             | 3.09 ms                                                      | 3.63 ms: 1.17x slower                                                         |
| dask                     | 472 ms                                                       | 591 ms: 1.25x slower                                                          |
| coverage                 | 63.3 ms                                                      | 80.4 ms: 1.27x slower                                                         |
| python_startup           | 11.5 ms                                                      | 14.8 ms: 1.29x slower                                                         |
| python_startup_no_site   | 7.33 ms                                                      | 13.3 ms: 1.81x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.24x faster                                                                  |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-84bbac4-JIT/bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.35x