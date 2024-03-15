# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_superinstructi
- machine: linux-x86_64
- commit hash: 4861d7d
- commit date: 2024-03-05
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.34x

Benchmarks with tag 'apps':
===========================

| Benchmark    | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|--------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tornado_http | 136 ms                                                 | 96.8 ms: 1.41x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 438 ms: 1.66x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 563 ms: 1.55x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 705 ms: 1.44x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.3 ms: 1.66x faster                                                            |
| float          | 117 ms                                                 | 77.8 ms: 1.51x faster                                                            |
| pidigits       | 191 ms                                                 | 186 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.37x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 141 ms: 1.34x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| regex_dna      | 227 ms                                                 | 215 ms: 1.05x faster                                                             |
| Geometric mean | (ref)                                                  | 1.11x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 3.14 sec                                               | 2.02 sec: 1.55x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 236 us: 1.40x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 86.0 ms: 1.16x faster                                                            |
| json_loads           | 31.2 us                                                | 27.3 us: 1.14x faster                                                            |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                                             |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| unpickle_list        | 5.20 us                                                | 4.85 us: 1.07x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.17 us: 1.02x slower                                                            |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.18x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 4.99x faster                                                             |
| deltablue                | 7.91 ms                                                | 3.39 ms: 2.34x faster                                                            |
| raytrace                 | 507 ms                                                 | 266 ms: 1.91x faster                                                             |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                                             |
| asyncio_tcp              | 922 ms                                                 | 489 ms: 1.89x faster                                                             |
| chaos                    | 115 ms                                                 | 62.2 ms: 1.86x faster                                                            |
| richards_super           | 94.7 ms                                                | 52.0 ms: 1.82x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 73.4 ms: 1.74x faster                                                            |
| richards                 | 79.3 ms                                                | 45.9 ms: 1.73x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.69x faster                                                            |
| nbody                    | 154 ms                                                 | 92.3 ms: 1.66x faster                                                            |
| async_tree_none          | 728 ms                                                 | 438 ms: 1.66x faster                                                             |
| comprehensions           | 28.8 us                                                | 17.3 us: 1.66x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                            |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.58x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.4 ms: 1.56x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.02 sec: 1.55x faster                                                           |
| async_tree_memoization   | 870 ms                                                 | 563 ms: 1.55x faster                                                             |
| go                       | 240 ms                                                 | 156 ms: 1.54x faster                                                             |
| pyflate                  | 716 ms                                                 | 470 ms: 1.52x faster                                                             |
| mako                     | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 38.7 us: 1.51x faster                                                            |
| float                    | 117 ms                                                 | 77.8 ms: 1.51x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                           |
| hexiom                   | 10.4 ms                                                | 6.98 ms: 1.49x faster                                                            |
| logging_simple           | 8.30 us                                                | 5.63 us: 1.47x faster                                                            |
| logging_format           | 9.09 us                                                | 6.19 us: 1.47x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 705 ms: 1.44x faster                                                             |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| tornado_http             | 136 ms                                                 | 96.8 ms: 1.41x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 236 us: 1.40x faster                                                             |
| deepcopy_reduce          | 4.17 us                                                | 3.01 us: 1.39x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 734 ms: 1.39x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.53 sec: 1.37x faster                                                           |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                            |
| deepcopy                 | 479 us                                                 | 350 us: 1.37x faster                                                             |
| fannkuch                 | 532 ms                                                 | 393 ms: 1.35x faster                                                             |
| regex_compile            | 188 ms                                                 | 141 ms: 1.34x faster                                                             |
| pycparser                | 1.58 sec                                               | 1.18 sec: 1.34x faster                                                           |
| xml_etree_process        | 79.1 ms                                                | 59.2 ms: 1.34x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.33x faster                                                             |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                                             |
| sympy_str                | 346 ms                                                 | 278 ms: 1.24x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                                            |
| sqlglot_optimize         | 69.2 ms                                                | 55.9 ms: 1.24x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 68.3 ms: 1.23x faster                                                            |
| sympy_expand             | 566 ms                                                 | 475 ms: 1.19x faster                                                             |
| python_startup           | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 843 us: 1.17x faster                                                             |
| nqueens                  | 106 ms                                                 | 90.6 ms: 1.17x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 86.0 ms: 1.16x faster                                                            |
| json_loads               | 31.2 us                                                | 27.3 us: 1.14x faster                                                            |
| json                     | 5.69 ms                                                | 5.06 ms: 1.13x faster                                                            |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.11x faster                                                             |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 107 ms: 1.08x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| unpickle_list            | 5.20 us                                                | 4.85 us: 1.07x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                           |
| regex_dna                | 227 ms                                                 | 215 ms: 1.05x faster                                                             |
| pidigits                 | 191 ms                                                 | 186 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| pickle_list              | 5.08 us                                                | 5.17 us: 1.02x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.76 ms: 1.04x slower                                                            |
| async_generators         | 444 ms                                                 | 466 ms: 1.05x slower                                                             |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| bench_mp_pool            | 24.0 ms                                                | 28.2 ms: 1.17x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.18x slower                                                            |
| dask                     | 441 ms                                                 | 531 ms: 1.20x slower                                                             |
| coverage                 | 79.4 ms                                                | 97.3 ms: 1.23x slower                                                            |
| unpack_sequence          | 60.0 ns                                                | 87.0 ns: 1.45x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                                     |

Benchmark hidden because not significant (2): mypy2, regex_effbot
Ignored benchmarks (24) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: 2to3, aiohttp, chameleon, django_template, djangocms, docutils, flaskblogging, generators, genshi_text, genshi_xml, gunicorn, html5lib, pickle_pure_python, pylint, scimark_fft, scimark_lu, scimark_monte_carlo, scimark_sor, scimark_sparse_mat_mult, sqlalchemy_declarative, sqlalchemy_imperative, telco, thrift, unpickle
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-4861d7d-JIT/bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.34x