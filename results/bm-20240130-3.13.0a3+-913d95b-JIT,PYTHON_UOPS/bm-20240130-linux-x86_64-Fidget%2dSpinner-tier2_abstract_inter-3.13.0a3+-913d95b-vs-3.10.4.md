
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 280 ms: 1.25x faster                                                             |
| chameleon      | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                            |
| docutils       | 3.30 sec                                               | 2.68 sec: 1.23x faster                                                           |
| tornado_http   | 136 ms                                                 | 97.9 ms: 1.39x faster                                                            |
| Geometric mean | (ref)                                                  | 1.31x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 442 ms: 1.65x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 570 ms: 1.53x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 99.8 ms: 1.54x faster                                                            |
| float          | 117 ms                                                 | 86.6 ms: 1.35x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.28x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 143 ms: 1.32x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.61x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.44x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.22 sec: 1.42x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 87.7 ms: 1.13x faster                                                            |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| unpickle             | 14.4 us                                                | 14.7 us: 1.02x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                                            |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.0 us: 1.18x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                     |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.3 ms: 1.42x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.93 ms: 1.51x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.5 ms: 1.30x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.90x faster                                                             |
| generators               | 80.1 ms                                                | 29.7 ms: 2.69x faster                                                            |
| deltablue                | 7.91 ms                                                | 4.01 ms: 1.97x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 495 ms: 1.86x faster                                                             |
| logging_silent           | 190 ns                                                 | 102 ns: 1.86x faster                                                             |
| raytrace                 | 507 ms                                                 | 281 ms: 1.80x faster                                                             |
| richards_super           | 94.7 ms                                                | 52.9 ms: 1.79x faster                                                            |
| scimark_sor              | 220 ms                                                 | 125 ms: 1.76x faster                                                             |
| richards                 | 79.3 ms                                                | 46.6 ms: 1.70x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                                            |
| chaos                    | 115 ms                                                 | 69.5 ms: 1.66x faster                                                            |
| async_tree_none          | 728 ms                                                 | 442 ms: 1.65x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.61x faster                                                             |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.58x faster                                                            |
| go                       | 240 ms                                                 | 152 ms: 1.58x faster                                                             |
| crypto_pyaes             | 128 ms                                                 | 81.1 ms: 1.58x faster                                                            |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.55x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 76.2 ms: 1.55x faster                                                            |
| nbody                    | 154 ms                                                 | 99.8 ms: 1.54x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 570 ms: 1.53x faster                                                             |
| coroutines               | 35.1 ms                                                | 23.2 ms: 1.52x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 38.8 us: 1.51x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| comprehensions           | 28.8 us                                                | 19.4 us: 1.48x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 229 us: 1.44x faster                                                             |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                           |
| logging_format           | 9.09 us                                                | 6.40 us: 1.42x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.3 ms: 1.42x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| logging_simple           | 8.30 us                                                | 5.86 us: 1.42x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.22 sec: 1.42x faster                                                           |
| tornado_http             | 136 ms                                                 | 97.9 ms: 1.39x faster                                                            |
| chameleon                | 9.68 ms                                                | 6.96 ms: 1.39x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 43.2 ns: 1.39x faster                                                            |
| pyflate                  | 716 ms                                                 | 515 ms: 1.39x faster                                                             |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                                             |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.08 us: 1.35x faster                                                            |
| float                    | 117 ms                                                 | 86.6 ms: 1.35x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                                           |
| xml_etree_process        | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                            |
| regex_compile            | 188 ms                                                 | 143 ms: 1.32x faster                                                             |
| mako                     | 16.3 ms                                                | 12.5 ms: 1.30x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 111 ms: 1.29x faster                                                             |
| spectral_norm            | 170 ms                                                 | 135 ms: 1.26x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 809 ms: 1.26x faster                                                             |
| scimark_fft              | 466 ms                                                 | 372 ms: 1.25x faster                                                             |
| 2to3                     | 348 ms                                                 | 280 ms: 1.25x faster                                                             |
| fannkuch                 | 532 ms                                                 | 428 ms: 1.24x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 68.5 ms: 1.23x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.68 sec: 1.23x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 56.5 ms: 1.22x faster                                                            |
| pprint_pformat           | 2.10 sec                                               | 1.73 sec: 1.22x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.3 ms: 1.21x faster                                                            |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                                             |
| dask                     | 441 ms                                                 | 366 ms: 1.21x faster                                                             |
| hexiom                   | 10.4 ms                                                | 8.65 ms: 1.20x faster                                                            |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 839 us: 1.18x faster                                                             |
| nqueens                  | 106 ms                                                 | 90.0 ms: 1.18x faster                                                            |
| sympy_expand             | 566 ms                                                 | 485 ms: 1.17x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.57 ms: 1.16x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 87.7 ms: 1.13x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.13x faster                                                            |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| json                     | 5.69 ms                                                | 5.19 ms: 1.10x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                            |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                            |
| meteor_contest           | 120 ms                                                 | 112 ms: 1.07x faster                                                             |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.74 sec: 1.04x faster                                                           |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                             |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 555 ms: 1.01x faster                                                             |
| unpickle                 | 14.4 us                                                | 14.7 us: 1.02x slower                                                            |
| pickle_list              | 5.08 us                                                | 5.20 us: 1.02x slower                                                            |
| async_generators         | 444 ms                                                 | 463 ms: 1.04x slower                                                             |
| gc_traversal             | 3.62 ms                                                | 3.87 ms: 1.07x slower                                                            |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| telco                    | 7.27 ms                                                | 8.43 ms: 1.16x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.0 us: 1.18x slower                                                            |
| coverage                 | 79.4 ms                                                | 94.6 ms: 1.19x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.93 ms: 1.51x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                                     |

Benchmark hidden because not significant (4): mypy2, bench_mp_pool, unpickle_list, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240130-3.13.0a3+-913d95b-JIT,PYTHON_UOPS/bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.11x