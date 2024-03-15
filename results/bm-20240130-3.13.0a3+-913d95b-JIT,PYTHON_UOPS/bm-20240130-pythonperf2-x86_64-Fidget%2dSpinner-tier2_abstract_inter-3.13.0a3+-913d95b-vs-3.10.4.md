
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.12x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 303 ms: 1.16x faster                                                                   |
| chameleon      | 9.44 ms                                                      | 7.67 ms: 1.23x faster                                                                  |
| docutils       | 3.41 sec                                                     | 2.90 sec: 1.18x faster                                                                 |
| tornado_http   | 157 ms                                                       | 126 ms: 1.24x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.20x faster                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 434 ms: 1.59x faster                                                                   |
| async_tree_memoization  | 819 ms                                                       | 545 ms: 1.50x faster                                                                   |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                                 |
| async_tree_cpu_io_mixed | 936 ms                                                       | 700 ms: 1.34x faster                                                                   |
| Geometric mean          | (ref)                                                        | 1.48x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 82.1 ms: 1.35x faster                                                                  |
| nbody          | 134 ms                                                       | 104 ms: 1.29x faster                                                                   |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.21x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 147 ms: 1.29x faster                                                                   |
| regex_dna      | 261 ms                                                       | 241 ms: 1.08x faster                                                                   |
| regex_v8       | 27.2 ms                                                      | 25.6 ms: 1.06x faster                                                                  |
| regex_effbot   | 3.09 ms                                                      | 3.59 ms: 1.16x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 304 us: 1.50x faster                                                                   |
| unpickle_pure_python | 312 us                                                       | 224 us: 1.39x faster                                                                   |
| json_dumps           | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                                  |
| xml_etree_process    | 75.9 ms                                                      | 58.6 ms: 1.30x faster                                                                  |
| tomli_loads          | 2.92 sec                                                     | 2.34 sec: 1.24x faster                                                                 |
| json_loads           | 30.3 us                                                      | 25.3 us: 1.20x faster                                                                  |
| xml_etree_generate   | 92.3 ms                                                      | 85.1 ms: 1.08x faster                                                                  |
| xml_etree_parse      | 160 ms                                                       | 149 ms: 1.07x faster                                                                   |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.04x faster                                                                   |
| pickle_dict          | 29.5 us                                                      | 31.0 us: 1.05x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| pickle_list          | 4.12 us                                                      | 4.37 us: 1.06x slower                                                                  |
| unpickle_list        | 4.65 us                                                      | 4.95 us: 1.07x slower                                                                  |
| unpickle             | 13.5 us                                                      | 15.3 us: 1.13x slower                                                                  |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| python_startup_no_site | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.8 ms: 1.25x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 122 us: 4.41x faster                                                                   |
| asyncio_tcp              | 779 ms                                                       | 370 ms: 2.10x faster                                                                   |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                                 |
| deltablue                | 7.50 ms                                                      | 3.94 ms: 1.90x faster                                                                  |
| raytrace                 | 489 ms                                                       | 277 ms: 1.77x faster                                                                   |
| logging_silent           | 167 ns                                                       | 95.6 ns: 1.75x faster                                                                  |
| generators               | 57.3 ms                                                      | 34.4 ms: 1.66x faster                                                                  |
| scimark_lu               | 167 ms                                                       | 101 ms: 1.66x faster                                                                   |
| sqlglot_parse            | 2.24 ms                                                      | 1.38 ms: 1.62x faster                                                                  |
| async_tree_none          | 692 ms                                                       | 434 ms: 1.59x faster                                                                   |
| richards_super           | 90.6 ms                                                      | 57.4 ms: 1.58x faster                                                                  |
| chaos                    | 109 ms                                                       | 69.8 ms: 1.55x faster                                                                  |
| go                       | 262 ms                                                       | 168 ms: 1.55x faster                                                                   |
| async_tree_memoization   | 819 ms                                                       | 545 ms: 1.50x faster                                                                   |
| sqlglot_transpile        | 2.68 ms                                                      | 1.79 ms: 1.50x faster                                                                  |
| pickle_pure_python       | 455 us                                                       | 304 us: 1.50x faster                                                                   |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                                 |
| richards                 | 75.1 ms                                                      | 51.0 ms: 1.47x faster                                                                  |
| crypto_pyaes             | 119 ms                                                       | 82.1 ms: 1.45x faster                                                                  |
| pyflate                  | 733 ms                                                       | 517 ms: 1.42x faster                                                                   |
| unpickle_pure_python     | 312 us                                                       | 224 us: 1.39x faster                                                                   |
| unpack_sequence          | 59.9 ns                                                      | 43.7 ns: 1.37x faster                                                                  |
| scimark_monte_carlo      | 107 ms                                                       | 79.0 ms: 1.36x faster                                                                  |
| json_dumps               | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                                  |
| float                    | 111 ms                                                       | 82.1 ms: 1.35x faster                                                                  |
| coroutines               | 30.3 ms                                                      | 22.5 ms: 1.35x faster                                                                  |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 700 ms: 1.34x faster                                                                   |
| logging_simple           | 8.88 us                                                      | 6.65 us: 1.34x faster                                                                  |
| deepcopy_memo            | 49.8 us                                                      | 37.5 us: 1.33x faster                                                                  |
| pycparser                | 1.67 sec                                                     | 1.27 sec: 1.31x faster                                                                 |
| xml_etree_process        | 75.9 ms                                                      | 58.6 ms: 1.30x faster                                                                  |
| regex_compile            | 190 ms                                                       | 147 ms: 1.29x faster                                                                   |
| logging_format           | 9.64 us                                                      | 7.46 us: 1.29x faster                                                                  |
| deepcopy                 | 468 us                                                       | 363 us: 1.29x faster                                                                   |
| nbody                    | 134 ms                                                       | 104 ms: 1.29x faster                                                                   |
| comprehensions           | 26.7 us                                                      | 20.8 us: 1.28x faster                                                                  |
| bench_mp_pool            | 6.37 ms                                                      | 5.00 ms: 1.27x faster                                                                  |
| scimark_sor              | 180 ms                                                       | 143 ms: 1.26x faster                                                                   |
| mako                     | 14.7 ms                                                      | 11.8 ms: 1.25x faster                                                                  |
| tomli_loads              | 2.92 sec                                                     | 2.34 sec: 1.24x faster                                                                 |
| tornado_http             | 157 ms                                                       | 126 ms: 1.24x faster                                                                   |
| chameleon                | 9.44 ms                                                      | 7.67 ms: 1.23x faster                                                                  |
| deepcopy_reduce          | 4.01 us                                                      | 3.28 us: 1.22x faster                                                                  |
| pprint_safe_repr         | 1.05 sec                                                     | 860 ms: 1.22x faster                                                                   |
| pprint_pformat           | 2.15 sec                                                     | 1.78 sec: 1.21x faster                                                                 |
| json_loads               | 30.3 us                                                      | 25.3 us: 1.20x faster                                                                  |
| spectral_norm            | 139 ms                                                       | 116 ms: 1.20x faster                                                                   |
| sqlglot_normalize        | 144 ms                                                       | 121 ms: 1.19x faster                                                                   |
| sympy_str                | 360 ms                                                       | 304 ms: 1.19x faster                                                                   |
| sympy_sum                | 193 ms                                                       | 163 ms: 1.18x faster                                                                   |
| mdp                      | 3.01 sec                                                     | 2.55 sec: 1.18x faster                                                                 |
| sympy_expand             | 600 ms                                                       | 509 ms: 1.18x faster                                                                   |
| docutils                 | 3.41 sec                                                     | 2.90 sec: 1.18x faster                                                                 |
| hexiom                   | 9.42 ms                                                      | 8.04 ms: 1.17x faster                                                                  |
| nqueens                  | 115 ms                                                       | 98.4 ms: 1.17x faster                                                                  |
| bench_thread_pool        | 1.14 ms                                                      | 982 us: 1.16x faster                                                                   |
| pathlib                  | 21.4 ms                                                      | 18.4 ms: 1.16x faster                                                                  |
| 2to3                     | 350 ms                                                       | 303 ms: 1.16x faster                                                                   |
| create_gc_cycles         | 1.76 ms                                                      | 1.52 ms: 1.16x faster                                                                  |
| dask                     | 472 ms                                                       | 409 ms: 1.16x faster                                                                   |
| dulwich_log              | 81.1 ms                                                      | 70.4 ms: 1.15x faster                                                                  |
| sympy_integrate          | 28.2 ms                                                      | 24.5 ms: 1.15x faster                                                                  |
| async_generators         | 421 ms                                                       | 368 ms: 1.14x faster                                                                   |
| sqlglot_optimize         | 70.1 ms                                                      | 62.1 ms: 1.13x faster                                                                  |
| fannkuch                 | 483 ms                                                       | 430 ms: 1.12x faster                                                                   |
| json                     | 5.86 ms                                                      | 5.36 ms: 1.09x faster                                                                  |
| xml_etree_generate       | 92.3 ms                                                      | 85.1 ms: 1.08x faster                                                                  |
| regex_dna                | 261 ms                                                       | 241 ms: 1.08x faster                                                                   |
| sqlite_synth             | 2.99 us                                                      | 2.78 us: 1.07x faster                                                                  |
| xml_etree_parse          | 160 ms                                                       | 149 ms: 1.07x faster                                                                   |
| regex_v8                 | 27.2 ms                                                      | 25.6 ms: 1.06x faster                                                                  |
| meteor_contest           | 138 ms                                                       | 134 ms: 1.04x faster                                                                   |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.04x faster                                                                   |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                                   |
| asyncio_websockets       | 390 ms                                                       | 383 ms: 1.02x faster                                                                   |
| scimark_fft              | 361 ms                                                       | 359 ms: 1.01x faster                                                                   |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.22 ms: 1.03x slower                                                                  |
| pickle_dict              | 29.5 us                                                      | 31.0 us: 1.05x slower                                                                  |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| pickle_list              | 4.12 us                                                      | 4.37 us: 1.06x slower                                                                  |
| unpickle_list            | 4.65 us                                                      | 4.95 us: 1.07x slower                                                                  |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| unpickle                 | 13.5 us                                                      | 15.3 us: 1.13x slower                                                                  |
| telco                    | 7.23 ms                                                      | 8.22 ms: 1.14x slower                                                                  |
| regex_effbot             | 3.09 ms                                                      | 3.59 ms: 1.16x slower                                                                  |
| coverage                 | 63.3 ms                                                      | 80.7 ms: 1.27x slower                                                                  |
| python_startup_no_site   | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                                  |
| Geometric mean           | (ref)                                                        | 1.24x faster                                                                           |

Benchmark hidden because not significant (2): mypy2, gc_traversal
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240130-3.13.0a3+-913d95b-JIT,PYTHON_UOPS/bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.12x