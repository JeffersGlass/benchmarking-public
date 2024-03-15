
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 289 ms: 1.21x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.52 ms: 1.29x faster                                                            |
| docutils       | 3.30 sec                                               | 2.74 sec: 1.20x faster                                                           |
| tornado_http   | 136 ms                                                 | 101 ms: 1.34x faster                                                             |
| Geometric mean | (ref)                                                  | 1.26x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 450 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 581 ms: 1.50x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 101 ms: 1.16x faster                                                             |
| nbody          | 154 ms                                                 | 135 ms: 1.13x faster                                                             |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 156 ms: 1.21x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.5 ms: 1.13x faster                                                            |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                                             |
| regex_effbot   | 3.63 ms                                                | 3.54 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.62x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 240 us: 1.38x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 61.5 ms: 1.29x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.74 sec: 1.15x faster                                                           |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 90.0 ms: 1.10x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| unpickle_list        | 5.20 us                                                | 5.06 us: 1.03x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.15 us: 1.01x slower                                                            |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                                            |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.2 us: 1.16x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                                     |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.8 ms: 1.10x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 121 us: 4.51x faster                                                             |
| generators               | 80.1 ms                                                | 29.9 ms: 2.68x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 500 ms: 1.84x faster                                                             |
| logging_silent           | 190 ns                                                 | 106 ns: 1.80x faster                                                             |
| scimark_sor              | 220 ms                                                 | 130 ms: 1.69x faster                                                             |
| richards_super           | 94.7 ms                                                | 57.0 ms: 1.66x faster                                                            |
| raytrace                 | 507 ms                                                 | 312 ms: 1.62x faster                                                             |
| async_tree_none          | 728 ms                                                 | 450 ms: 1.62x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.62x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.35 ms: 1.60x faster                                                            |
| richards                 | 79.3 ms                                                | 50.6 ms: 1.57x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.9 ms: 1.53x faster                                                            |
| deltablue                | 7.91 ms                                                | 5.18 ms: 1.53x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.69 ms: 1.53x faster                                                            |
| chaos                    | 115 ms                                                 | 76.8 ms: 1.50x faster                                                            |
| go                       | 240 ms                                                 | 160 ms: 1.50x faster                                                             |
| async_tree_memoization   | 870 ms                                                 | 581 ms: 1.50x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| scimark_lu               | 176 ms                                                 | 121 ms: 1.46x faster                                                             |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 41.0 us: 1.43x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                           |
| crypto_pyaes             | 128 ms                                                 | 90.4 ms: 1.41x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 240 us: 1.38x faster                                                             |
| scimark_monte_carlo      | 118 ms                                                 | 86.3 ms: 1.37x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.08 us: 1.37x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                            |
| tornado_http             | 136 ms                                                 | 101 ms: 1.34x faster                                                             |
| deepcopy                 | 479 us                                                 | 357 us: 1.34x faster                                                             |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                            |
| pyflate                  | 716 ms                                                 | 540 ms: 1.33x faster                                                             |
| logging_format           | 9.09 us                                                | 6.87 us: 1.32x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.52 ms: 1.29x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 61.5 ms: 1.29x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                                           |
| unpack_sequence          | 60.0 ns                                                | 47.8 ns: 1.26x faster                                                            |
| comprehensions           | 28.8 us                                                | 23.1 us: 1.24x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 116 ms: 1.24x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 69.2 ms: 1.22x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 842 ms: 1.21x faster                                                             |
| 2to3                     | 348 ms                                                 | 289 ms: 1.21x faster                                                             |
| regex_compile            | 188 ms                                                 | 156 ms: 1.21x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.74 sec: 1.20x faster                                                           |
| pprint_pformat           | 2.10 sec                                               | 1.75 sec: 1.20x faster                                                           |
| sympy_sum                | 196 ms                                                 | 164 ms: 1.20x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 21.6 ms: 1.20x faster                                                            |
| dask                     | 441 ms                                                 | 369 ms: 1.19x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 59.0 ms: 1.17x faster                                                            |
| spectral_norm            | 170 ms                                                 | 145 ms: 1.17x faster                                                             |
| float                    | 117 ms                                                 | 101 ms: 1.16x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 855 us: 1.15x faster                                                             |
| tomli_loads              | 3.14 sec                                               | 2.74 sec: 1.15x faster                                                           |
| sympy_str                | 346 ms                                                 | 303 ms: 1.14x faster                                                             |
| fannkuch                 | 532 ms                                                 | 468 ms: 1.14x faster                                                             |
| nbody                    | 154 ms                                                 | 135 ms: 1.13x faster                                                             |
| regex_v8                 | 27.8 ms                                                | 24.5 ms: 1.13x faster                                                            |
| hexiom                   | 10.4 ms                                                | 9.23 ms: 1.13x faster                                                            |
| sympy_expand             | 566 ms                                                 | 504 ms: 1.12x faster                                                             |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                            |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 90.0 ms: 1.10x faster                                                            |
| mako                     | 16.3 ms                                                | 14.8 ms: 1.10x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                            |
| json                     | 5.69 ms                                                | 5.18 ms: 1.10x faster                                                            |
| nqueens                  | 106 ms                                                 | 98.6 ms: 1.07x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                           |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.06 ms: 1.07x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.92 us: 1.03x faster                                                            |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                                             |
| unpickle_list            | 5.20 us                                                | 5.06 us: 1.03x faster                                                            |
| regex_effbot             | 3.63 ms                                                | 3.54 ms: 1.03x faster                                                            |
| scimark_fft              | 466 ms                                                 | 459 ms: 1.02x faster                                                             |
| meteor_contest           | 120 ms                                                 | 118 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| gc_traversal             | 3.62 ms                                                | 3.65 ms: 1.01x slower                                                            |
| pickle_list              | 5.08 us                                                | 5.15 us: 1.01x slower                                                            |
| async_generators         | 444 ms                                                 | 460 ms: 1.04x slower                                                             |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.2 us: 1.16x slower                                                            |
| telco                    | 7.27 ms                                                | 8.66 ms: 1.19x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.1 ms: 1.20x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.24x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, xml_etree_iterparse, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240128-3.13.0a3+-d226882-PYTHON_UOPS/bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.07x