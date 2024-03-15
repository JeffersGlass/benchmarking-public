# Results vs. base

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: f5a8425
- commit date: 2024-01-23
- overall geometric mean: 1.00x faster
- HPT reliability: 52.52%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 262 ms                                                                 | 263 ms: 1.00x slower                                               |
| chameleon      | 6.95 ms                                                                | 6.87 ms: 1.01x faster                                              |
| docutils       | 2.61 sec                                                               | 2.64 sec: 1.01x slower                                             |
| tornado_http   | 94.2 ms                                                                | 94.8 ms: 1.01x slower                                              |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_io    | 1.17 sec                                                               | 1.18 sec: 1.00x slower                                             |
| async_tree_io_tg | 1.19 sec                                                               | 1.19 sec: 1.01x slower                                             |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                       |

Benchmark hidden because not significant (6): async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_none, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 89.4 ms                                                                | 88.6 ms: 1.01x faster                                              |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                               |
| float          | 79.9 ms                                                                | 80.5 ms: 1.01x slower                                              |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_effbot   | 3.74 ms                                                                | 3.55 ms: 1.05x faster                                              |
| regex_v8       | 25.8 ms                                                                | 25.4 ms: 1.02x faster                                              |
| regex_dna      | 223 ms                                                                 | 221 ms: 1.01x faster                                               |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                       |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|---------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| unpickle            | 15.3 us                                                                | 14.9 us: 1.03x faster                                              |
| pickle              | 11.8 us                                                                | 11.6 us: 1.02x faster                                              |
| pickle_dict         | 34.5 us                                                                | 34.0 us: 1.01x faster                                              |
| pickle_pure_python  | 297 us                                                                 | 299 us: 1.01x slower                                               |
| xml_etree_iterparse | 104 ms                                                                 | 105 ms: 1.01x slower                                               |
| xml_etree_process   | 58.4 ms                                                                | 58.8 ms: 1.01x slower                                              |
| xml_etree_generate  | 85.4 ms                                                                | 86.3 ms: 1.01x slower                                              |
| xml_etree_parse     | 157 ms                                                                 | 159 ms: 1.01x slower                                               |
| unpickle_list       | 5.25 us                                                                | 5.32 us: 1.01x slower                                              |
| tomli_loads         | 2.11 sec                                                               | 2.14 sec: 1.02x slower                                             |
| pickle_list         | 4.94 us                                                                | 5.11 us: 1.03x slower                                              |
| Geometric mean      | (ref)                                                                  | 1.00x slower                                                       |

