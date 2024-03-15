# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_superinstructi
- machine: linux-x86_64
- commit hash: c04ea6c
- commit date: 2024-03-01
- overall geometric mean: 1.28x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.34x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 280 ms: 1.24x faster                                                             |
| chameleon      | 9.68 ms                                                | 6.99 ms: 1.38x faster                                                            |
| docutils       | 3.30 sec                                               | 2.74 sec: 1.20x faster                                                           |
| tornado_http   | 136 ms                                                 | 96.3 ms: 1.42x faster                                                            |
| Geometric mean | (ref)                                                  | 1.31x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 439 ms: 1.66x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 567 ms: 1.54x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.43x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 96.2 ms: 1.60x faster                                                            |
| float          | 117 ms                                                 | 82.7 ms: 1.42x faster                                                            |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.32x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 153 ms: 1.23x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| regex_dna      | 227 ms                                                 | 232 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.16 sec: 1.45x faster                                                           |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                            |
| unpickle_pure_python | 331 us                                                 | 245 us: 1.35x faster                                                             |
| xml_etree_process    | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 86.8 ms: 1.15x faster                                                            |
| json_loads           | 31.2 us                                                | 27.3 us: 1.14x faster                                                            |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.08x faster                                                             |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                             |
| unpickle_list        | 5.20 us                                                | 4.93 us: 1.06x faster                                                            |
| pickle_list          | 5.08 us                                                | 4.97 us: 1.02x faster                                                            |
| pickle               | 10.7 us                                                | 11.7 us: 1.09x slower                                                            |
| unpickle             | 14.4 us                                                | 16.2 us: 1.12x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.1 us: 1.15x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.24x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.9 ms: 1.37x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.96x faster                                                             |
| generators               | 80.1 ms                                                | 29.3 ms: 2.74x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.46 ms: 2.28x faster                                                            |
| logging_silent           | 190 ns                                                 | 101 ns: 1.88x faster                                                             |
| asyncio_tcp              | 922 ms                                                 | 492 ms: 1.88x faster                                                             |
| raytrace                 | 507 ms                                                 | 276 ms: 1.84x faster                                                             |
| chaos                    | 115 ms                                                 | 64.8 ms: 1.78x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 74.7 ms: 1.71x faster                                                            |
| richards_super           | 94.7 ms                                                | 56.0 ms: 1.69x faster                                                            |
| scimark_sor              | 220 ms                                                 | 130 ms: 1.69x faster                                                             |
| async_tree_none          | 728 ms                                                 | 439 ms: 1.66x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.31 ms: 1.65x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                             |
| nbody                    | 154 ms                                                 | 96.2 ms: 1.60x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                            |
| richards                 | 79.3 ms                                                | 50.1 ms: 1.58x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 76.2 ms: 1.55x faster                                                            |
| comprehensions           | 28.8 us                                                | 18.6 us: 1.54x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 567 ms: 1.54x faster                                                             |
| go                       | 240 ms                                                 | 156 ms: 1.53x faster                                                             |
| deepcopy_memo            | 58.5 us                                                | 39.0 us: 1.50x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.49x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.16 sec: 1.45x faster                                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.43x faster                                                             |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| spectral_norm            | 170 ms                                                 | 120 ms: 1.42x faster                                                             |
| logging_format           | 9.09 us                                                | 6.41 us: 1.42x faster                                                            |
| logging_simple           | 8.30 us                                                | 5.86 us: 1.42x faster                                                            |
| float                    | 117 ms                                                 | 82.7 ms: 1.42x faster                                                            |
| tornado_http             | 136 ms                                                 | 96.3 ms: 1.42x faster                                                            |
| pyflate                  | 716 ms                                                 | 509 ms: 1.41x faster                                                             |
| chameleon                | 9.68 ms                                                | 6.99 ms: 1.38x faster                                                            |
| deepcopy                 | 479 us                                                 | 347 us: 1.38x faster                                                             |
| mako                     | 16.3 ms                                                | 11.9 ms: 1.37x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 245 us: 1.35x faster                                                             |
| xml_etree_process        | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                            |
| hexiom                   | 10.4 ms                                                | 7.74 ms: 1.34x faster                                                            |
| scimark_lu               | 176 ms                                                 | 131 ms: 1.34x faster                                                             |
| deepcopy_reduce          | 4.17 us                                                | 3.12 us: 1.34x faster                                                            |
| scimark_fft              | 466 ms                                                 | 354 ms: 1.32x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                                             |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                                           |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.08 ms: 1.27x faster                                                            |
| fannkuch                 | 532 ms                                                 | 419 ms: 1.27x faster                                                             |
| 2to3                     | 348 ms                                                 | 280 ms: 1.24x faster                                                             |
| regex_compile            | 188 ms                                                 | 153 ms: 1.23x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.72 sec: 1.23x faster                                                           |
| pprint_safe_repr         | 1.02 sec                                               | 831 ms: 1.22x faster                                                             |
| sympy_sum                | 196 ms                                                 | 161 ms: 1.22x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 56.7 ms: 1.22x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 69.3 ms: 1.22x faster                                                            |
| sympy_str                | 346 ms                                                 | 286 ms: 1.21x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.74 sec: 1.20x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.5 ms: 1.20x faster                                                            |
| python_startup           | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                            |
| sympy_expand             | 566 ms                                                 | 485 ms: 1.17x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 849 us: 1.16x faster                                                             |
| nqueens                  | 106 ms                                                 | 91.4 ms: 1.16x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 86.8 ms: 1.15x faster                                                            |
| json_loads               | 31.2 us                                                | 27.3 us: 1.14x faster                                                            |
| json                     | 5.69 ms                                                | 5.10 ms: 1.12x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                            |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.10x faster                                                             |
| pathlib                  | 20.5 ms                                                | 18.6 ms: 1.10x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.08x faster                                                             |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                           |
| unpickle_list            | 5.20 us                                                | 4.93 us: 1.06x faster                                                            |
| pickle_list              | 5.08 us                                                | 4.97 us: 1.02x faster                                                            |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| regex_dna                | 227 ms                                                 | 232 ms: 1.03x slower                                                             |
| gc_traversal             | 3.62 ms                                                | 3.72 ms: 1.03x slower                                                            |
| async_generators         | 444 ms                                                 | 463 ms: 1.04x slower                                                             |
| pickle                   | 10.7 us                                                | 11.7 us: 1.09x slower                                                            |
| unpickle                 | 14.4 us                                                | 16.2 us: 1.12x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.1 us: 1.15x slower                                                            |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.16x slower                                                            |
| telco                    | 7.27 ms                                                | 8.59 ms: 1.18x slower                                                            |
| coverage                 | 79.4 ms                                                | 96.3 ms: 1.21x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                            |
| unpack_sequence          | 60.0 ns                                                | 126 ns: 2.11x slower                                                             |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                                     |

Benchmark hidden because not significant (2): regex_effbot, mypy2
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240301-3.13.0a4+-c04ea6c-JIT/bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.34x