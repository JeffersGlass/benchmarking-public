# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_superinstructi
- machine: linux-x86_64
- commit hash: 4861d7d
- commit date: 2024-03-05
- overall geometric mean: 1.01x faster \*
- HPT reliability: 98.90%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark    | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|--------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tornado_http | 103 ms                                                 | 96.8 ms: 1.06x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 438 ms: 1.08x faster                                                             |
| async_tree_cpu_io_mixed | 726 ms                                                 | 705 ms: 1.03x faster                                                             |
| async_tree_memoization  | 578 ms                                                 | 563 ms: 1.03x faster                                                             |
| async_tree_none_tg      | 450 ms                                                 | 445 ms: 1.01x faster                                                             |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                           |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 77.8 ms: 1.09x faster                                                            |
| nbody          | 97.0 ms                                                | 92.3 ms: 1.05x faster                                                            |
| pidigits       | 187 ms                                                 | 186 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                  | 1.05x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 141 ms: 1.06x faster                                                             |
| regex_dna      | 212 ms                                                 | 215 ms: 1.01x slower                                                             |
| regex_effbot   | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                            |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.02 sec: 1.15x faster                                                           |
| unpickle_list        | 5.29 us                                                | 4.85 us: 1.09x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                            |
| json_loads           | 28.5 us                                                | 27.3 us: 1.04x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 86.0 ms: 1.04x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.00x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.17 us: 1.02x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 236 us: 1.02x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                                     |

