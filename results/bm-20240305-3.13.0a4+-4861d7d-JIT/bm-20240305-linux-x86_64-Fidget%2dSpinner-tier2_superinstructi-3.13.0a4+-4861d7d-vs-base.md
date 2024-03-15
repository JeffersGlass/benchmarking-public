# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_superinstructi
- machine: linux-x86_64
- commit hash: 4861d7d
- commit date: 2024-03-05
- overall geometric mean: 1.00x faster
- HPT reliability: 94.61%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg | 448 ms                                                                 | 445 ms: 1.00x faster                                                             |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_io, async_tree_none, async_tree_io_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 95.4 ms                                                                | 92.3 ms: 1.03x faster                                                            |
| float          | 79.2 ms                                                                | 77.8 ms: 1.02x faster                                                            |
| pidigits       | 188 ms                                                                 | 186 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 226 ms                                                                 | 215 ms: 1.05x faster                                                             |
| regex_compile  | 143 ms                                                                 | 141 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (2): regex_v8, regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle               | 11.8 us                                                                | 11.6 us: 1.02x faster                                                            |
| unpickle_list        | 4.90 us                                                                | 4.85 us: 1.01x faster                                                            |
| xml_etree_process    | 58.7 ms                                                                | 59.2 ms: 1.01x slower                                                            |
| unpickle_pure_python | 233 us                                                                 | 236 us: 1.01x slower                                                             |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (8): json_loads, json_dumps, xml_etree_generate, pickle_dict, pickle_list, tomli_loads, xml_etree_parse, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 10.9 ms                                                                | 10.9 ms: 1.00x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.8 ms                                                                | 10.8 ms: 1.00x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-4861d7d |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| raytrace                 | 288 ms                                                                 | 266 ms: 1.08x faster                                                             |
| gc_traversal             | 4.03 ms                                                                | 3.76 ms: 1.07x faster                                                            |
| regex_dna                | 226 ms                                                                 | 215 ms: 1.05x faster                                                             |
| spectral_norm            | 112 ms                                                                 | 108 ms: 1.04x faster                                                             |
| nbody                    | 95.4 ms                                                                | 92.3 ms: 1.03x faster                                                            |
| pycparser                | 1.20 sec                                                               | 1.18 sec: 1.02x faster                                                           |
| pickle                   | 11.8 us                                                                | 11.6 us: 1.02x faster                                                            |
| deepcopy_reduce          | 3.06 us                                                                | 3.01 us: 1.02x faster                                                            |
| float                    | 79.2 ms                                                                | 77.8 ms: 1.02x faster                                                            |
| regex_compile            | 143 ms                                                                 | 141 ms: 1.01x faster                                                             |
| pprint_safe_repr         | 745 ms                                                                 | 734 ms: 1.01x faster                                                             |
| typing_runtime_protocols | 110 us                                                                 | 109 us: 1.01x faster                                                             |
| unpickle_list            | 4.90 us                                                                | 4.85 us: 1.01x faster                                                            |
| coroutines               | 22.7 ms                                                                | 22.4 ms: 1.01x faster                                                            |
| logging_format           | 6.23 us                                                                | 6.19 us: 1.01x faster                                                            |
| sympy_str                | 280 ms                                                                 | 278 ms: 1.01x faster                                                             |
| sqlglot_parse            | 1.29 ms                                                                | 1.29 ms: 1.01x faster                                                            |
| logging_simple           | 5.67 us                                                                | 5.63 us: 1.01x faster                                                            |
| pidigits                 | 188 ms                                                                 | 186 ms: 1.01x faster                                                             |
| async_tree_none_tg       | 448 ms                                                                 | 445 ms: 1.00x faster                                                             |
| bench_thread_pool        | 846 us                                                                 | 843 us: 1.00x faster                                                             |
| mako                     | 10.8 ms                                                                | 10.8 ms: 1.00x faster                                                            |
| sympy_integrate          | 20.9 ms                                                                | 20.8 ms: 1.00x faster                                                            |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                           |
| python_startup_no_site   | 10.9 ms                                                                | 10.9 ms: 1.00x slower                                                            |
| create_gc_cycles         | 1.50 ms                                                                | 1.50 ms: 1.00x slower                                                            |
| dulwich_log              | 68.1 ms                                                                | 68.3 ms: 1.00x slower                                                            |
| hexiom                   | 6.95 ms                                                                | 6.98 ms: 1.00x slower                                                            |
| pathlib                  | 18.3 ms                                                                | 18.4 ms: 1.01x slower                                                            |
| xml_etree_process        | 58.7 ms                                                                | 59.2 ms: 1.01x slower                                                            |
| unpickle_pure_python     | 233 us                                                                 | 236 us: 1.01x slower                                                             |
| async_generators         | 462 ms                                                                 | 466 ms: 1.01x slower                                                             |
| sqlglot_normalize        | 106 ms                                                                 | 107 ms: 1.01x slower                                                             |
| comprehensions           | 17.0 us                                                                | 17.3 us: 1.02x slower                                                            |
| asyncio_tcp              | 479 ms                                                                 | 489 ms: 1.02x slower                                                             |
| mdp                      | 2.61 sec                                                               | 2.66 sec: 1.02x slower                                                           |
| unpack_sequence          | 85.0 ns                                                                | 87.0 ns: 1.02x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (44): crypto_pyaes, mypy2, sqlglot_transpile, pprint_pformat, async_tree_cpu_io_mixed_tg, richards_super, async_tree_cpu_io_mixed, deepcopy_memo, json_loads, chaos, asyncio_websockets, tornado_http, json_dumps, logging_silent, sympy_sum, xml_etree_generate, dask, pickle_dict, async_tree_memoization_tg, deepcopy, regex_v8, python_startup, meteor_contest, sympy_expand, pickle_list, go, richards, async_tree_io, pyflate, async_tree_none, async_tree_io_tg, regex_effbot, fannkuch, deltablue, tomli_loads, xml_etree_parse, coverage, async_tree_memoization, xml_etree_iterparse, sqlglot_optimize, sqlite_synth, nqueens, json, bench_mp_pool
Ignored benchmarks (12) of results/bm-20240304-3.13.0a4+-ffed8d9-JIT/bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9.json: 2to3, chameleon, docutils, generators, pickle_pure_python, scimark_fft, scimark_lu, scimark_monte_carlo, scimark_sor, scimark_sparse_mat_mult, telco, unpickle


# HPT report

- Reliability score: 94.61% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x