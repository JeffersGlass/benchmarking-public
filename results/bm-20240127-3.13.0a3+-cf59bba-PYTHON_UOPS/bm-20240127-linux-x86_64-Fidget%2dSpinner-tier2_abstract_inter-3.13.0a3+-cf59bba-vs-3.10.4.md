
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 283 ms: 1.23x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.16 ms: 1.35x faster                                                            |
| docutils       | 3.30 sec                                               | 2.69 sec: 1.23x faster                                                           |
| tornado_http   | 136 ms                                                 | 98.5 ms: 1.38x faster                                                            |
| Geometric mean | (ref)                                                  | 1.30x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 448 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 573 ms: 1.52x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 113 ms: 1.36x faster                                                             |
| float          | 117 ms                                                 | 87.7 ms: 1.33x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.23x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 148 ms: 1.27x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.9 ms: 1.11x faster                                                            |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                             |
| regex_effbot   | 3.63 ms                                                | 3.56 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 297 us: 1.63x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 234 us: 1.41x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.31 sec: 1.36x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 60.5 ms: 1.31x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 89.1 ms: 1.12x faster                                                            |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpickle_list        | 5.20 us                                                | 4.94 us: 1.05x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                                            |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                            |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.17x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.79 ms: 1.48x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.9 ms: 1.26x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.70x faster                                                             |
| generators               | 80.1 ms                                                | 29.8 ms: 2.69x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 488 ms: 1.89x faster                                                             |
| logging_silent           | 190 ns                                                 | 104 ns: 1.83x faster                                                             |
| deltablue                | 7.91 ms                                                | 4.41 ms: 1.79x faster                                                            |
| raytrace                 | 507 ms                                                 | 294 ms: 1.73x faster                                                             |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.72x faster                                                             |
| richards_super           | 94.7 ms                                                | 55.3 ms: 1.71x faster                                                            |
| chaos                    | 115 ms                                                 | 70.2 ms: 1.65x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.64x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 297 us: 1.63x faster                                                             |
| async_tree_none          | 728 ms                                                 | 448 ms: 1.62x faster                                                             |
| richards                 | 79.3 ms                                                | 48.9 ms: 1.62x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 82.2 ms: 1.56x faster                                                            |
| go                       | 240 ms                                                 | 155 ms: 1.55x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.55x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 77.5 ms: 1.52x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 573 ms: 1.52x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| unpack_sequence          | 60.0 ns                                                | 40.7 ns: 1.47x faster                                                            |
| scimark_lu               | 176 ms                                                 | 120 ms: 1.47x faster                                                             |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 40.9 us: 1.43x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 234 us: 1.41x faster                                                             |
| pyflate                  | 716 ms                                                 | 508 ms: 1.41x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.6 us: 1.40x faster                                                            |
| tornado_http             | 136 ms                                                 | 98.5 ms: 1.38x faster                                                            |
| logging_simple           | 8.30 us                                                | 6.06 us: 1.37x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                            |
| nbody                    | 154 ms                                                 | 113 ms: 1.36x faster                                                             |
| tomli_loads              | 3.14 sec                                               | 2.31 sec: 1.36x faster                                                           |
| chameleon                | 9.68 ms                                                | 7.16 ms: 1.35x faster                                                            |
| logging_format           | 9.09 us                                                | 6.76 us: 1.34x faster                                                            |
| float                    | 117 ms                                                 | 87.7 ms: 1.33x faster                                                            |
| deepcopy                 | 479 us                                                 | 361 us: 1.33x faster                                                             |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.31x faster                                                           |
| xml_etree_process        | 79.1 ms                                                | 60.5 ms: 1.31x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.19 us: 1.31x faster                                                            |
| hexiom                   | 10.4 ms                                                | 8.01 ms: 1.30x faster                                                            |
| spectral_norm            | 170 ms                                                 | 132 ms: 1.29x faster                                                             |
| regex_compile            | 188 ms                                                 | 148 ms: 1.27x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.66 sec: 1.27x faster                                                           |
| mako                     | 16.3 ms                                                | 12.9 ms: 1.26x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.26x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 806 ms: 1.26x faster                                                             |
| fannkuch                 | 532 ms                                                 | 429 ms: 1.24x faster                                                             |
| sympy_sum                | 196 ms                                                 | 159 ms: 1.24x faster                                                             |
| 2to3                     | 348 ms                                                 | 283 ms: 1.23x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.69 sec: 1.23x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.23x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 68.8 ms: 1.22x faster                                                            |
| sqlglot_optimize         | 69.2 ms                                                | 57.6 ms: 1.20x faster                                                            |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                             |
| sympy_str                | 346 ms                                                 | 290 ms: 1.19x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.50 ms: 1.18x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 842 us: 1.17x faster                                                             |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                             |
| nqueens                  | 106 ms                                                 | 92.2 ms: 1.15x faster                                                            |
| scimark_fft              | 466 ms                                                 | 414 ms: 1.13x faster                                                             |
| xml_etree_generate       | 99.4 ms                                                | 89.1 ms: 1.12x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 24.9 ms: 1.11x faster                                                            |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| json                     | 5.69 ms                                                | 5.17 ms: 1.10x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.6 ms: 1.10x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.61 sec: 1.09x faster                                                           |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpickle_list            | 5.20 us                                                | 4.94 us: 1.05x faster                                                            |
| meteor_contest           | 120 ms                                                 | 114 ms: 1.05x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                            |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                             |
| regex_effbot             | 3.63 ms                                                | 3.56 ms: 1.02x faster                                                            |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 553 ms: 1.01x faster                                                             |
| gc_traversal             | 3.62 ms                                                | 3.72 ms: 1.03x slower                                                            |
| async_generators         | 444 ms                                                 | 456 ms: 1.03x slower                                                             |
| pickle_list              | 5.08 us                                                | 5.23 us: 1.03x slower                                                            |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                            |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.17x slower                                                            |
| coverage                 | 79.4 ms                                                | 93.5 ms: 1.18x slower                                                            |
| telco                    | 7.27 ms                                                | 8.62 ms: 1.19x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.79 ms: 1.48x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                                     |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-cf59bba-PYTHON_UOPS/bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.08x