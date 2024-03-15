
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: a8adada
- commit date: 2024-02-04
- overall geometric mean: 1.28x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.23x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.27 ms: 1.33x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 98.4 ms: 1.39x faster                                                            |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 452 ms: 1.61x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 578 ms: 1.50x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 727 ms: 1.40x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 119 ms: 1.29x faster                                                             |
| float          | 117 ms                                                 | 92.0 ms: 1.27x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 149 ms: 1.27x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.2 ms: 1.15x faster                                                            |
| regex_dna      | 227 ms                                                 | 221 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 234 us: 1.41x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.35 sec: 1.33x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.4 ms: 1.31x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 88.9 ms: 1.12x faster                                                            |
| json_loads           | 31.2 us                                                | 28.7 us: 1.09x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.05x faster                                                             |
| unpickle_list        | 5.20 us                                                | 4.96 us: 1.05x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.12 us: 1.01x slower                                                            |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| unpickle             | 14.4 us                                                | 16.5 us: 1.14x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.18x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.6 ms: 1.20x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 114 us: 4.77x faster                                                             |
| generators               | 80.1 ms                                                | 29.6 ms: 2.70x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.52 ms: 2.25x faster                                                            |
| logging_silent           | 190 ns                                                 | 99.1 ns: 1.91x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 496 ms: 1.86x faster                                                             |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.79x faster                                                             |
| richards_super           | 94.7 ms                                                | 53.7 ms: 1.76x faster                                                            |
| raytrace                 | 507 ms                                                 | 296 ms: 1.71x faster                                                             |
| richards                 | 79.3 ms                                                | 48.0 ms: 1.65x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.64x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                             |
| async_tree_none          | 728 ms                                                 | 452 ms: 1.61x faster                                                             |
| chaos                    | 115 ms                                                 | 71.6 ms: 1.61x faster                                                            |
| coroutines               | 35.1 ms                                                | 21.9 ms: 1.60x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 39.2 ns: 1.53x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 84.0 ms: 1.52x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 578 ms: 1.50x faster                                                             |
| scimark_lu               | 176 ms                                                 | 117 ms: 1.50x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 79.8 ms: 1.48x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 40.2 us: 1.46x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.42x faster                                                           |
| logging_simple           | 8.30 us                                                | 5.85 us: 1.42x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 234 us: 1.41x faster                                                             |
| pyflate                  | 716 ms                                                 | 509 ms: 1.41x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.5 us: 1.40x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 727 ms: 1.40x faster                                                             |
| tornado_http             | 136 ms                                                 | 98.4 ms: 1.39x faster                                                            |
| logging_format           | 9.09 us                                                | 6.67 us: 1.36x faster                                                            |
| go                       | 240 ms                                                 | 177 ms: 1.36x faster                                                             |
| deepcopy                 | 479 us                                                 | 359 us: 1.34x faster                                                             |
| tomli_loads              | 3.14 sec                                               | 2.35 sec: 1.33x faster                                                           |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.27 ms: 1.33x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.16 us: 1.32x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 60.4 ms: 1.31x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.31x faster                                                           |
| nbody                    | 154 ms                                                 | 119 ms: 1.29x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 799 ms: 1.27x faster                                                             |
| float                    | 117 ms                                                 | 92.0 ms: 1.27x faster                                                            |
| regex_compile            | 188 ms                                                 | 149 ms: 1.27x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.67 sec: 1.26x faster                                                           |
| spectral_norm            | 170 ms                                                 | 135 ms: 1.26x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.25x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 20.7 ms: 1.25x faster                                                            |
| hexiom                   | 10.4 ms                                                | 8.34 ms: 1.25x faster                                                            |
| 2to3                     | 348 ms                                                 | 282 ms: 1.23x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 68.6 ms: 1.23x faster                                                            |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 57.4 ms: 1.21x faster                                                            |
| mako                     | 16.3 ms                                                | 13.6 ms: 1.20x faster                                                            |
| sympy_str                | 346 ms                                                 | 289 ms: 1.20x faster                                                             |
| dask                     | 441 ms                                                 | 369 ms: 1.19x faster                                                             |
| fannkuch                 | 532 ms                                                 | 448 ms: 1.19x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 843 us: 1.17x faster                                                             |
| sympy_expand             | 566 ms                                                 | 486 ms: 1.16x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.63 ms: 1.15x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 24.2 ms: 1.15x faster                                                            |
| nqueens                  | 106 ms                                                 | 92.8 ms: 1.14x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 88.9 ms: 1.12x faster                                                            |
| scimark_fft              | 466 ms                                                 | 416 ms: 1.12x faster                                                             |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.10x faster                                                            |
| json_loads               | 31.2 us                                                | 28.7 us: 1.09x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                            |
| json                     | 5.69 ms                                                | 5.25 ms: 1.08x faster                                                            |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.05x faster                                                             |
| meteor_contest           | 120 ms                                                 | 114 ms: 1.05x faster                                                             |
| unpickle_list            | 5.20 us                                                | 4.96 us: 1.05x faster                                                            |
| regex_dna                | 227 ms                                                 | 221 ms: 1.02x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.80 sec: 1.02x faster                                                           |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                             |
| pickle_list              | 5.08 us                                                | 5.12 us: 1.01x slower                                                            |
| async_generators         | 444 ms                                                 | 456 ms: 1.03x slower                                                             |
| gc_traversal             | 3.62 ms                                                | 3.93 ms: 1.09x slower                                                            |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| unpickle                 | 14.4 us                                                | 16.5 us: 1.14x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.18x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.1 ms: 1.20x slower                                                            |
| telco                    | 7.27 ms                                                | 8.75 ms: 1.20x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240204-3.13.0a3+-a8adada-PYTHON_UOPS/bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.07x