# Results vs. base

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.00x slower
- HPT reliability: 74.20%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                                                            | 264 ms: 1.00x slower                                                                                                  |
| chameleon      | 6.97 ms                                                                                                           | 6.90 ms: 1.01x faster                                                                                                 |
| docutils       | 2.61 sec                                                                                                          | 2.59 sec: 1.01x faster                                                                                                |
| Geometric mean | (ref)                                                                                                             | 1.00x faster                                                                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|--------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| async_tree_io_tg   | 1.20 sec                                                                                                          | 1.19 sec: 1.01x faster                                                                                                |
| async_tree_none_tg | 441 ms                                                                                                            | 438 ms: 1.01x faster                                                                                                  |
| async_tree_io      | 1.18 sec                                                                                                          | 1.17 sec: 1.01x faster                                                                                                |
| Geometric mean     | (ref)                                                                                                             | 1.00x faster                                                                                                          |

Benchmark hidden because not significant (5): async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 195 ms                                                                                                            | 187 ms: 1.04x faster                                                                                                  |
| nbody          | 88.9 ms                                                                                                           | 87.4 ms: 1.02x faster                                                                                                 |
| float          | 79.4 ms                                                                                                           | 79.7 ms: 1.00x slower                                                                                                 |
| Geometric mean | (ref)                                                                                                             | 1.02x faster                                                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 3.77 ms                                                                                                           | 3.65 ms: 1.03x faster                                                                                                 |
| regex_v8       | 25.3 ms                                                                                                           | 25.0 ms: 1.01x faster                                                                                                 |
| regex_dna      | 224 ms                                                                                                            | 223 ms: 1.00x faster                                                                                                  |
| regex_compile  | 129 ms                                                                                                            | 130 ms: 1.00x slower                                                                                                  |
| Geometric mean | (ref)                                                                                                             | 1.01x faster                                                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| unpickle_list        | 5.13 us                                                                                                           | 5.05 us: 1.02x faster                                                                                                 |
| unpickle             | 15.0 us                                                                                                           | 14.9 us: 1.00x faster                                                                                                 |
| xml_etree_generate   | 84.9 ms                                                                                                           | 85.1 ms: 1.00x slower                                                                                                 |
| json_dumps           | 10.5 ms                                                                                                           | 10.5 ms: 1.01x slower                                                                                                 |
| tomli_loads          | 2.11 sec                                                                                                          | 2.13 sec: 1.01x slower                                                                                                |
| xml_etree_parse      | 156 ms                                                                                                            | 157 ms: 1.01x slower                                                                                                  |
| pickle_pure_python   | 300 us                                                                                                            | 302 us: 1.01x slower                                                                                                  |
| unpickle_pure_python | 213 us                                                                                                            | 216 us: 1.01x slower                                                                                                  |
| pickle               | 11.5 us                                                                                                           | 11.7 us: 1.01x slower                                                                                                 |
| pickle_list          | 4.92 us                                                                                                           | 5.20 us: 1.06x slower                                                                                                 |
| pickle_dict          | 33.4 us                                                                                                           | 35.5 us: 1.06x slower                                                                                                 |
| Geometric mean       | (ref)                                                                                                             | 1.01x slower                                                                                                          |

Benchmark hidden because not significant (3): json_loads, xml_etree_process, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                                                           | 10.1 ms: 1.00x faster                                                                                                 |
| python_startup_no_site | 8.70 ms                                                                                                           | 8.71 ms: 1.00x slower                                                                                                 |
| Geometric mean         | (ref)                                                                                                             | 1.00x slower                                                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| mako      | 11.1 ms                                                                                                           | 11.2 ms: 1.01x slower                                                                                                 |

All benchmarks:
===============

