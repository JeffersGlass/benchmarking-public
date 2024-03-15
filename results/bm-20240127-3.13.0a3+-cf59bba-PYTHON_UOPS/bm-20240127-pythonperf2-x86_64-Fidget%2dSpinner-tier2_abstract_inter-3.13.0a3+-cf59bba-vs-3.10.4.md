
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.20x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 310 ms: 1.13x faster                                                                   |
| chameleon      | 9.44 ms                                                      | 7.83 ms: 1.21x faster                                                                  |
| docutils       | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                                 |
| tornado_http   | 157 ms                                                       | 127 ms: 1.23x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.18x faster                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 441 ms: 1.57x faster                                                                   |
| async_tree_memoization  | 819 ms                                                       | 554 ms: 1.48x faster                                                                   |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                                 |
| async_tree_cpu_io_mixed | 936 ms                                                       | 705 ms: 1.33x faster                                                                   |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 112 ms: 1.20x faster                                                                   |
| float          | 111 ms                                                       | 94.0 ms: 1.18x faster                                                                  |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.13x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 167 ms: 1.13x faster                                                                   |
| regex_dna      | 261 ms                                                       | 241 ms: 1.08x faster                                                                   |
| regex_v8       | 27.2 ms                                                      | 25.4 ms: 1.07x faster                                                                  |
| regex_effbot   | 3.09 ms                                                      | 3.47 ms: 1.12x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 314 us: 1.45x faster                                                                   |
| json_dumps           | 14.5 ms                                                      | 10.9 ms: 1.33x faster                                                                  |
| unpickle_pure_python | 312 us                                                       | 241 us: 1.29x faster                                                                   |
| xml_etree_process    | 75.9 ms                                                      | 61.6 ms: 1.23x faster                                                                  |
| json_loads           | 30.3 us                                                      | 24.8 us: 1.23x faster                                                                  |
| tomli_loads          | 2.92 sec                                                     | 2.60 sec: 1.12x faster                                                                 |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                                   |
| xml_etree_generate   | 92.3 ms                                                      | 90.0 ms: 1.03x faster                                                                  |
| unpickle_list        | 4.65 us                                                      | 4.74 us: 1.02x slower                                                                  |
| xml_etree_iterparse  | 110 ms                                                       | 114 ms: 1.04x slower                                                                   |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                                  |
| pickle_list          | 4.12 us                                                      | 4.52 us: 1.10x slower                                                                  |
| pickle_dict          | 29.5 us                                                      | 32.8 us: 1.11x slower                                                                  |
| unpickle             | 13.5 us                                                      | 15.1 us: 1.12x slower                                                                  |
| Geometric mean       | (ref)                                                        | 1.08x faster                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| python_startup_no_site | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 13.3 ms: 1.10x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 126 us: 4.25x faster                                                                   |
| asyncio_tcp              | 779 ms                                                       | 373 ms: 2.09x faster                                                                   |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                                 |
| logging_silent           | 167 ns                                                       | 99.6 ns: 1.68x faster                                                                  |
| generators               | 57.3 ms                                                      | 34.2 ms: 1.68x faster                                                                  |
| raytrace                 | 489 ms                                                       | 298 ms: 1.64x faster                                                                   |
| scimark_lu               | 167 ms                                                       | 104 ms: 1.60x faster                                                                   |
| sqlglot_parse            | 2.24 ms                                                      | 1.41 ms: 1.59x faster                                                                  |
| async_tree_none          | 692 ms                                                       | 441 ms: 1.57x faster                                                                   |
| deltablue                | 7.50 ms                                                      | 4.86 ms: 1.54x faster                                                                  |
| richards_super           | 90.6 ms                                                      | 59.1 ms: 1.53x faster                                                                  |
| chaos                    | 109 ms                                                       | 72.8 ms: 1.49x faster                                                                  |
| crypto_pyaes             | 119 ms                                                       | 80.5 ms: 1.48x faster                                                                  |
| async_tree_memoization   | 819 ms                                                       | 554 ms: 1.48x faster                                                                   |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                                 |
| sqlglot_transpile        | 2.68 ms                                                      | 1.82 ms: 1.47x faster                                                                  |
| go                       | 262 ms                                                       | 180 ms: 1.46x faster                                                                   |
| pickle_pure_python       | 455 us                                                       | 314 us: 1.45x faster                                                                   |
| richards                 | 75.1 ms                                                      | 53.5 ms: 1.40x faster                                                                  |
| bench_mp_pool            | 6.37 ms                                                      | 4.61 ms: 1.38x faster                                                                  |
| coroutines               | 30.3 ms                                                      | 22.0 ms: 1.38x faster                                                                  |
| json_dumps               | 14.5 ms                                                      | 10.9 ms: 1.33x faster                                                                  |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 705 ms: 1.33x faster                                                                   |
| scimark_monte_carlo      | 107 ms                                                       | 81.1 ms: 1.33x faster                                                                  |
| unpickle_pure_python     | 312 us                                                       | 241 us: 1.29x faster                                                                   |
| unpack_sequence          | 59.9 ns                                                      | 46.5 ns: 1.29x faster                                                                  |
| logging_format           | 9.64 us                                                      | 7.50 us: 1.28x faster                                                                  |
| pyflate                  | 733 ms                                                       | 576 ms: 1.27x faster                                                                   |
| logging_simple           | 8.88 us                                                      | 6.98 us: 1.27x faster                                                                  |
| scimark_sor              | 180 ms                                                       | 143 ms: 1.26x faster                                                                   |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                                 |
| tornado_http             | 157 ms                                                       | 127 ms: 1.23x faster                                                                   |
| xml_etree_process        | 75.9 ms                                                      | 61.6 ms: 1.23x faster                                                                  |
| json_loads               | 30.3 us                                                      | 24.8 us: 1.23x faster                                                                  |
| deepcopy                 | 468 us                                                       | 383 us: 1.22x faster                                                                   |
| deepcopy_memo            | 49.8 us                                                      | 40.7 us: 1.22x faster                                                                  |
| chameleon                | 9.44 ms                                                      | 7.83 ms: 1.21x faster                                                                  |
| nbody                    | 134 ms                                                       | 112 ms: 1.20x faster                                                                   |
| float                    | 111 ms                                                       | 94.0 ms: 1.18x faster                                                                  |
| sqlglot_normalize        | 144 ms                                                       | 122 ms: 1.18x faster                                                                   |
| deepcopy_reduce          | 4.01 us                                                      | 3.42 us: 1.17x faster                                                                  |
| pprint_safe_repr         | 1.05 sec                                                     | 901 ms: 1.17x faster                                                                   |
| docutils                 | 3.41 sec                                                     | 2.93 sec: 1.16x faster                                                                 |
| pprint_pformat           | 2.15 sec                                                     | 1.85 sec: 1.16x faster                                                                 |
| comprehensions           | 26.7 us                                                      | 23.0 us: 1.16x faster                                                                  |
| bench_thread_pool        | 1.14 ms                                                      | 985 us: 1.16x faster                                                                   |
| mdp                      | 3.01 sec                                                     | 2.60 sec: 1.16x faster                                                                 |
| sympy_sum                | 193 ms                                                       | 167 ms: 1.15x faster                                                                   |
| dask                     | 472 ms                                                       | 410 ms: 1.15x faster                                                                   |
| sympy_integrate          | 28.2 ms                                                      | 24.7 ms: 1.14x faster                                                                  |
| regex_compile            | 190 ms                                                       | 167 ms: 1.13x faster                                                                   |
| 2to3                     | 350 ms                                                       | 310 ms: 1.13x faster                                                                   |
| dulwich_log              | 81.1 ms                                                      | 72.0 ms: 1.13x faster                                                                  |
| nqueens                  | 115 ms                                                       | 102 ms: 1.13x faster                                                                   |
| async_generators         | 421 ms                                                       | 374 ms: 1.13x faster                                                                   |
| sympy_str                | 360 ms                                                       | 320 ms: 1.12x faster                                                                   |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.12x faster                                                                  |
| tomli_loads              | 2.92 sec                                                     | 2.60 sec: 1.12x faster                                                                 |
| sympy_expand             | 600 ms                                                       | 537 ms: 1.12x faster                                                                   |
| json                     | 5.86 ms                                                      | 5.25 ms: 1.12x faster                                                                  |
| sqlglot_optimize         | 70.1 ms                                                      | 63.3 ms: 1.11x faster                                                                  |
| mako                     | 14.7 ms                                                      | 13.3 ms: 1.10x faster                                                                  |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                                                  |
| fannkuch                 | 483 ms                                                       | 445 ms: 1.09x faster                                                                   |
| regex_dna                | 261 ms                                                       | 241 ms: 1.08x faster                                                                   |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                                   |
| sqlite_synth             | 2.99 us                                                      | 2.80 us: 1.07x faster                                                                  |
| regex_v8                 | 27.2 ms                                                      | 25.4 ms: 1.07x faster                                                                  |
| hexiom                   | 9.42 ms                                                      | 9.05 ms: 1.04x faster                                                                  |
| xml_etree_generate       | 92.3 ms                                                      | 90.0 ms: 1.03x faster                                                                  |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                                                   |
| meteor_contest           | 138 ms                                                       | 136 ms: 1.02x faster                                                                   |
| asyncio_websockets       | 390 ms                                                       | 385 ms: 1.01x faster                                                                   |
| spectral_norm            | 139 ms                                                       | 138 ms: 1.01x faster                                                                   |
| unpickle_list            | 4.65 us                                                      | 4.74 us: 1.02x slower                                                                  |
| gc_traversal             | 3.42 ms                                                      | 3.53 ms: 1.03x slower                                                                  |
| xml_etree_iterparse      | 110 ms                                                       | 114 ms: 1.04x slower                                                                   |
| pickle                   | 9.89 us                                                      | 10.6 us: 1.07x slower                                                                  |
| scimark_fft              | 361 ms                                                       | 392 ms: 1.08x slower                                                                   |
| pickle_list              | 4.12 us                                                      | 4.52 us: 1.10x slower                                                                  |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.11x slower                                                                  |
| pickle_dict              | 29.5 us                                                      | 32.8 us: 1.11x slower                                                                  |
| unpickle                 | 13.5 us                                                      | 15.1 us: 1.12x slower                                                                  |
| regex_effbot             | 3.09 ms                                                      | 3.47 ms: 1.12x slower                                                                  |
| telco                    | 7.23 ms                                                      | 8.29 ms: 1.15x slower                                                                  |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.01 ms: 1.18x slower                                                                  |
| coverage                 | 63.3 ms                                                      | 80.4 ms: 1.27x slower                                                                  |
| python_startup_no_site   | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                                  |
| Geometric mean           | (ref)                                                        | 1.20x faster                                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-cf59bba-PYTHON_UOPS/bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.09x