Benchmark hidden because not significant (3): json_loads, json_dumps, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup_no_site | 8.71 ms                                                                | 8.73 ms: 1.00x slower                                              |
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                              |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|-----------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 11.0 ms: 1.01x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|--------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| gc_traversal             | 4.16 ms                                                                | 3.74 ms: 1.11x faster                                              |
| mdp                      | 2.70 sec                                                               | 2.53 sec: 1.07x faster                                             |
| scimark_sor              | 127 ms                                                                 | 121 ms: 1.05x faster                                               |
| regex_effbot             | 3.74 ms                                                                | 3.55 ms: 1.05x faster                                              |
| unpickle                 | 15.3 us                                                                | 14.9 us: 1.03x faster                                              |
| scimark_monte_carlo      | 68.5 ms                                                                | 66.6 ms: 1.03x faster                                              |
| pycparser                | 1.19 sec                                                               | 1.16 sec: 1.02x faster                                             |
| deepcopy                 | 347 us                                                                 | 339 us: 1.02x faster                                               |
| chaos                    | 59.9 ms                                                                | 58.7 ms: 1.02x faster                                              |
| nqueens                  | 80.9 ms                                                                | 79.4 ms: 1.02x faster                                              |
| regex_v8                 | 25.8 ms                                                                | 25.4 ms: 1.02x faster                                              |
| raytrace                 | 264 ms                                                                 | 260 ms: 1.02x faster                                               |
| pickle                   | 11.8 us                                                                | 11.6 us: 1.02x faster                                              |
| telco                    | 8.48 ms                                                                | 8.33 ms: 1.02x faster                                              |
| richards                 | 48.1 ms                                                                | 47.4 ms: 1.02x faster                                              |
| coroutines               | 22.3 ms                                                                | 21.9 ms: 1.02x faster                                              |
| richards_super           | 54.0 ms                                                                | 53.2 ms: 1.01x faster                                              |
| go                       | 139 ms                                                                 | 137 ms: 1.01x faster                                               |
| pyflate                  | 465 ms                                                                 | 458 ms: 1.01x faster                                               |
| pickle_dict              | 34.5 us                                                                | 34.0 us: 1.01x faster                                              |
| fannkuch                 | 407 ms                                                                 | 402 ms: 1.01x faster                                               |
| deepcopy_reduce          | 3.03 us                                                                | 2.99 us: 1.01x faster                                              |
| chameleon                | 6.95 ms                                                                | 6.87 ms: 1.01x faster                                              |
| mako                     | 11.1 ms                                                                | 11.0 ms: 1.01x faster                                              |
| deepcopy_memo            | 37.7 us                                                                | 37.3 us: 1.01x faster                                              |
| typing_runtime_protocols | 110 us                                                                 | 109 us: 1.01x faster                                               |
| nbody                    | 89.4 ms                                                                | 88.6 ms: 1.01x faster                                              |
| coverage                 | 94.8 ms                                                                | 93.9 ms: 1.01x faster                                              |
| pprint_pformat           | 1.50 sec                                                               | 1.49 sec: 1.01x faster                                             |
| regex_dna                | 223 ms                                                                 | 221 ms: 1.01x faster                                               |
| async_generators         | 443 ms                                                                 | 441 ms: 1.01x faster                                               |
| pidigits                 | 188 ms                                                                 | 187 ms: 1.00x faster                                               |
| 2to3                     | 262 ms                                                                 | 263 ms: 1.00x slower                                               |
| python_startup_no_site   | 8.71 ms                                                                | 8.73 ms: 1.00x slower                                              |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                              |
| scimark_fft              | 359 ms                                                                 | 360 ms: 1.00x slower                                               |
| hexiom                   | 6.11 ms                                                                | 6.13 ms: 1.00x slower                                              |
| async_tree_io            | 1.17 sec                                                               | 1.18 sec: 1.00x slower                                             |
| sympy_sum                | 148 ms                                                                 | 149 ms: 1.00x slower                                               |
| async_tree_io_tg         | 1.19 sec                                                               | 1.19 sec: 1.01x slower                                             |
| pickle_pure_python       | 297 us                                                                 | 299 us: 1.01x slower                                               |
| asyncio_tcp              | 479 ms                                                                 | 482 ms: 1.01x slower                                               |
| xml_etree_iterparse      | 104 ms                                                                 | 105 ms: 1.01x slower                                               |
| tornado_http             | 94.2 ms                                                                | 94.8 ms: 1.01x slower                                              |
| create_gc_cycles         | 1.46 ms                                                                | 1.47 ms: 1.01x slower                                              |
| float                    | 79.9 ms                                                                | 80.5 ms: 1.01x slower                                              |
| sqlglot_transpile        | 1.57 ms                                                                | 1.58 ms: 1.01x slower                                              |
| xml_etree_process        | 58.4 ms                                                                | 58.8 ms: 1.01x slower                                              |
| sqlglot_parse            | 1.24 ms                                                                | 1.25 ms: 1.01x slower                                              |
| docutils                 | 2.61 sec                                                               | 2.64 sec: 1.01x slower                                             |
| meteor_contest           | 108 ms                                                                 | 109 ms: 1.01x slower                                               |
| xml_etree_generate       | 85.4 ms                                                                | 86.3 ms: 1.01x slower                                              |
| xml_etree_parse          | 157 ms                                                                 | 159 ms: 1.01x slower                                               |
| bench_thread_pool        | 824 us                                                                 | 835 us: 1.01x slower                                               |
| deltablue                | 3.17 ms                                                                | 3.22 ms: 1.01x slower                                              |
| generators               | 29.0 ms                                                                | 29.4 ms: 1.01x slower                                              |
| unpickle_list            | 5.25 us                                                                | 5.32 us: 1.01x slower                                              |
| tomli_loads              | 2.11 sec                                                               | 2.14 sec: 1.02x slower                                             |
| scimark_sparse_mat_mult  | 4.60 ms                                                                | 4.69 ms: 1.02x slower                                              |
| pathlib                  | 18.0 ms                                                                | 18.3 ms: 1.02x slower                                              |
| pickle_list              | 4.94 us                                                                | 5.11 us: 1.03x slower                                              |
| unpack_sequence          | 48.1 ns                                                                | 55.0 ns: 1.14x slower                                              |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                       |

Benchmark hidden because not significant (31): sqlite_synth, json_loads, json_dumps, logging_simple, comprehensions, logging_silent, bench_mp_pool, pprint_safe_repr, scimark_lu, asyncio_websockets, asyncio_tcp_ssl, sqlglot_optimize, regex_compile, crypto_pyaes, dask, spectral_norm, async_tree_none_tg, sympy_integrate, logging_format, sqlglot_normalize, dulwich_log, json, mypy2, sympy_expand, unpickle_pure_python, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_none, async_tree_memoization_tg, sympy_str


# HPT report

- Reliability score: 52.52% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x