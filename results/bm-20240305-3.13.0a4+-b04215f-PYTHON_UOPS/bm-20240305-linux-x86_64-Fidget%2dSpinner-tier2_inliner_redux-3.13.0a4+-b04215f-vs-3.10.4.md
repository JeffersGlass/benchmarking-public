# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_inliner_redux
- machine: linux-x86_64
- commit hash: b04215f
- commit date: 2024-03-05
- overall geometric mean: 1.18x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 300 ms: 1.16x faster                                                            |
| chameleon      | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                           |
| docutils       | 3.30 sec                                               | 2.84 sec: 1.16x faster                                                          |
| tornado_http   | 136 ms                                                 | 102 ms: 1.33x faster                                                            |
| Geometric mean | (ref)                                                  | 1.26x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 462 ms: 1.57x faster                                                            |
| async_tree_memoization  | 870 ms                                                 | 592 ms: 1.47x faster                                                            |
| async_tree_io           | 1.77 sec                                               | 1.25 sec: 1.41x faster                                                          |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 737 ms: 1.38x faster                                                            |
| Geometric mean          | (ref)                                                  | 1.46x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 132 ms: 1.16x faster                                                            |
| float          | 117 ms                                                 | 106 ms: 1.11x faster                                                            |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                  | 1.09x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 24.4 ms: 1.14x faster                                                           |
| regex_dna      | 227 ms                                                 | 213 ms: 1.06x faster                                                            |
| regex_effbot   | 3.63 ms                                                | 3.55 ms: 1.02x faster                                                           |
| regex_compile  | 188 ms                                                 | 191 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 303 us: 1.60x faster                                                            |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 63.1 ms: 1.25x faster                                                           |
| tomli_loads          | 3.14 sec                                               | 2.79 sec: 1.12x faster                                                          |
| json_loads           | 31.2 us                                                | 27.9 us: 1.12x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 309 us: 1.07x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 93.3 ms: 1.07x faster                                                           |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                            |
| unpickle_list        | 5.20 us                                                | 5.12 us: 1.02x faster                                                           |
| pickle_list          | 5.08 us                                                | 5.33 us: 1.05x slower                                                           |
| unpickle             | 14.4 us                                                | 15.7 us: 1.09x slower                                                           |
| pickle               | 10.7 us                                                | 11.9 us: 1.12x slower                                                           |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.19x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.08x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                           |
| python_startup_no_site | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                           |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 15.1 ms: 1.08x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 119 us: 4.58x faster                                                            |
| generators               | 80.1 ms                                                | 29.9 ms: 2.68x faster                                                           |
| deltablue                | 7.91 ms                                                | 4.02 ms: 1.97x faster                                                           |
| asyncio_tcp              | 922 ms                                                 | 489 ms: 1.89x faster                                                            |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 303 us: 1.60x faster                                                            |
| async_tree_none          | 728 ms                                                 | 462 ms: 1.57x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.54x faster                                                           |
| scimark_sor              | 220 ms                                                 | 148 ms: 1.48x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.48 ms: 1.47x faster                                                           |
| async_tree_memoization   | 870 ms                                                 | 592 ms: 1.47x faster                                                            |
| chaos                    | 115 ms                                                 | 80.3 ms: 1.44x faster                                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                          |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.82 ms: 1.42x faster                                                           |
| async_tree_io            | 1.77 sec                                               | 1.25 sec: 1.41x faster                                                          |
| richards_super           | 94.7 ms                                                | 67.7 ms: 1.40x faster                                                           |
| crypto_pyaes             | 128 ms                                                 | 92.2 ms: 1.39x faster                                                           |
| logging_simple           | 8.30 us                                                | 6.00 us: 1.38x faster                                                           |
| chameleon                | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                           |
| raytrace                 | 507 ms                                                 | 367 ms: 1.38x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 737 ms: 1.38x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                           |
| logging_format           | 9.09 us                                                | 6.79 us: 1.34x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 43.8 us: 1.33x faster                                                           |
| tornado_http             | 136 ms                                                 | 102 ms: 1.33x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.15 us: 1.32x faster                                                           |
| deepcopy                 | 479 us                                                 | 366 us: 1.31x faster                                                            |
| richards                 | 79.3 ms                                                | 61.2 ms: 1.29x faster                                                           |
| go                       | 240 ms                                                 | 190 ms: 1.27x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.26x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 63.1 ms: 1.25x faster                                                           |
| comprehensions           | 28.8 us                                                | 23.5 us: 1.22x faster                                                           |
| pycparser                | 1.58 sec                                               | 1.30 sec: 1.21x faster                                                          |
| sympy_integrate          | 25.8 ms                                                | 21.6 ms: 1.19x faster                                                           |
| sympy_sum                | 196 ms                                                 | 166 ms: 1.18x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 72.1 ms: 1.17x faster                                                           |
| 2to3                     | 348 ms                                                 | 300 ms: 1.16x faster                                                            |
| nbody                    | 154 ms                                                 | 132 ms: 1.16x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.84 sec: 1.16x faster                                                          |
| scimark_monte_carlo      | 118 ms                                                 | 102 ms: 1.15x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 24.4 ms: 1.14x faster                                                           |
| bench_thread_pool        | 986 us                                                 | 867 us: 1.14x faster                                                            |
| sympy_str                | 346 ms                                                 | 306 ms: 1.13x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.79 sec: 1.12x faster                                                          |
| json_loads               | 31.2 us                                                | 27.9 us: 1.12x faster                                                           |
| float                    | 117 ms                                                 | 106 ms: 1.11x faster                                                            |
| json                     | 5.69 ms                                                | 5.13 ms: 1.11x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 62.7 ms: 1.10x faster                                                           |
| sympy_expand             | 566 ms                                                 | 514 ms: 1.10x faster                                                            |
| pyflate                  | 716 ms                                                 | 660 ms: 1.08x faster                                                            |
| mako                     | 16.3 ms                                                | 15.1 ms: 1.08x faster                                                           |
| pprint_safe_repr         | 1.02 sec                                               | 945 ms: 1.08x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                           |
| pprint_pformat           | 2.10 sec                                               | 1.96 sec: 1.07x faster                                                          |
| unpickle_pure_python     | 331 us                                                 | 309 us: 1.07x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 93.3 ms: 1.07x faster                                                           |
| pathlib                  | 20.5 ms                                                | 19.2 ms: 1.07x faster                                                           |
| regex_dna                | 227 ms                                                 | 213 ms: 1.06x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                            |
| spectral_norm            | 170 ms                                                 | 162 ms: 1.05x faster                                                            |
| scimark_lu               | 176 ms                                                 | 169 ms: 1.04x faster                                                            |
| regex_effbot             | 3.63 ms                                                | 3.55 ms: 1.02x faster                                                           |
| unpickle_list            | 5.20 us                                                | 5.12 us: 1.02x faster                                                           |
| sqlite_synth             | 3.02 us                                                | 2.98 us: 1.01x faster                                                           |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                            |
| pidigits                 | 191 ms                                                 | 190 ms: 1.01x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.53 ms: 1.01x slower                                                           |
| mdp                      | 2.85 sec                                               | 2.88 sec: 1.01x slower                                                          |
| regex_compile            | 188 ms                                                 | 191 ms: 1.01x slower                                                            |
| scimark_fft              | 466 ms                                                 | 473 ms: 1.02x slower                                                            |
| fannkuch                 | 532 ms                                                 | 540 ms: 1.02x slower                                                            |
| hexiom                   | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                           |
| unpack_sequence          | 60.0 ns                                                | 61.2 ns: 1.02x slower                                                           |
| meteor_contest           | 120 ms                                                 | 122 ms: 1.02x slower                                                            |
| async_generators         | 444 ms                                                 | 462 ms: 1.04x slower                                                            |
| pickle_list              | 5.08 us                                                | 5.33 us: 1.05x slower                                                           |
| nqueens                  | 106 ms                                                 | 112 ms: 1.06x slower                                                            |
| unpickle                 | 14.4 us                                                | 15.7 us: 1.09x slower                                                           |
| gc_traversal             | 3.62 ms                                                | 4.02 ms: 1.11x slower                                                           |
| pickle                   | 10.7 us                                                | 11.9 us: 1.12x slower                                                           |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.19x slower                                                           |
| telco                    | 7.27 ms                                                | 8.84 ms: 1.22x slower                                                           |
| dask                     | 441 ms                                                 | 538 ms: 1.22x slower                                                            |
| coverage                 | 79.4 ms                                                | 97.4 ms: 1.23x slower                                                           |
| python_startup_no_site   | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                           |
| Geometric mean           | (ref)                                                  | 1.18x faster                                                                    |

Benchmark hidden because not significant (3): bench_mp_pool, xml_etree_iterparse, mypy2
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-b04215f-PYTHON_UOPS/bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: 1.07x