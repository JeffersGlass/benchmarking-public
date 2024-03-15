
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.39x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 316 ms: 1.11x faster                                                                   |
| chameleon      | 9.44 ms                                                      | 8.17 ms: 1.16x faster                                                                  |
| docutils       | 3.41 sec                                                     | 2.92 sec: 1.17x faster                                                                 |
| tornado_http   | 157 ms                                                       | 123 ms: 1.27x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.17x faster                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 444 ms: 1.56x faster                                                                   |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                                 |
| async_tree_memoization  | 819 ms                                                       | 560 ms: 1.46x faster                                                                   |
| async_tree_cpu_io_mixed | 936 ms                                                       | 713 ms: 1.31x faster                                                                   |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 105 ms: 1.06x faster                                                                   |
| pidigits       | 271 ms                                                       | 266 ms: 1.02x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                           |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 171 ms: 1.11x faster                                                                   |
| regex_dna      | 261 ms                                                       | 240 ms: 1.09x faster                                                                   |
| regex_v8       | 27.2 ms                                                      | 26.0 ms: 1.04x faster                                                                  |
| regex_effbot   | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 310 us: 1.47x faster                                                                   |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                                  |
| unpickle_pure_python | 312 us                                                       | 242 us: 1.29x faster                                                                   |
| xml_etree_process    | 75.9 ms                                                      | 62.0 ms: 1.23x faster                                                                  |
| json_loads           | 30.3 us                                                      | 24.8 us: 1.22x faster                                                                  |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                                   |
| tomli_loads          | 2.92 sec                                                     | 2.83 sec: 1.03x faster                                                                 |
| xml_etree_generate   | 92.3 ms                                                      | 91.7 ms: 1.01x faster                                                                  |
| unpickle_list        | 4.65 us                                                      | 4.69 us: 1.01x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| xml_etree_iterparse  | 110 ms                                                       | 118 ms: 1.06x slower                                                                   |
| pickle_list          | 4.12 us                                                      | 4.43 us: 1.08x slower                                                                  |
| unpickle             | 13.5 us                                                      | 14.8 us: 1.10x slower                                                                  |
| pickle_dict          | 29.5 us                                                      | 32.4 us: 1.10x slower                                                                  |
| Geometric mean       | (ref)                                                        | 1.08x faster                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                           |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 128 us: 4.20x faster                                                                   |
| asyncio_tcp              | 779 ms                                                       | 377 ms: 2.07x faster                                                                   |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                                 |
| generators               | 57.3 ms                                                      | 33.9 ms: 1.69x faster                                                                  |
| logging_silent           | 167 ns                                                       | 99.8 ns: 1.68x faster                                                                  |
| raytrace                 | 489 ms                                                       | 304 ms: 1.61x faster                                                                   |
| scimark_lu               | 167 ms                                                       | 105 ms: 1.58x faster                                                                   |
| async_tree_none          | 692 ms                                                       | 444 ms: 1.56x faster                                                                   |
| sqlglot_parse            | 2.24 ms                                                      | 1.44 ms: 1.56x faster                                                                  |
| richards_super           | 90.6 ms                                                      | 61.1 ms: 1.48x faster                                                                  |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                                 |
| pickle_pure_python       | 455 us                                                       | 310 us: 1.47x faster                                                                   |
| async_tree_memoization   | 819 ms                                                       | 560 ms: 1.46x faster                                                                   |
| sqlglot_transpile        | 2.68 ms                                                      | 1.85 ms: 1.45x faster                                                                  |
| go                       | 262 ms                                                       | 185 ms: 1.41x faster                                                                   |
| chaos                    | 109 ms                                                       | 77.9 ms: 1.39x faster                                                                  |
| crypto_pyaes             | 119 ms                                                       | 86.6 ms: 1.38x faster                                                                  |
| richards                 | 75.1 ms                                                      | 54.7 ms: 1.37x faster                                                                  |
| deltablue                | 7.50 ms                                                      | 5.50 ms: 1.36x faster                                                                  |
| coroutines               | 30.3 ms                                                      | 22.2 ms: 1.36x faster                                                                  |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                                  |
| bench_mp_pool            | 6.37 ms                                                      | 4.82 ms: 1.32x faster                                                                  |
| unpack_sequence          | 59.9 ns                                                      | 45.5 ns: 1.32x faster                                                                  |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 713 ms: 1.31x faster                                                                   |
| logging_format           | 9.64 us                                                      | 7.42 us: 1.30x faster                                                                  |
| unpickle_pure_python     | 312 us                                                       | 242 us: 1.29x faster                                                                   |
| logging_simple           | 8.88 us                                                      | 6.94 us: 1.28x faster                                                                  |
| tornado_http             | 157 ms                                                       | 123 ms: 1.27x faster                                                                   |
| pyflate                  | 733 ms                                                       | 588 ms: 1.25x faster                                                                   |
| scimark_sor              | 180 ms                                                       | 146 ms: 1.24x faster                                                                   |
| pycparser                | 1.67 sec                                                     | 1.36 sec: 1.23x faster                                                                 |
| xml_etree_process        | 75.9 ms                                                      | 62.0 ms: 1.23x faster                                                                  |
| json_loads               | 30.3 us                                                      | 24.8 us: 1.22x faster                                                                  |
| deepcopy                 | 468 us                                                       | 384 us: 1.22x faster                                                                   |
| deepcopy_memo            | 49.8 us                                                      | 40.9 us: 1.22x faster                                                                  |
| scimark_monte_carlo      | 107 ms                                                       | 90.4 ms: 1.19x faster                                                                  |
| bench_thread_pool        | 1.14 ms                                                      | 968 us: 1.18x faster                                                                   |
| deepcopy_reduce          | 4.01 us                                                      | 3.41 us: 1.18x faster                                                                  |
| docutils                 | 3.41 sec                                                     | 2.92 sec: 1.17x faster                                                                 |
| dask                     | 472 ms                                                       | 407 ms: 1.16x faster                                                                   |
| sqlglot_normalize        | 144 ms                                                       | 124 ms: 1.16x faster                                                                   |
| chameleon                | 9.44 ms                                                      | 8.17 ms: 1.16x faster                                                                  |
| sympy_sum                | 193 ms                                                       | 169 ms: 1.14x faster                                                                   |
| pprint_safe_repr         | 1.05 sec                                                     | 920 ms: 1.14x faster                                                                   |
| async_generators         | 421 ms                                                       | 370 ms: 1.14x faster                                                                   |
| pprint_pformat           | 2.15 sec                                                     | 1.90 sec: 1.13x faster                                                                 |
| dulwich_log              | 81.1 ms                                                      | 71.9 ms: 1.13x faster                                                                  |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.12x faster                                                                  |
| sympy_expand             | 600 ms                                                       | 535 ms: 1.12x faster                                                                   |
| sympy_integrate          | 28.2 ms                                                      | 25.1 ms: 1.12x faster                                                                  |
| mdp                      | 3.01 sec                                                     | 2.69 sec: 1.12x faster                                                                 |
| create_gc_cycles         | 1.76 ms                                                      | 1.58 ms: 1.12x faster                                                                  |
| sympy_str                | 360 ms                                                       | 324 ms: 1.11x faster                                                                   |
| json                     | 5.86 ms                                                      | 5.28 ms: 1.11x faster                                                                  |
| regex_compile            | 190 ms                                                       | 171 ms: 1.11x faster                                                                   |
| 2to3                     | 350 ms                                                       | 316 ms: 1.11x faster                                                                   |
| sqlglot_optimize         | 70.1 ms                                                      | 64.2 ms: 1.09x faster                                                                  |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                                   |
| regex_dna                | 261 ms                                                       | 240 ms: 1.09x faster                                                                   |
| sqlite_synth             | 2.99 us                                                      | 2.82 us: 1.06x faster                                                                  |
| float                    | 111 ms                                                       | 105 ms: 1.06x faster                                                                   |
| regex_v8                 | 27.2 ms                                                      | 26.0 ms: 1.04x faster                                                                  |
| comprehensions           | 26.7 us                                                      | 25.7 us: 1.04x faster                                                                  |
| nqueens                  | 115 ms                                                       | 111 ms: 1.04x faster                                                                   |
| asyncio_websockets       | 390 ms                                                       | 376 ms: 1.04x faster                                                                   |
| tomli_loads              | 2.92 sec                                                     | 2.83 sec: 1.03x faster                                                                 |
| pidigits                 | 271 ms                                                       | 266 ms: 1.02x faster                                                                   |
| fannkuch                 | 483 ms                                                       | 478 ms: 1.01x faster                                                                   |
| xml_etree_generate       | 92.3 ms                                                      | 91.7 ms: 1.01x faster                                                                  |
| meteor_contest           | 138 ms                                                       | 138 ms: 1.00x faster                                                                   |
| unpickle_list            | 4.65 us                                                      | 4.69 us: 1.01x slower                                                                  |
| gc_traversal             | 3.42 ms                                                      | 3.52 ms: 1.03x slower                                                                  |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| hexiom                   | 9.42 ms                                                      | 9.90 ms: 1.05x slower                                                                  |
| xml_etree_iterparse      | 110 ms                                                       | 118 ms: 1.06x slower                                                                   |
| pickle_list              | 4.12 us                                                      | 4.43 us: 1.08x slower                                                                  |
| spectral_norm            | 139 ms                                                       | 152 ms: 1.09x slower                                                                   |
| unpickle                 | 13.5 us                                                      | 14.8 us: 1.10x slower                                                                  |
| pickle_dict              | 29.5 us                                                      | 32.4 us: 1.10x slower                                                                  |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| regex_effbot             | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                                  |
| scimark_fft              | 361 ms                                                       | 424 ms: 1.17x slower                                                                   |
| telco                    | 7.23 ms                                                      | 8.54 ms: 1.18x slower                                                                  |
| coverage                 | 63.3 ms                                                      | 80.2 ms: 1.27x slower                                                                  |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.58 ms: 1.30x slower                                                                  |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                                  |
| Geometric mean           | (ref)                                                        | 1.18x faster                                                                           |

Benchmark hidden because not significant (3): mypy2, nbody, mako
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-27ce303-PYTHON_UOPS/bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.39x