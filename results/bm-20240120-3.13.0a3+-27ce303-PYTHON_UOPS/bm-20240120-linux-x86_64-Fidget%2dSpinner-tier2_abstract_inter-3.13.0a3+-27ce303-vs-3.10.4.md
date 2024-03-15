
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.27x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.37x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 287 ms: 1.21x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.39 ms: 1.31x faster                                                            |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                           |
| tornado_http   | 136 ms                                                 | 97.5 ms: 1.40x faster                                                            |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 578 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 89.4 ms: 1.31x faster                                                            |
| nbody          | 154 ms                                                 | 119 ms: 1.29x faster                                                             |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.20x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 150 ms: 1.26x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                            |
| regex_dna      | 227 ms                                                 | 227 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 238 us: 1.39x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.32 sec: 1.35x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 61.2 ms: 1.29x faster                                                            |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 89.6 ms: 1.11x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| unpickle_list        | 5.20 us                                                | 5.01 us: 1.04x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                            |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                                            |
| pickle               | 10.7 us                                                | 11.9 us: 1.12x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.18x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.7 ms: 1.19x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 120 us: 4.55x faster                                                             |
| generators               | 80.1 ms                                                | 29.7 ms: 2.69x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 500 ms: 1.84x faster                                                             |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                                             |
| richards_super           | 94.7 ms                                                | 54.5 ms: 1.74x faster                                                            |
| deltablue                | 7.91 ms                                                | 4.59 ms: 1.72x faster                                                            |
| raytrace                 | 507 ms                                                 | 296 ms: 1.71x faster                                                             |
| richards                 | 79.3 ms                                                | 48.4 ms: 1.64x faster                                                            |
| scimark_sor              | 220 ms                                                 | 134 ms: 1.63x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                            |
| async_tree_none          | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| chaos                    | 115 ms                                                 | 71.3 ms: 1.62x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 305 us: 1.59x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.2 ms: 1.58x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                            |
| go                       | 240 ms                                                 | 157 ms: 1.53x faster                                                             |
| crypto_pyaes             | 128 ms                                                 | 84.0 ms: 1.52x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 578 ms: 1.51x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 79.5 ms: 1.49x faster                                                            |
| scimark_lu               | 176 ms                                                 | 118 ms: 1.49x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.42x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 41.2 us: 1.42x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| tornado_http             | 136 ms                                                 | 97.5 ms: 1.40x faster                                                            |
| logging_simple           | 8.30 us                                                | 5.96 us: 1.39x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 238 us: 1.39x faster                                                             |
| pyflate                  | 716 ms                                                 | 522 ms: 1.37x faster                                                             |
| comprehensions           | 28.8 us                                                | 21.1 us: 1.37x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.32 sec: 1.35x faster                                                           |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| logging_format           | 9.09 us                                                | 6.77 us: 1.34x faster                                                            |
| deepcopy                 | 479 us                                                 | 361 us: 1.33x faster                                                             |
| deepcopy_reduce          | 4.17 us                                                | 3.17 us: 1.31x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.39 ms: 1.31x faster                                                            |
| float                    | 117 ms                                                 | 89.4 ms: 1.31x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                                           |
| xml_etree_process        | 79.1 ms                                                | 61.2 ms: 1.29x faster                                                            |
| nbody                    | 154 ms                                                 | 119 ms: 1.29x faster                                                             |
| hexiom                   | 10.4 ms                                                | 8.15 ms: 1.28x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 810 ms: 1.26x faster                                                             |
| regex_compile            | 188 ms                                                 | 150 ms: 1.26x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.69 sec: 1.25x faster                                                           |
| sqlglot_normalize        | 143 ms                                                 | 116 ms: 1.24x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.23x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 68.6 ms: 1.23x faster                                                            |
| spectral_norm            | 170 ms                                                 | 138 ms: 1.23x faster                                                             |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| 2to3                     | 348 ms                                                 | 287 ms: 1.21x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                           |
| fannkuch                 | 532 ms                                                 | 442 ms: 1.20x faster                                                             |
| mako                     | 16.3 ms                                                | 13.7 ms: 1.19x faster                                                            |
| dask                     | 441 ms                                                 | 369 ms: 1.19x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 58.4 ms: 1.18x faster                                                            |
| sympy_str                | 346 ms                                                 | 292 ms: 1.18x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 850 us: 1.16x faster                                                             |
| sympy_expand             | 566 ms                                                 | 492 ms: 1.15x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.72 ms: 1.13x faster                                                            |
| nqueens                  | 106 ms                                                 | 93.8 ms: 1.13x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                            |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 89.6 ms: 1.11x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                            |
| scimark_fft              | 466 ms                                                 | 422 ms: 1.10x faster                                                             |
| json                     | 5.69 ms                                                | 5.17 ms: 1.10x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 56.7 ns: 1.06x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| meteor_contest           | 120 ms                                                 | 114 ms: 1.05x faster                                                             |
| unpickle_list            | 5.20 us                                                | 5.01 us: 1.04x faster                                                            |
| asyncio_websockets       | 559 ms                                                 | 550 ms: 1.02x faster                                                             |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.83 sec: 1.01x faster                                                           |
| regex_dna                | 227 ms                                                 | 227 ms: 1.00x slower                                                             |
| pickle_list              | 5.08 us                                                | 5.25 us: 1.03x slower                                                            |
| async_generators         | 444 ms                                                 | 459 ms: 1.03x slower                                                             |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.98 ms: 1.10x slower                                                            |
| pickle                   | 10.7 us                                                | 11.9 us: 1.12x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.18x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.2 ms: 1.20x slower                                                            |
| telco                    | 7.27 ms                                                | 8.82 ms: 1.21x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.27x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-27ce303-PYTHON_UOPS/bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.37x