
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 298 ms: 1.17x faster                                                       |
| chameleon      | 9.44 ms                                                      | 7.60 ms: 1.24x faster                                                      |
| docutils       | 3.41 sec                                                     | 2.90 sec: 1.18x faster                                                     |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                        | 1.21x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 435 ms: 1.59x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 548 ms: 1.50x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.49x faster                                                     |
| async_tree_cpu_io_mixed | 936 ms                                                       | 698 ms: 1.34x faster                                                       |
| Geometric mean          | (ref)                                                        | 1.48x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 94.1 ms: 1.42x faster                                                      |
| float          | 111 ms                                                       | 80.5 ms: 1.38x faster                                                      |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                        | 1.27x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.30x faster                                                       |
| regex_dna      | 261 ms                                                       | 248 ms: 1.06x faster                                                       |
| regex_v8       | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                      |
| regex_effbot   | 3.09 ms                                                      | 3.61 ms: 1.17x slower                                                      |
| Geometric mean | (ref)                                                        | 1.05x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 307 us: 1.48x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                      |
| unpickle_pure_python | 312 us                                                       | 230 us: 1.36x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 59.1 ms: 1.29x faster                                                      |
| tomli_loads          | 2.92 sec                                                     | 2.31 sec: 1.26x faster                                                     |
| json_loads           | 30.3 us                                                      | 25.0 us: 1.21x faster                                                      |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 85.9 ms: 1.07x faster                                                      |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.05x faster                                                       |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| pickle_dict          | 29.5 us                                                      | 30.9 us: 1.05x slower                                                      |
| unpickle_list        | 4.65 us                                                      | 4.93 us: 1.06x slower                                                      |
| pickle_list          | 4.12 us                                                      | 4.46 us: 1.08x slower                                                      |
| unpickle             | 13.5 us                                                      | 15.1 us: 1.12x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                      |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.6 ms: 1.27x faster                                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 121 us: 4.44x faster                                                       |
| asyncio_tcp              | 779 ms                                                       | 370 ms: 2.11x faster                                                       |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                     |
| deltablue                | 7.50 ms                                                      | 3.91 ms: 1.92x faster                                                      |
| raytrace                 | 489 ms                                                       | 270 ms: 1.81x faster                                                       |
| logging_silent           | 167 ns                                                       | 95.8 ns: 1.75x faster                                                      |
| generators               | 57.3 ms                                                      | 34.4 ms: 1.66x faster                                                      |
| scimark_lu               | 167 ms                                                       | 102 ms: 1.64x faster                                                       |
| chaos                    | 109 ms                                                       | 66.8 ms: 1.63x faster                                                      |
| sqlglot_parse            | 2.24 ms                                                      | 1.39 ms: 1.61x faster                                                      |
| richards_super           | 90.6 ms                                                      | 56.4 ms: 1.61x faster                                                      |
| crypto_pyaes             | 119 ms                                                       | 75.0 ms: 1.59x faster                                                      |
| async_tree_none          | 692 ms                                                       | 435 ms: 1.59x faster                                                       |
| go                       | 262 ms                                                       | 168 ms: 1.55x faster                                                       |
| async_tree_memoization   | 819 ms                                                       | 548 ms: 1.50x faster                                                       |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.49x faster                                                     |
| richards                 | 75.1 ms                                                      | 50.6 ms: 1.49x faster                                                      |
| sqlglot_transpile        | 2.68 ms                                                      | 1.81 ms: 1.48x faster                                                      |
| pickle_pure_python       | 455 us                                                       | 307 us: 1.48x faster                                                       |
| pyflate                  | 733 ms                                                       | 506 ms: 1.45x faster                                                       |
| nbody                    | 134 ms                                                       | 94.1 ms: 1.42x faster                                                      |
| scimark_monte_carlo      | 107 ms                                                       | 75.8 ms: 1.42x faster                                                      |
| float                    | 111 ms                                                       | 80.5 ms: 1.38x faster                                                      |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                      |
| unpickle_pure_python     | 312 us                                                       | 230 us: 1.36x faster                                                       |
| logging_simple           | 8.88 us                                                      | 6.57 us: 1.35x faster                                                      |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 698 ms: 1.34x faster                                                       |
| coroutines               | 30.3 ms                                                      | 22.7 ms: 1.34x faster                                                      |
| logging_format           | 9.64 us                                                      | 7.27 us: 1.33x faster                                                      |
| comprehensions           | 26.7 us                                                      | 20.3 us: 1.31x faster                                                      |
| deepcopy_memo            | 49.8 us                                                      | 37.9 us: 1.31x faster                                                      |
| unpack_sequence          | 59.9 ns                                                      | 45.8 ns: 1.31x faster                                                      |
| regex_compile            | 190 ms                                                       | 146 ms: 1.30x faster                                                       |
| pycparser                | 1.67 sec                                                     | 1.29 sec: 1.30x faster                                                     |
| scimark_sor              | 180 ms                                                       | 140 ms: 1.29x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 59.1 ms: 1.29x faster                                                      |
| mako                     | 14.7 ms                                                      | 11.6 ms: 1.27x faster                                                      |
| deepcopy                 | 468 us                                                       | 371 us: 1.26x faster                                                       |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                                       |
| tomli_loads              | 2.92 sec                                                     | 2.31 sec: 1.26x faster                                                     |
| bench_mp_pool            | 6.37 ms                                                      | 5.11 ms: 1.25x faster                                                      |
| spectral_norm            | 139 ms                                                       | 112 ms: 1.25x faster                                                       |
| chameleon                | 9.44 ms                                                      | 7.60 ms: 1.24x faster                                                      |
| hexiom                   | 9.42 ms                                                      | 7.60 ms: 1.24x faster                                                      |
| pprint_safe_repr         | 1.05 sec                                                     | 858 ms: 1.22x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.29 us: 1.22x faster                                                      |
| sympy_sum                | 193 ms                                                       | 158 ms: 1.22x faster                                                       |
| json_loads               | 30.3 us                                                      | 25.0 us: 1.21x faster                                                      |
| sympy_str                | 360 ms                                                       | 297 ms: 1.21x faster                                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.79 sec: 1.20x faster                                                     |
| nqueens                  | 115 ms                                                       | 95.8 ms: 1.20x faster                                                      |
| sympy_expand             | 600 ms                                                       | 501 ms: 1.20x faster                                                       |
| dulwich_log              | 81.1 ms                                                      | 67.9 ms: 1.19x faster                                                      |
| sqlglot_normalize        | 144 ms                                                       | 120 ms: 1.19x faster                                                       |
| bench_thread_pool        | 1.14 ms                                                      | 964 us: 1.18x faster                                                       |
| fannkuch                 | 483 ms                                                       | 409 ms: 1.18x faster                                                       |
| mdp                      | 3.01 sec                                                     | 2.55 sec: 1.18x faster                                                     |
| docutils                 | 3.41 sec                                                     | 2.90 sec: 1.18x faster                                                     |
| 2to3                     | 350 ms                                                       | 298 ms: 1.17x faster                                                       |
| dask                     | 472 ms                                                       | 404 ms: 1.17x faster                                                       |
| sympy_integrate          | 28.2 ms                                                      | 24.1 ms: 1.17x faster                                                      |
| create_gc_cycles         | 1.76 ms                                                      | 1.52 ms: 1.16x faster                                                      |
| async_generators         | 421 ms                                                       | 366 ms: 1.15x faster                                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 61.5 ms: 1.14x faster                                                      |
| pathlib                  | 21.4 ms                                                      | 18.7 ms: 1.14x faster                                                      |
| json                     | 5.86 ms                                                      | 5.18 ms: 1.13x faster                                                      |
| sqlite_synth             | 2.99 us                                                      | 2.74 us: 1.09x faster                                                      |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                       |
| xml_etree_generate       | 92.3 ms                                                      | 85.9 ms: 1.07x faster                                                      |
| regex_dna                | 261 ms                                                       | 248 ms: 1.06x faster                                                       |
| meteor_contest           | 138 ms                                                       | 131 ms: 1.05x faster                                                       |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.05x faster                                                       |
| scimark_fft              | 361 ms                                                       | 346 ms: 1.04x faster                                                       |
| regex_v8                 | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                      |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                       |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.03 ms: 1.01x faster                                                      |
| asyncio_websockets       | 390 ms                                                       | 387 ms: 1.01x faster                                                       |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| pickle_dict              | 29.5 us                                                      | 30.9 us: 1.05x slower                                                      |
| unpickle_list            | 4.65 us                                                      | 4.93 us: 1.06x slower                                                      |
| pickle_list              | 4.12 us                                                      | 4.46 us: 1.08x slower                                                      |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                      |
| unpickle                 | 13.5 us                                                      | 15.1 us: 1.12x slower                                                      |
| telco                    | 7.23 ms                                                      | 8.11 ms: 1.12x slower                                                      |
| gc_traversal             | 3.42 ms                                                      | 3.88 ms: 1.14x slower                                                      |
| regex_effbot             | 3.09 ms                                                      | 3.61 ms: 1.17x slower                                                      |
| coverage                 | 63.3 ms                                                      | 79.3 ms: 1.25x slower                                                      |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                      |
| Geometric mean           | (ref)                                                        | 1.25x faster                                                               |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240203-3.13.0a3+-61c470b-JIT/bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.11x