| Benchmark                | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-JIT/bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|--------------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| spectral_norm            | 114 ms                                                                                                            | 109 ms: 1.04x faster                                                                                                  |
| nqueens                  | 83.9 ms                                                                                                           | 80.6 ms: 1.04x faster                                                                                                 |
| pidigits                 | 195 ms                                                                                                            | 187 ms: 1.04x faster                                                                                                  |
| regex_effbot             | 3.77 ms                                                                                                           | 3.65 ms: 1.03x faster                                                                                                 |
| hexiom                   | 6.20 ms                                                                                                           | 6.07 ms: 1.02x faster                                                                                                 |
| pyflate                  | 464 ms                                                                                                            | 455 ms: 1.02x faster                                                                                                  |
| crypto_pyaes             | 71.3 ms                                                                                                           | 70.0 ms: 1.02x faster                                                                                                 |
| nbody                    | 88.9 ms                                                                                                           | 87.4 ms: 1.02x faster                                                                                                 |
| unpickle_list            | 5.13 us                                                                                                           | 5.05 us: 1.02x faster                                                                                                 |
| scimark_sparse_mat_mult  | 4.93 ms                                                                                                           | 4.87 ms: 1.01x faster                                                                                                 |
| coverage                 | 96.2 ms                                                                                                           | 95.0 ms: 1.01x faster                                                                                                 |
| regex_v8                 | 25.3 ms                                                                                                           | 25.0 ms: 1.01x faster                                                                                                 |
| deepcopy_reduce          | 3.05 us                                                                                                           | 3.02 us: 1.01x faster                                                                                                 |
| pathlib                  | 18.5 ms                                                                                                           | 18.3 ms: 1.01x faster                                                                                                 |
| scimark_monte_carlo      | 68.3 ms                                                                                                           | 67.6 ms: 1.01x faster                                                                                                 |
| chameleon                | 6.97 ms                                                                                                           | 6.90 ms: 1.01x faster                                                                                                 |
| asyncio_tcp              | 484 ms                                                                                                            | 480 ms: 1.01x faster                                                                                                  |
| pprint_pformat           | 1.49 sec                                                                                                          | 1.48 sec: 1.01x faster                                                                                                |
| gc_traversal             | 3.72 ms                                                                                                           | 3.69 ms: 1.01x faster                                                                                                 |
| typing_runtime_protocols | 112 us                                                                                                            | 111 us: 1.01x faster                                                                                                  |
| async_tree_io_tg         | 1.20 sec                                                                                                          | 1.19 sec: 1.01x faster                                                                                                |
| generators               | 29.6 ms                                                                                                           | 29.4 ms: 1.01x faster                                                                                                 |
| pycparser                | 1.20 sec                                                                                                          | 1.19 sec: 1.01x faster                                                                                                |
| docutils                 | 2.61 sec                                                                                                          | 2.59 sec: 1.01x faster                                                                                                |
| async_tree_none_tg       | 441 ms                                                                                                            | 438 ms: 1.01x faster                                                                                                  |
| async_tree_io            | 1.18 sec                                                                                                          | 1.17 sec: 1.01x faster                                                                                                |
| pprint_safe_repr         | 728 ms                                                                                                            | 724 ms: 1.01x faster                                                                                                  |
| asyncio_tcp_ssl          | 1.78 sec                                                                                                          | 1.77 sec: 1.01x faster                                                                                                |
| chaos                    | 59.2 ms                                                                                                           | 58.9 ms: 1.00x faster                                                                                                 |
| regex_dna                | 224 ms                                                                                                            | 223 ms: 1.00x faster                                                                                                  |
| unpickle                 | 15.0 us                                                                                                           | 14.9 us: 1.00x faster                                                                                                 |
| python_startup           | 10.1 ms                                                                                                           | 10.1 ms: 1.00x faster                                                                                                 |
| python_startup_no_site   | 8.70 ms                                                                                                           | 8.71 ms: 1.00x slower                                                                                                 |
| xml_etree_generate       | 84.9 ms                                                                                                           | 85.1 ms: 1.00x slower                                                                                                 |
| 2to3                     | 263 ms                                                                                                            | 264 ms: 1.00x slower                                                                                                  |
| float                    | 79.4 ms                                                                                                           | 79.7 ms: 1.00x slower                                                                                                 |
| regex_compile            | 129 ms                                                                                                            | 130 ms: 1.00x slower                                                                                                  |
| json_dumps               | 10.5 ms                                                                                                           | 10.5 ms: 1.01x slower                                                                                                 |
| raytrace                 | 260 ms                                                                                                            | 262 ms: 1.01x slower                                                                                                  |
| tomli_loads              | 2.11 sec                                                                                                          | 2.13 sec: 1.01x slower                                                                                                |
| xml_etree_parse          | 156 ms                                                                                                            | 157 ms: 1.01x slower                                                                                                  |
| meteor_contest           | 107 ms                                                                                                            | 108 ms: 1.01x slower                                                                                                  |
| sqlite_synth             | 2.82 us                                                                                                           | 2.85 us: 1.01x slower                                                                                                 |
| deltablue                | 3.23 ms                                                                                                           | 3.26 ms: 1.01x slower                                                                                                 |
| mako                     | 11.1 ms                                                                                                           | 11.2 ms: 1.01x slower                                                                                                 |
| pickle_pure_python       | 300 us                                                                                                            | 302 us: 1.01x slower                                                                                                  |
| sqlglot_optimize         | 53.4 ms                                                                                                           | 53.9 ms: 1.01x slower                                                                                                 |
| unpickle_pure_python     | 213 us                                                                                                            | 216 us: 1.01x slower                                                                                                  |
| sqlglot_parse            | 1.24 ms                                                                                                           | 1.25 ms: 1.01x slower                                                                                                 |
| pickle                   | 11.5 us                                                                                                           | 11.7 us: 1.01x slower                                                                                                 |
| deepcopy_memo            | 37.9 us                                                                                                           | 38.4 us: 1.01x slower                                                                                                 |
| scimark_lu               | 111 ms                                                                                                            | 112 ms: 1.01x slower                                                                                                  |
| sqlglot_normalize        | 106 ms                                                                                                            | 108 ms: 1.02x slower                                                                                                  |
| richards                 | 47.4 ms                                                                                                           | 48.3 ms: 1.02x slower                                                                                                 |
| sympy_expand             | 457 ms                                                                                                            | 465 ms: 1.02x slower                                                                                                  |
| richards_super           | 53.8 ms                                                                                                           | 55.0 ms: 1.02x slower                                                                                                 |
| sympy_str                | 269 ms                                                                                                            | 276 ms: 1.02x slower                                                                                                  |
| scimark_fft              | 352 ms                                                                                                            | 362 ms: 1.03x slower                                                                                                  |
| coroutines               | 21.6 ms                                                                                                           | 22.4 ms: 1.04x slower                                                                                                 |
| pickle_list              | 4.92 us                                                                                                           | 5.20 us: 1.06x slower                                                                                                 |
| pickle_dict              | 33.4 us                                                                                                           | 35.5 us: 1.06x slower                                                                                                 |
| unpack_sequence          | 40.5 ns                                                                                                           | 44.4 ns: 1.10x slower                                                                                                 |
| Geometric mean           | (ref)                                                                                                             | 1.00x slower                                                                                                          |

Benchmark hidden because not significant (31): json, scimark_sor, tornado_http, mypy2, fannkuch, create_gc_cycles, dulwich_log, async_tree_none, deepcopy, async_tree_cpu_io_mixed_tg, bench_thread_pool, logging_format, bench_mp_pool, dask, async_tree_memoization, sympy_integrate, json_loads, mdp, async_tree_memoization_tg, comprehensions, sympy_sum, logging_silent, asyncio_websockets, async_generators, xml_etree_process, sqlglot_transpile, go, async_tree_cpu_io_mixed, telco, logging_simple, xml_etree_iterparse


# HPT report

- Reliability score: 74.20% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x