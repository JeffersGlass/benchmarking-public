
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.20x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 309 ms: 1.13x faster                                                                   |
| chameleon      | 9.44 ms                                                      | 8.09 ms: 1.17x faster                                                                  |
| docutils       | 3.41 sec                                                     | 2.95 sec: 1.16x faster                                                                 |
| tornado_http   | 157 ms                                                       | 129 ms: 1.22x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.17x faster                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 438 ms: 1.58x faster                                                                   |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                                 |
| async_tree_memoization  | 819 ms                                                       | 549 ms: 1.49x faster                                                                   |
| async_tree_cpu_io_mixed | 936 ms                                                       | 702 ms: 1.33x faster                                                                   |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 114 ms: 1.18x faster                                                                   |
| float          | 111 ms                                                       | 95.3 ms: 1.17x faster                                                                  |
| pidigits       | 271 ms                                                       | 264 ms: 1.02x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.12x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 169 ms: 1.12x faster                                                                   |
| regex_dna      | 261 ms                                                       | 251 ms: 1.04x faster                                                                   |
| regex_v8       | 27.2 ms                                                      | 26.3 ms: 1.03x faster                                                                  |
| regex_effbot   | 3.09 ms                                                      | 3.57 ms: 1.16x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 314 us: 1.45x faster                                                                   |
| unpickle_pure_python | 312 us                                                       | 229 us: 1.36x faster                                                                   |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.34x faster                                                                  |
| xml_etree_process    | 75.9 ms                                                      | 61.6 ms: 1.23x faster                                                                  |
| json_loads           | 30.3 us                                                      | 24.9 us: 1.22x faster                                                                  |
| tomli_loads          | 2.92 sec                                                     | 2.61 sec: 1.12x faster                                                                 |
| xml_etree_parse      | 160 ms                                                       | 144 ms: 1.11x faster                                                                   |
| xml_etree_generate   | 92.3 ms                                                      | 89.9 ms: 1.03x faster                                                                  |
| xml_etree_iterparse  | 110 ms                                                       | 112 ms: 1.02x slower                                                                   |
| unpickle_list        | 4.65 us                                                      | 4.75 us: 1.02x slower                                                                  |
| unpickle             | 13.5 us                                                      | 14.5 us: 1.07x slower                                                                  |
| pickle_list          | 4.12 us                                                      | 4.44 us: 1.08x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.7 us: 1.08x slower                                                                  |
| pickle_dict          | 29.5 us                                                      | 34.6 us: 1.17x slower                                                                  |
| Geometric mean       | (ref)                                                        | 1.09x faster                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| python_startup_no_site | 7.33 ms                                                      | 11.2 ms: 1.52x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 13.6 ms: 1.08x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 127 us: 4.23x faster                                                                   |
| asyncio_tcp              | 779 ms                                                       | 377 ms: 2.07x faster                                                                   |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.96x faster                                                                 |
| generators               | 57.3 ms                                                      | 34.2 ms: 1.68x faster                                                                  |
| logging_silent           | 167 ns                                                       | 100 ns: 1.67x faster                                                                   |
| raytrace                 | 489 ms                                                       | 298 ms: 1.64x faster                                                                   |
| async_tree_none          | 692 ms                                                       | 438 ms: 1.58x faster                                                                   |
| scimark_lu               | 167 ms                                                       | 106 ms: 1.58x faster                                                                   |
| sqlglot_parse            | 2.24 ms                                                      | 1.44 ms: 1.56x faster                                                                  |
| deltablue                | 7.50 ms                                                      | 4.88 ms: 1.54x faster                                                                  |
| richards_super           | 90.6 ms                                                      | 59.4 ms: 1.53x faster                                                                  |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                                 |
| async_tree_memoization   | 819 ms                                                       | 549 ms: 1.49x faster                                                                   |
| go                       | 262 ms                                                       | 177 ms: 1.48x faster                                                                   |
| chaos                    | 109 ms                                                       | 73.8 ms: 1.47x faster                                                                  |
| crypto_pyaes             | 119 ms                                                       | 81.8 ms: 1.46x faster                                                                  |
| pickle_pure_python       | 455 us                                                       | 314 us: 1.45x faster                                                                   |
| sqlglot_transpile        | 2.68 ms                                                      | 1.85 ms: 1.45x faster                                                                  |
| unpack_sequence          | 59.9 ns                                                      | 42.2 ns: 1.42x faster                                                                  |
| richards                 | 75.1 ms                                                      | 53.5 ms: 1.40x faster                                                                  |
| coroutines               | 30.3 ms                                                      | 22.2 ms: 1.37x faster                                                                  |
| unpickle_pure_python     | 312 us                                                       | 229 us: 1.36x faster                                                                   |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.34x faster                                                                  |
| logging_format           | 9.64 us                                                      | 7.20 us: 1.34x faster                                                                  |
| bench_mp_pool            | 6.37 ms                                                      | 4.78 ms: 1.33x faster                                                                  |
| logging_simple           | 8.88 us                                                      | 6.65 us: 1.33x faster                                                                  |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 702 ms: 1.33x faster                                                                   |
| scimark_monte_carlo      | 107 ms                                                       | 81.9 ms: 1.31x faster                                                                  |
| pyflate                  | 733 ms                                                       | 561 ms: 1.31x faster                                                                   |
| pycparser                | 1.67 sec                                                     | 1.35 sec: 1.24x faster                                                                 |
| xml_etree_process        | 75.9 ms                                                      | 61.6 ms: 1.23x faster                                                                  |
| tornado_http             | 157 ms                                                       | 129 ms: 1.22x faster                                                                   |
| json_loads               | 30.3 us                                                      | 24.9 us: 1.22x faster                                                                  |
| scimark_sor              | 180 ms                                                       | 148 ms: 1.22x faster                                                                   |
| deepcopy_memo            | 49.8 us                                                      | 41.3 us: 1.21x faster                                                                  |
| deepcopy                 | 468 us                                                       | 391 us: 1.20x faster                                                                   |
| sqlglot_normalize        | 144 ms                                                       | 122 ms: 1.18x faster                                                                   |
| nbody                    | 134 ms                                                       | 114 ms: 1.18x faster                                                                   |
| deepcopy_reduce          | 4.01 us                                                      | 3.44 us: 1.17x faster                                                                  |
| chameleon                | 9.44 ms                                                      | 8.09 ms: 1.17x faster                                                                  |
| float                    | 111 ms                                                       | 95.3 ms: 1.17x faster                                                                  |
| pprint_safe_repr         | 1.05 sec                                                     | 901 ms: 1.17x faster                                                                   |
| pprint_pformat           | 2.15 sec                                                     | 1.85 sec: 1.16x faster                                                                 |
| bench_thread_pool        | 1.14 ms                                                      | 985 us: 1.16x faster                                                                   |
| docutils                 | 3.41 sec                                                     | 2.95 sec: 1.16x faster                                                                 |
| comprehensions           | 26.7 us                                                      | 23.1 us: 1.15x faster                                                                  |
| mdp                      | 3.01 sec                                                     | 2.61 sec: 1.15x faster                                                                 |
| dask                     | 472 ms                                                       | 413 ms: 1.14x faster                                                                   |
| sympy_sum                | 193 ms                                                       | 170 ms: 1.13x faster                                                                   |
| 2to3                     | 350 ms                                                       | 309 ms: 1.13x faster                                                                   |
| sympy_integrate          | 28.2 ms                                                      | 25.0 ms: 1.13x faster                                                                  |
| regex_compile            | 190 ms                                                       | 169 ms: 1.12x faster                                                                   |
| async_generators         | 421 ms                                                       | 375 ms: 1.12x faster                                                                   |
| pathlib                  | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                                                  |
| tomli_loads              | 2.92 sec                                                     | 2.61 sec: 1.12x faster                                                                 |
| nqueens                  | 115 ms                                                       | 104 ms: 1.11x faster                                                                   |
| sympy_str                | 360 ms                                                       | 325 ms: 1.11x faster                                                                   |
| xml_etree_parse          | 160 ms                                                       | 144 ms: 1.11x faster                                                                   |
| sqlglot_optimize         | 70.1 ms                                                      | 63.4 ms: 1.11x faster                                                                  |
| json                     | 5.86 ms                                                      | 5.31 ms: 1.10x faster                                                                  |
| dulwich_log              | 81.1 ms                                                      | 73.5 ms: 1.10x faster                                                                  |
| sympy_expand             | 600 ms                                                       | 547 ms: 1.10x faster                                                                   |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                                                  |
| mako                     | 14.7 ms                                                      | 13.6 ms: 1.08x faster                                                                  |
| fannkuch                 | 483 ms                                                       | 446 ms: 1.08x faster                                                                   |
| sqlite_synth             | 2.99 us                                                      | 2.81 us: 1.07x faster                                                                  |
| hexiom                   | 9.42 ms                                                      | 8.91 ms: 1.06x faster                                                                  |
| regex_dna                | 261 ms                                                       | 251 ms: 1.04x faster                                                                   |
| regex_v8                 | 27.2 ms                                                      | 26.3 ms: 1.03x faster                                                                  |
| xml_etree_generate       | 92.3 ms                                                      | 89.9 ms: 1.03x faster                                                                  |
| asyncio_websockets       | 390 ms                                                       | 380 ms: 1.03x faster                                                                   |
| pidigits                 | 271 ms                                                       | 264 ms: 1.02x faster                                                                   |
| meteor_contest           | 138 ms                                                       | 137 ms: 1.01x faster                                                                   |
| xml_etree_iterparse      | 110 ms                                                       | 112 ms: 1.02x slower                                                                   |
| unpickle_list            | 4.65 us                                                      | 4.75 us: 1.02x slower                                                                  |
| spectral_norm            | 139 ms                                                       | 144 ms: 1.03x slower                                                                   |
| gc_traversal             | 3.42 ms                                                      | 3.56 ms: 1.04x slower                                                                  |
| unpickle                 | 13.5 us                                                      | 14.5 us: 1.07x slower                                                                  |
| pickle_list              | 4.12 us                                                      | 4.44 us: 1.08x slower                                                                  |
| pickle                   | 9.89 us                                                      | 10.7 us: 1.08x slower                                                                  |
| scimark_fft              | 361 ms                                                       | 396 ms: 1.10x slower                                                                   |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| telco                    | 7.23 ms                                                      | 8.27 ms: 1.14x slower                                                                  |
| regex_effbot             | 3.09 ms                                                      | 3.57 ms: 1.16x slower                                                                  |
| pickle_dict              | 29.5 us                                                      | 34.6 us: 1.17x slower                                                                  |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.10 ms: 1.20x slower                                                                  |
| coverage                 | 63.3 ms                                                      | 79.3 ms: 1.25x slower                                                                  |
| python_startup_no_site   | 7.33 ms                                                      | 11.2 ms: 1.52x slower                                                                  |
| Geometric mean           | (ref)                                                        | 1.20x faster                                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240128-3.13.0a3+-d226882-PYTHON_UOPS/bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.07x