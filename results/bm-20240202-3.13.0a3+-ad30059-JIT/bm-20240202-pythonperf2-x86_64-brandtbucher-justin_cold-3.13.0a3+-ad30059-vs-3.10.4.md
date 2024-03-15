
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_cold
- machine: linux-x86_64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 302 ms: 1.16x faster                                                      |
| chameleon      | 9.44 ms                                                      | 7.93 ms: 1.19x faster                                                     |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.18x faster                                                    |
| tornado_http   | 157 ms                                                       | 125 ms: 1.25x faster                                                      |
| Geometric mean | (ref)                                                        | 1.20x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 440 ms: 1.57x faster                                                      |
| async_tree_memoization  | 819 ms                                                       | 552 ms: 1.48x faster                                                      |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                    |
| async_tree_cpu_io_mixed | 936 ms                                                       | 702 ms: 1.33x faster                                                      |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 83.1 ms: 1.34x faster                                                     |
| nbody          | 134 ms                                                       | 107 ms: 1.25x faster                                                      |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                      |
| Geometric mean | (ref)                                                        | 1.20x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 148 ms: 1.28x faster                                                      |
| regex_dna      | 261 ms                                                       | 251 ms: 1.04x faster                                                      |
| regex_v8       | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                     |
| regex_effbot   | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                     |
| Geometric mean | (ref)                                                        | 1.05x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 308 us: 1.48x faster                                                      |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                     |
| unpickle_pure_python | 312 us                                                       | 232 us: 1.34x faster                                                      |
| xml_etree_process    | 75.9 ms                                                      | 59.5 ms: 1.28x faster                                                     |
| tomli_loads          | 2.92 sec                                                     | 2.38 sec: 1.23x faster                                                    |
| json_loads           | 30.3 us                                                      | 25.1 us: 1.21x faster                                                     |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                      |
| xml_etree_generate   | 92.3 ms                                                      | 87.1 ms: 1.06x faster                                                     |
| xml_etree_iterparse  | 110 ms                                                       | 108 ms: 1.03x faster                                                      |
| unpickle_list        | 4.65 us                                                      | 4.77 us: 1.03x slower                                                     |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                     |
| pickle_dict          | 29.5 us                                                      | 30.8 us: 1.05x slower                                                     |
| pickle_list          | 4.12 us                                                      | 4.34 us: 1.05x slower                                                     |
| unpickle             | 13.5 us                                                      | 15.5 us: 1.15x slower                                                     |
| Geometric mean       | (ref)                                                        | 1.11x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                     |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                     |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.9 ms: 1.23x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 124 us: 4.33x faster                                                      |
| asyncio_tcp              | 779 ms                                                       | 369 ms: 2.11x faster                                                      |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                    |
| deltablue                | 7.50 ms                                                      | 4.05 ms: 1.85x faster                                                     |
| logging_silent           | 167 ns                                                       | 95.1 ns: 1.76x faster                                                     |
| raytrace                 | 489 ms                                                       | 281 ms: 1.74x faster                                                      |
| scimark_lu               | 167 ms                                                       | 99.4 ms: 1.68x faster                                                     |
| generators               | 57.3 ms                                                      | 34.5 ms: 1.66x faster                                                     |
| sqlglot_parse            | 2.24 ms                                                      | 1.38 ms: 1.62x faster                                                     |
| async_tree_none          | 692 ms                                                       | 440 ms: 1.57x faster                                                      |
| richards_super           | 90.6 ms                                                      | 58.2 ms: 1.56x faster                                                     |
| chaos                    | 109 ms                                                       | 70.7 ms: 1.53x faster                                                     |
| go                       | 262 ms                                                       | 173 ms: 1.51x faster                                                      |
| sqlglot_transpile        | 2.68 ms                                                      | 1.80 ms: 1.49x faster                                                     |
| async_tree_memoization   | 819 ms                                                       | 552 ms: 1.48x faster                                                      |
| richards                 | 75.1 ms                                                      | 50.7 ms: 1.48x faster                                                     |
| pickle_pure_python       | 455 us                                                       | 308 us: 1.48x faster                                                      |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                    |
| crypto_pyaes             | 119 ms                                                       | 81.5 ms: 1.46x faster                                                     |
| pyflate                  | 733 ms                                                       | 522 ms: 1.40x faster                                                      |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                     |
| unpack_sequence          | 59.9 ns                                                      | 43.7 ns: 1.37x faster                                                     |
| unpickle_pure_python     | 312 us                                                       | 232 us: 1.34x faster                                                      |
| scimark_monte_carlo      | 107 ms                                                       | 80.0 ms: 1.34x faster                                                     |
| float                    | 111 ms                                                       | 83.1 ms: 1.34x faster                                                     |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 702 ms: 1.33x faster                                                      |
| coroutines               | 30.3 ms                                                      | 22.8 ms: 1.33x faster                                                     |
| pycparser                | 1.67 sec                                                     | 1.29 sec: 1.29x faster                                                    |
| deepcopy_memo            | 49.8 us                                                      | 38.7 us: 1.29x faster                                                     |
| logging_simple           | 8.88 us                                                      | 6.92 us: 1.28x faster                                                     |
| regex_compile            | 190 ms                                                       | 148 ms: 1.28x faster                                                      |
| logging_format           | 9.64 us                                                      | 7.55 us: 1.28x faster                                                     |
| xml_etree_process        | 75.9 ms                                                      | 59.5 ms: 1.28x faster                                                     |
| comprehensions           | 26.7 us                                                      | 20.9 us: 1.27x faster                                                     |
| scimark_sor              | 180 ms                                                       | 142 ms: 1.27x faster                                                      |
| bench_mp_pool            | 6.37 ms                                                      | 5.08 ms: 1.26x faster                                                     |
| nbody                    | 134 ms                                                       | 107 ms: 1.25x faster                                                      |
| tornado_http             | 157 ms                                                       | 125 ms: 1.25x faster                                                      |
| mako                     | 14.7 ms                                                      | 11.9 ms: 1.23x faster                                                     |
| tomli_loads              | 2.92 sec                                                     | 2.38 sec: 1.23x faster                                                    |
| deepcopy                 | 468 us                                                       | 386 us: 1.21x faster                                                      |
| json_loads               | 30.3 us                                                      | 25.1 us: 1.21x faster                                                     |
| pprint_safe_repr         | 1.05 sec                                                     | 878 ms: 1.20x faster                                                      |
| sympy_sum                | 193 ms                                                       | 161 ms: 1.19x faster                                                      |
| chameleon                | 9.44 ms                                                      | 7.93 ms: 1.19x faster                                                     |
| pprint_pformat           | 2.15 sec                                                     | 1.81 sec: 1.19x faster                                                    |
| sympy_str                | 360 ms                                                       | 303 ms: 1.19x faster                                                      |
| sqlglot_normalize        | 144 ms                                                       | 121 ms: 1.19x faster                                                      |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.18x faster                                                    |
| sympy_expand             | 600 ms                                                       | 509 ms: 1.18x faster                                                      |
| dulwich_log              | 81.1 ms                                                      | 68.9 ms: 1.18x faster                                                     |
| deepcopy_reduce          | 4.01 us                                                      | 3.41 us: 1.18x faster                                                     |
| mdp                      | 3.01 sec                                                     | 2.57 sec: 1.17x faster                                                    |
| hexiom                   | 9.42 ms                                                      | 8.10 ms: 1.16x faster                                                     |
| bench_thread_pool        | 1.14 ms                                                      | 984 us: 1.16x faster                                                      |
| dask                     | 472 ms                                                       | 407 ms: 1.16x faster                                                      |
| 2to3                     | 350 ms                                                       | 302 ms: 1.16x faster                                                      |
| sympy_integrate          | 28.2 ms                                                      | 24.4 ms: 1.16x faster                                                     |
| spectral_norm            | 139 ms                                                       | 122 ms: 1.14x faster                                                      |
| sqlglot_optimize         | 70.1 ms                                                      | 61.8 ms: 1.14x faster                                                     |
| create_gc_cycles         | 1.76 ms                                                      | 1.55 ms: 1.14x faster                                                     |
| nqueens                  | 115 ms                                                       | 102 ms: 1.13x faster                                                      |
| pathlib                  | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                                     |
| fannkuch                 | 483 ms                                                       | 431 ms: 1.12x faster                                                      |
| json                     | 5.86 ms                                                      | 5.26 ms: 1.11x faster                                                     |
| async_generators         | 421 ms                                                       | 379 ms: 1.11x faster                                                      |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                      |
| sqlite_synth             | 2.99 us                                                      | 2.74 us: 1.09x faster                                                     |
| meteor_contest           | 138 ms                                                       | 130 ms: 1.06x faster                                                      |
| xml_etree_generate       | 92.3 ms                                                      | 87.1 ms: 1.06x faster                                                     |
| regex_dna                | 261 ms                                                       | 251 ms: 1.04x faster                                                      |
| regex_v8                 | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                     |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                      |
| xml_etree_iterparse      | 110 ms                                                       | 108 ms: 1.03x faster                                                      |
| scimark_fft              | 361 ms                                                       | 369 ms: 1.02x slower                                                      |
| unpickle_list            | 4.65 us                                                      | 4.77 us: 1.03x slower                                                     |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.22 ms: 1.03x slower                                                     |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.04x slower                                                     |
| pickle_dict              | 29.5 us                                                      | 30.8 us: 1.05x slower                                                     |
| pickle_list              | 4.12 us                                                      | 4.34 us: 1.05x slower                                                     |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                     |
| regex_effbot             | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                     |
| telco                    | 7.23 ms                                                      | 8.22 ms: 1.14x slower                                                     |
| unpickle                 | 13.5 us                                                      | 15.5 us: 1.15x slower                                                     |
| gc_traversal             | 3.42 ms                                                      | 4.09 ms: 1.20x slower                                                     |
| coverage                 | 63.3 ms                                                      | 84.1 ms: 1.33x slower                                                     |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                     |
| Geometric mean           | (ref)                                                        | 1.23x faster                                                              |

Benchmark hidden because not significant (2): mypy2, asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240202-3.13.0a3+-ad30059-JIT/bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.13x