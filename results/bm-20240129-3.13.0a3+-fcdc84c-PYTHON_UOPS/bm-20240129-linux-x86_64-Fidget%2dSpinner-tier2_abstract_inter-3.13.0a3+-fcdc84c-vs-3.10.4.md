
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.26x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 284 ms: 1.23x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.49 ms: 1.29x faster                                                            |
| docutils       | 3.30 sec                                               | 2.73 sec: 1.21x faster                                                           |
| tornado_http   | 136 ms                                                 | 99.2 ms: 1.37x faster                                                            |
| Geometric mean | (ref)                                                  | 1.27x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 450 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 723 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 117 ms: 1.31x faster                                                             |
| float          | 117 ms                                                 | 93.3 ms: 1.26x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 152 ms: 1.24x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                            |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.09x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.61x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 236 us: 1.40x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.41 sec: 1.30x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 61.6 ms: 1.28x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 89.9 ms: 1.11x faster                                                            |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 112 ms: 1.03x faster                                                             |
| unpickle_list        | 5.20 us                                                | 5.05 us: 1.03x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.01 us: 1.01x faster                                                            |
| unpickle             | 14.4 us                                                | 15.4 us: 1.07x slower                                                            |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                            |
| pickle_dict          | 29.6 us                                                | 33.9 us: 1.14x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.78 ms: 1.48x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.1 ms: 1.15x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 118 us: 4.61x faster                                                             |
| generators               | 80.1 ms                                                | 30.0 ms: 2.67x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 495 ms: 1.86x faster                                                             |
| scimark_sor              | 220 ms                                                 | 125 ms: 1.76x faster                                                             |
| logging_silent           | 190 ns                                                 | 108 ns: 1.75x faster                                                             |
| richards_super           | 94.7 ms                                                | 55.2 ms: 1.72x faster                                                            |
| raytrace                 | 507 ms                                                 | 300 ms: 1.69x faster                                                             |
| deltablue                | 7.91 ms                                                | 4.70 ms: 1.68x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                            |
| richards                 | 79.3 ms                                                | 48.9 ms: 1.62x faster                                                            |
| async_tree_none          | 728 ms                                                 | 450 ms: 1.62x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.61x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.58x faster                                                            |
| chaos                    | 115 ms                                                 | 73.4 ms: 1.57x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                            |
| go                       | 240 ms                                                 | 156 ms: 1.54x faster                                                             |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| scimark_lu               | 176 ms                                                 | 117 ms: 1.50x faster                                                             |
| crypto_pyaes             | 128 ms                                                 | 85.6 ms: 1.49x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 80.1 ms: 1.48x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 41.0 us: 1.43x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 723 ms: 1.41x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 236 us: 1.40x faster                                                             |
| pyflate                  | 716 ms                                                 | 519 ms: 1.38x faster                                                             |
| tornado_http             | 136 ms                                                 | 99.2 ms: 1.37x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.09 us: 1.36x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| deepcopy                 | 479 us                                                 | 357 us: 1.34x faster                                                             |
| logging_format           | 9.09 us                                                | 6.83 us: 1.33x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.8 us: 1.32x faster                                                            |
| nbody                    | 154 ms                                                 | 117 ms: 1.31x faster                                                             |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.41 sec: 1.30x faster                                                           |
| chameleon                | 9.68 ms                                                | 7.49 ms: 1.29x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 61.6 ms: 1.28x faster                                                            |
| float                    | 117 ms                                                 | 93.3 ms: 1.26x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.25x faster                                                             |
| regex_compile            | 188 ms                                                 | 152 ms: 1.24x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 823 ms: 1.24x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.71 sec: 1.23x faster                                                           |
| 2to3                     | 348 ms                                                 | 284 ms: 1.23x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 68.8 ms: 1.23x faster                                                            |
| sympy_sum                | 196 ms                                                 | 161 ms: 1.22x faster                                                             |
| hexiom                   | 10.4 ms                                                | 8.51 ms: 1.22x faster                                                            |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.22x faster                                                            |
| spectral_norm            | 170 ms                                                 | 140 ms: 1.21x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.73 sec: 1.21x faster                                                           |
| fannkuch                 | 532 ms                                                 | 444 ms: 1.20x faster                                                             |
| dask                     | 441 ms                                                 | 369 ms: 1.19x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 58.2 ms: 1.19x faster                                                            |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 848 us: 1.16x faster                                                             |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                             |
| mako                     | 16.3 ms                                                | 14.1 ms: 1.15x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 53.0 ns: 1.13x faster                                                            |
| nqueens                  | 106 ms                                                 | 93.8 ms: 1.13x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                            |
| json                     | 5.69 ms                                                | 5.15 ms: 1.11x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 89.9 ms: 1.11x faster                                                            |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| scimark_fft              | 466 ms                                                 | 426 ms: 1.09x faster                                                             |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.09x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.97 ms: 1.08x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.63 sec: 1.08x faster                                                           |
| pathlib                  | 20.5 ms                                                | 19.1 ms: 1.07x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                            |
| meteor_contest           | 120 ms                                                 | 116 ms: 1.03x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 112 ms: 1.03x faster                                                             |
| unpickle_list            | 5.20 us                                                | 5.05 us: 1.03x faster                                                            |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                             |
| pickle_list              | 5.08 us                                                | 5.01 us: 1.01x faster                                                            |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 554 ms: 1.01x faster                                                             |
| async_generators         | 444 ms                                                 | 462 ms: 1.04x slower                                                             |
| unpickle                 | 14.4 us                                                | 15.4 us: 1.07x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.91 ms: 1.08x slower                                                            |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                            |
| pickle_dict              | 29.6 us                                                | 33.9 us: 1.14x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.1 ms: 1.20x slower                                                            |
| telco                    | 7.27 ms                                                | 8.79 ms: 1.21x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.78 ms: 1.48x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.26x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240129-3.13.0a3+-fcdc84c-PYTHON_UOPS/bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.07x