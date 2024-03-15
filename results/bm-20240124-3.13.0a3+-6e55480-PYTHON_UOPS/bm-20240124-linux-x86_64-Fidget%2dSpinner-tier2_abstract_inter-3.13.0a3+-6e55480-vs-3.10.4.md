
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 6e55480
- commit date: 2024-01-24
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 286 ms: 1.22x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.33 ms: 1.32x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 99.2 ms: 1.37x faster                                                            |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 447 ms: 1.63x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 571 ms: 1.52x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 110 ms: 1.40x faster                                                             |
| float          | 117 ms                                                 | 87.8 ms: 1.33x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.24x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.7 ms: 1.12x faster                                                            |
| regex_dna      | 227 ms                                                 | 223 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.09x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.61x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 235 us: 1.41x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.8 ms: 1.30x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.47 sec: 1.27x faster                                                           |
| xml_etree_generate   | 99.4 ms                                                | 88.5 ms: 1.12x faster                                                            |
| json_loads           | 31.2 us                                                | 28.8 us: 1.08x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpickle_list        | 5.20 us                                                | 5.31 us: 1.02x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.24 us: 1.03x slower                                                            |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                                            |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.3 ms: 1.23x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.67x faster                                                             |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 469 ms: 1.96x faster                                                             |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                                             |
| deltablue                | 7.91 ms                                                | 4.42 ms: 1.79x faster                                                            |
| scimark_sor              | 220 ms                                                 | 125 ms: 1.75x faster                                                             |
| richards_super           | 94.7 ms                                                | 54.5 ms: 1.74x faster                                                            |
| raytrace                 | 507 ms                                                 | 297 ms: 1.71x faster                                                             |
| richards                 | 79.3 ms                                                | 48.2 ms: 1.64x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.64x faster                                                            |
| chaos                    | 115 ms                                                 | 70.5 ms: 1.64x faster                                                            |
| async_tree_none          | 728 ms                                                 | 447 ms: 1.63x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.61x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.58x faster                                                            |
| go                       | 240 ms                                                 | 153 ms: 1.57x faster                                                             |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 82.3 ms: 1.55x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 39.0 ns: 1.54x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 571 ms: 1.52x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 78.8 ms: 1.50x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.48x faster                                                             |
| deepcopy_memo            | 58.5 us                                                | 40.6 us: 1.44x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 235 us: 1.41x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.5 us: 1.41x faster                                                            |
| nbody                    | 154 ms                                                 | 110 ms: 1.40x faster                                                             |
| pyflate                  | 716 ms                                                 | 516 ms: 1.39x faster                                                             |
| tornado_http             | 136 ms                                                 | 99.2 ms: 1.37x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.06 us: 1.37x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| float                    | 117 ms                                                 | 87.8 ms: 1.33x faster                                                            |
| deepcopy                 | 479 us                                                 | 360 us: 1.33x faster                                                             |
| logging_format           | 9.09 us                                                | 6.86 us: 1.33x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.33 ms: 1.32x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.17 us: 1.31x faster                                                            |
| hexiom                   | 10.4 ms                                                | 7.97 ms: 1.30x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 60.8 ms: 1.30x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.47 sec: 1.27x faster                                                           |
| regex_compile            | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.67 sec: 1.26x faster                                                           |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                                           |
| pprint_safe_repr         | 1.02 sec                                               | 811 ms: 1.26x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.25x faster                                                             |
| spectral_norm            | 170 ms                                                 | 136 ms: 1.25x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.24x faster                                                            |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| mako                     | 16.3 ms                                                | 13.3 ms: 1.23x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 68.8 ms: 1.23x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| 2to3                     | 348 ms                                                 | 286 ms: 1.22x faster                                                             |
| fannkuch                 | 532 ms                                                 | 437 ms: 1.22x faster                                                             |
| sympy_str                | 346 ms                                                 | 288 ms: 1.20x faster                                                             |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 57.8 ms: 1.20x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 842 us: 1.17x faster                                                             |
| nqueens                  | 106 ms                                                 | 90.5 ms: 1.17x faster                                                            |
| sympy_expand             | 566 ms                                                 | 485 ms: 1.17x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.57 ms: 1.16x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 88.5 ms: 1.12x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 24.7 ms: 1.12x faster                                                            |
| scimark_fft              | 466 ms                                                 | 419 ms: 1.11x faster                                                             |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                            |
| json                     | 5.69 ms                                                | 5.20 ms: 1.09x faster                                                            |
| json_loads               | 31.2 us                                                | 28.8 us: 1.08x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.9 ms: 1.08x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.87 us: 1.05x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| meteor_contest           | 120 ms                                                 | 114 ms: 1.05x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.79 sec: 1.02x faster                                                           |
| regex_dna                | 227 ms                                                 | 223 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| unpickle_list            | 5.20 us                                                | 5.31 us: 1.02x slower                                                            |
| async_generators         | 444 ms                                                 | 456 ms: 1.03x slower                                                             |
| pickle_list              | 5.08 us                                                | 5.24 us: 1.03x slower                                                            |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.82 ms: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                            |
| telco                    | 7.27 ms                                                | 8.71 ms: 1.20x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240124-3.13.0a3+-6e55480-PYTHON_UOPS/bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.06x