Benchmark hidden because not significant (2): pickle, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 10.9 ms: 1.58x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.42x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 109 us: 1.45x faster                                                             |
| comprehensions           | 21.8 us                                                | 17.3 us: 1.26x faster                                                            |
| raytrace                 | 312 ms                                                 | 266 ms: 1.17x faster                                                             |
| logging_format           | 7.23 us                                                | 6.19 us: 1.17x faster                                                            |
| tomli_loads              | 2.33 sec                                               | 2.02 sec: 1.15x faster                                                           |
| logging_simple           | 6.46 us                                                | 5.63 us: 1.15x faster                                                            |
| crypto_pyaes             | 81.9 ms                                                | 73.4 ms: 1.11x faster                                                            |
| deepcopy_reduce          | 3.35 us                                                | 3.01 us: 1.11x faster                                                            |
| mako                     | 11.9 ms                                                | 10.8 ms: 1.10x faster                                                            |
| deltablue                | 3.72 ms                                                | 3.39 ms: 1.10x faster                                                            |
| unpickle_list            | 5.29 us                                                | 4.85 us: 1.09x faster                                                            |
| float                    | 84.7 ms                                                | 77.8 ms: 1.09x faster                                                            |
| sympy_sum                | 169 ms                                                 | 157 ms: 1.08x faster                                                             |
| sympy_str                | 300 ms                                                 | 278 ms: 1.08x faster                                                             |
| chaos                    | 67.0 ms                                                | 62.2 ms: 1.08x faster                                                            |
| async_tree_none          | 472 ms                                                 | 438 ms: 1.08x faster                                                             |
| spectral_norm            | 115 ms                                                 | 108 ms: 1.07x faster                                                             |
| fannkuch                 | 417 ms                                                 | 393 ms: 1.06x faster                                                             |
| tornado_http             | 103 ms                                                 | 96.8 ms: 1.06x faster                                                            |
| deepcopy                 | 371 us                                                 | 350 us: 1.06x faster                                                             |
| sqlglot_parse            | 1.36 ms                                                | 1.29 ms: 1.06x faster                                                            |
| pprint_safe_repr         | 776 ms                                                 | 734 ms: 1.06x faster                                                             |
| regex_compile            | 148 ms                                                 | 141 ms: 1.06x faster                                                             |
| deepcopy_memo            | 40.7 us                                                | 38.7 us: 1.05x faster                                                            |
| nbody                    | 97.0 ms                                                | 92.3 ms: 1.05x faster                                                            |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                            |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                                             |
| xml_etree_process        | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                            |
| json_loads               | 28.5 us                                                | 27.3 us: 1.04x faster                                                            |
| logging_silent           | 104 ns                                                 | 100 ns: 1.04x faster                                                             |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                            |
| json                     | 5.26 ms                                                | 5.06 ms: 1.04x faster                                                            |
| xml_etree_generate       | 89.2 ms                                                | 86.0 ms: 1.04x faster                                                            |
| coroutines               | 23.2 ms                                                | 22.4 ms: 1.03x faster                                                            |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 705 ms: 1.03x faster                                                             |
| sympy_integrate          | 21.4 ms                                                | 20.8 ms: 1.03x faster                                                            |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.03x faster                                                             |
| async_tree_memoization   | 578 ms                                                 | 563 ms: 1.03x faster                                                             |
| pyflate                  | 482 ms                                                 | 470 ms: 1.03x faster                                                             |
| pprint_pformat           | 1.57 sec                                               | 1.53 sec: 1.02x faster                                                           |
| pickle_dict              | 35.5 us                                                | 34.8 us: 1.02x faster                                                            |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| sqlite_synth             | 2.83 us                                                | 2.80 us: 1.01x faster                                                            |
| gc_traversal             | 3.79 ms                                                | 3.76 ms: 1.01x faster                                                            |
| async_tree_none_tg       | 450 ms                                                 | 445 ms: 1.01x faster                                                             |
| sympy_expand             | 478 ms                                                 | 475 ms: 1.01x faster                                                             |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.00x faster                                                            |
| pidigits                 | 187 ms                                                 | 186 ms: 1.00x faster                                                             |
| asyncio_tcp              | 491 ms                                                 | 489 ms: 1.00x faster                                                             |
| dulwich_log              | 68.5 ms                                                | 68.3 ms: 1.00x faster                                                            |
| async_generators         | 463 ms                                                 | 466 ms: 1.01x slower                                                             |
| richards_super           | 51.5 ms                                                | 52.0 ms: 1.01x slower                                                            |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| mdp                      | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                           |
| regex_dna                | 212 ms                                                 | 215 ms: 1.01x slower                                                             |
| pickle_list              | 5.08 us                                                | 5.17 us: 1.02x slower                                                            |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                            |
| regex_effbot             | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                            |
| sqlglot_optimize         | 54.8 ms                                                | 55.9 ms: 1.02x slower                                                            |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                           |
| unpickle_pure_python     | 230 us                                                 | 236 us: 1.02x slower                                                             |
| hexiom                   | 6.41 ms                                                | 6.98 ms: 1.09x slower                                                            |
| nqueens                  | 83.3 ms                                                | 90.6 ms: 1.09x slower                                                            |
| regex_v8                 | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| go                       | 139 ms                                                 | 156 ms: 1.12x slower                                                             |
| bench_mp_pool            | 24.0 ms                                                | 28.2 ms: 1.17x slower                                                            |
| python_startup           | 9.55 ms                                                | 12.3 ms: 1.29x slower                                                            |
| coverage                 | 72.7 ms                                                | 97.3 ms: 1.34x slower                                                            |
| dask                     | 372 ms                                                 | 531 ms: 1.43x slower                                                             |
| python_startup_no_site   | 6.94 ms                                                | 10.9 ms: 1.58x slower                                                            |
| unpack_sequence          | 54.0 ns                                                | 87.0 ns: 1.61x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (9): async_tree_cpu_io_mixed_tg, pycparser, pickle, async_tree_memoization_tg, xml_etree_iterparse, richards, bench_thread_pool, asyncio_websockets, mypy2
Ignored benchmarks (17) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: 2to3, aiohttp, chameleon, django_template, docutils, generators, gunicorn, pickle_pure_python, scimark_fft, scimark_lu, scimark_monte_carlo, scimark_sor, scimark_sparse_mat_mult, sqlalchemy_declarative, sqlalchemy_imperative, telco, unpickle


# HPT report

- Reliability score: 98.90% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.17x