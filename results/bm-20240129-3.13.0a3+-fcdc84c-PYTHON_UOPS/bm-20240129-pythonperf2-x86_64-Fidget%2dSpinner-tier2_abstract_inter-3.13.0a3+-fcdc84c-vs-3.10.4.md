
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.21x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 309 ms: 1.13x faster                                                                   |
| chameleon      | 9.44 ms                                                      | 8.13 ms: 1.16x faster                                                                  |
| docutils       | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                                 |
| tornado_http   | 157 ms                                                       | 126 ms: 1.24x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.18x faster                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 440 ms: 1.57x faster                                                                   |
| async_tree_memoization  | 819 ms                                                       | 550 ms: 1.49x faster                                                                   |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                                 |
| async_tree_cpu_io_mixed | 936 ms                                                       | 705 ms: 1.33x faster                                                                   |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 111 ms: 1.21x faster                                                                   |
| float          | 111 ms                                                       | 94.5 ms: 1.18x faster                                                                  |
| pidigits       | 271 ms                                                       | 264 ms: 1.02x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.13x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 168 ms: 1.13x faster                                                                   |
| regex_dna      | 261 ms                                                       | 236 ms: 1.11x faster                                                                   |
| regex_v8       | 27.2 ms                                                      | 25.8 ms: 1.05x faster                                                                  |
| regex_effbot   | 3.09 ms                                                      | 3.42 ms: 1.11x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 312 us: 1.46x faster                                                                   |
| unpickle_pure_python | 312 us                                                       | 229 us: 1.36x faster                                                                   |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                                  |
| xml_etree_process    | 75.9 ms                                                      | 61.2 ms: 1.24x faster                                                                  |
| json_loads           | 30.3 us                                                      | 24.5 us: 1.24x faster                                                                  |
| tomli_loads          | 2.92 sec                                                     | 2.58 sec: 1.13x faster                                                                 |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                                   |
| xml_etree_generate   | 92.3 ms                                                      | 90.1 ms: 1.02x faster                                                                  |
| xml_etree_iterparse  | 110 ms                                                       | 113 ms: 1.02x slower                                                                   |
| unpickle_list        | 4.65 us                                                      | 4.76 us: 1.02x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.5 us: 1.06x slower                                                                  |
| pickle_list          | 4.12 us                                                      | 4.40 us: 1.07x slower                                                                  |
| pickle_dict          | 29.5 us                                                      | 32.4 us: 1.10x slower                                                                  |
| unpickle             | 13.5 us                                                      | 14.9 us: 1.10x slower                                                                  |
| Geometric mean       | (ref)                                                        | 1.10x faster                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                                  |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 14.0 ms: 1.05x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 129 us: 4.16x faster                                                                   |
| asyncio_tcp              | 779 ms                                                       | 373 ms: 2.09x faster                                                                   |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                                 |
| logging_silent           | 167 ns                                                       | 99.5 ns: 1.68x faster                                                                  |
| generators               | 57.3 ms                                                      | 34.1 ms: 1.68x faster                                                                  |
| raytrace                 | 489 ms                                                       | 300 ms: 1.63x faster                                                                   |
| scimark_lu               | 167 ms                                                       | 104 ms: 1.60x faster                                                                   |
| sqlglot_parse            | 2.24 ms                                                      | 1.42 ms: 1.58x faster                                                                  |
| async_tree_none          | 692 ms                                                       | 440 ms: 1.57x faster                                                                   |
| deltablue                | 7.50 ms                                                      | 4.81 ms: 1.56x faster                                                                  |
| chaos                    | 109 ms                                                       | 72.0 ms: 1.51x faster                                                                  |
| richards_super           | 90.6 ms                                                      | 60.5 ms: 1.50x faster                                                                  |
| async_tree_memoization   | 819 ms                                                       | 550 ms: 1.49x faster                                                                   |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                                 |
| go                       | 262 ms                                                       | 177 ms: 1.48x faster                                                                   |
| sqlglot_transpile        | 2.68 ms                                                      | 1.84 ms: 1.46x faster                                                                  |
| pickle_pure_python       | 455 us                                                       | 312 us: 1.46x faster                                                                   |
| crypto_pyaes             | 119 ms                                                       | 82.5 ms: 1.44x faster                                                                  |
| richards                 | 75.1 ms                                                      | 54.2 ms: 1.39x faster                                                                  |
| unpack_sequence          | 59.9 ns                                                      | 43.3 ns: 1.39x faster                                                                  |
| bench_mp_pool            | 6.37 ms                                                      | 4.60 ms: 1.38x faster                                                                  |
| unpickle_pure_python     | 312 us                                                       | 229 us: 1.36x faster                                                                   |
| coroutines               | 30.3 ms                                                      | 22.5 ms: 1.35x faster                                                                  |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                                  |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 705 ms: 1.33x faster                                                                   |
| logging_format           | 9.64 us                                                      | 7.28 us: 1.32x faster                                                                  |
| pyflate                  | 733 ms                                                       | 554 ms: 1.32x faster                                                                   |
| logging_simple           | 8.88 us                                                      | 6.73 us: 1.32x faster                                                                  |
| scimark_monte_carlo      | 107 ms                                                       | 81.8 ms: 1.31x faster                                                                  |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                                 |
| tornado_http             | 157 ms                                                       | 126 ms: 1.24x faster                                                                   |
| xml_etree_process        | 75.9 ms                                                      | 61.2 ms: 1.24x faster                                                                  |
| json_loads               | 30.3 us                                                      | 24.5 us: 1.24x faster                                                                  |
| scimark_sor              | 180 ms                                                       | 147 ms: 1.22x faster                                                                   |
| deepcopy                 | 468 us                                                       | 384 us: 1.22x faster                                                                   |
| nbody                    | 134 ms                                                       | 111 ms: 1.21x faster                                                                   |
| deepcopy_memo            | 49.8 us                                                      | 41.2 us: 1.21x faster                                                                  |
| float                    | 111 ms                                                       | 94.5 ms: 1.18x faster                                                                  |
| deepcopy_reduce          | 4.01 us                                                      | 3.41 us: 1.18x faster                                                                  |
| bench_thread_pool        | 1.14 ms                                                      | 971 us: 1.18x faster                                                                   |
| pprint_safe_repr         | 1.05 sec                                                     | 895 ms: 1.17x faster                                                                   |
| sqlglot_normalize        | 144 ms                                                       | 123 ms: 1.17x faster                                                                   |
| pprint_pformat           | 2.15 sec                                                     | 1.85 sec: 1.17x faster                                                                 |
| docutils                 | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                                 |
| chameleon                | 9.44 ms                                                      | 8.13 ms: 1.16x faster                                                                  |
| dask                     | 472 ms                                                       | 408 ms: 1.16x faster                                                                   |
| comprehensions           | 26.7 us                                                      | 23.2 us: 1.15x faster                                                                  |
| sympy_sum                | 193 ms                                                       | 167 ms: 1.15x faster                                                                   |
| sympy_integrate          | 28.2 ms                                                      | 24.7 ms: 1.14x faster                                                                  |
| 2to3                     | 350 ms                                                       | 309 ms: 1.13x faster                                                                   |
| regex_compile            | 190 ms                                                       | 168 ms: 1.13x faster                                                                   |
| dulwich_log              | 81.1 ms                                                      | 71.7 ms: 1.13x faster                                                                  |
| tomli_loads              | 2.92 sec                                                     | 2.58 sec: 1.13x faster                                                                 |
| mdp                      | 3.01 sec                                                     | 2.66 sec: 1.13x faster                                                                 |
| sympy_str                | 360 ms                                                       | 319 ms: 1.13x faster                                                                   |
| json                     | 5.86 ms                                                      | 5.20 ms: 1.13x faster                                                                  |
| nqueens                  | 115 ms                                                       | 103 ms: 1.12x faster                                                                   |
| sympy_expand             | 600 ms                                                       | 536 ms: 1.12x faster                                                                   |
| async_generators         | 421 ms                                                       | 379 ms: 1.11x faster                                                                   |
| sqlglot_optimize         | 70.1 ms                                                      | 63.2 ms: 1.11x faster                                                                  |
| pathlib                  | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                                                  |
| regex_dna                | 261 ms                                                       | 236 ms: 1.11x faster                                                                   |
| fannkuch                 | 483 ms                                                       | 438 ms: 1.10x faster                                                                   |
| create_gc_cycles         | 1.76 ms                                                      | 1.60 ms: 1.10x faster                                                                  |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                                   |
| sqlite_synth             | 2.99 us                                                      | 2.82 us: 1.06x faster                                                                  |
| regex_v8                 | 27.2 ms                                                      | 25.8 ms: 1.05x faster                                                                  |
| mako                     | 14.7 ms                                                      | 14.0 ms: 1.05x faster                                                                  |
| hexiom                   | 9.42 ms                                                      | 8.99 ms: 1.05x faster                                                                  |
| spectral_norm            | 139 ms                                                       | 135 ms: 1.03x faster                                                                   |
| pidigits                 | 271 ms                                                       | 264 ms: 1.02x faster                                                                   |
| xml_etree_generate       | 92.3 ms                                                      | 90.1 ms: 1.02x faster                                                                  |
| asyncio_websockets       | 390 ms                                                       | 384 ms: 1.02x faster                                                                   |
| meteor_contest           | 138 ms                                                       | 136 ms: 1.01x faster                                                                   |
| xml_etree_iterparse      | 110 ms                                                       | 113 ms: 1.02x slower                                                                   |
| unpickle_list            | 4.65 us                                                      | 4.76 us: 1.02x slower                                                                  |
| gc_traversal             | 3.42 ms                                                      | 3.53 ms: 1.03x slower                                                                  |
| scimark_fft              | 361 ms                                                       | 379 ms: 1.05x slower                                                                   |
| pickle                   | 9.89 us                                                      | 10.5 us: 1.06x slower                                                                  |
| pickle_list              | 4.12 us                                                      | 4.40 us: 1.07x slower                                                                  |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                                  |
| pickle_dict              | 29.5 us                                                      | 32.4 us: 1.10x slower                                                                  |
| unpickle                 | 13.5 us                                                      | 14.9 us: 1.10x slower                                                                  |
| regex_effbot             | 3.09 ms                                                      | 3.42 ms: 1.11x slower                                                                  |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.82 ms: 1.15x slower                                                                  |
| telco                    | 7.23 ms                                                      | 8.35 ms: 1.16x slower                                                                  |
| coverage                 | 63.3 ms                                                      | 78.5 ms: 1.24x slower                                                                  |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                                  |
| Geometric mean           | (ref)                                                        | 1.21x faster                                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240129-3.13.0a3+-fcdc84c-PYTHON_UOPS/bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.07x