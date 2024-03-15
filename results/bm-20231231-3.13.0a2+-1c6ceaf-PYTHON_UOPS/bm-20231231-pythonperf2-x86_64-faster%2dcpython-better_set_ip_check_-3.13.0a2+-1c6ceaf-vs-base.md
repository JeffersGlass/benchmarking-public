# Results vs. base

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 1c6ceaf
- commit date: 2023-12-31
- overall geometric mean: 1.00x faster
- HPT reliability: 98.57%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 311 ms                                                                       | 309 ms: 1.01x faster                                                                   |
| chameleon      | 7.82 ms                                                                      | 8.09 ms: 1.03x slower                                                                  |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                                           |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_io, async_tree_none, async_tree_memoization, async_tree_io_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                                       | 263 ms: 1.01x faster                                                                   |
| float          | 102 ms                                                                       | 103 ms: 1.01x slower                                                                   |
| nbody          | 126 ms                                                                       | 129 ms: 1.02x slower                                                                   |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 173 ms                                                                       | 170 ms: 1.02x faster                                                                   |
| regex_v8       | 24.9 ms                                                                      | 25.5 ms: 1.02x slower                                                                  |
| regex_dna      | 236 ms                                                                       | 245 ms: 1.04x slower                                                                   |
| regex_effbot   | 3.44 ms                                                                      | 3.62 ms: 1.05x slower                                                                  |
| Geometric mean | (ref)                                                                        | 1.02x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|---------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| xml_etree_iterparse | 116 ms                                                                       | 112 ms: 1.03x faster                                                                   |
| pickle_list         | 4.35 us                                                                      | 4.23 us: 1.03x faster                                                                  |
| xml_etree_process   | 63.0 ms                                                                      | 61.5 ms: 1.03x faster                                                                  |
| xml_etree_generate  | 92.8 ms                                                                      | 90.5 ms: 1.03x faster                                                                  |
| tomli_loads         | 2.81 sec                                                                     | 2.75 sec: 1.02x faster                                                                 |
| json_loads          | 25.2 us                                                                      | 25.0 us: 1.01x faster                                                                  |
| pickle_dict         | 30.5 us                                                                      | 30.7 us: 1.00x slower                                                                  |
| pickle_pure_python  | 309 us                                                                       | 314 us: 1.02x slower                                                                   |
| unpickle_list       | 4.57 us                                                                      | 4.69 us: 1.03x slower                                                                  |
| unpickle            | 14.7 us                                                                      | 15.2 us: 1.03x slower                                                                  |
| Geometric mean      | (ref)                                                                        | 1.00x faster                                                                           |

Benchmark hidden because not significant (4): xml_etree_parse, pickle, json_dumps, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup_no_site | 11.0 ms                                                                      | 11.1 ms: 1.00x slower                                                                  |
| python_startup         | 12.5 ms                                                                      | 12.6 ms: 1.01x slower                                                                  |
| Geometric mean         | (ref)                                                                        | 1.01x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.6 ms                                                                      | 14.1 ms: 1.03x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|--------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| gc_traversal             | 3.79 ms                                                                      | 3.51 ms: 1.08x faster                                                                  |
| spectral_norm            | 172 ms                                                                       | 162 ms: 1.06x faster                                                                   |
| pyflate                  | 597 ms                                                                       | 567 ms: 1.05x faster                                                                   |
| scimark_sparse_mat_mult  | 6.52 ms                                                                      | 6.30 ms: 1.03x faster                                                                  |
| mako                     | 14.6 ms                                                                      | 14.1 ms: 1.03x faster                                                                  |
| xml_etree_iterparse      | 116 ms                                                                       | 112 ms: 1.03x faster                                                                   |
| pickle_list              | 4.35 us                                                                      | 4.23 us: 1.03x faster                                                                  |
| async_generators         | 370 ms                                                                       | 361 ms: 1.03x faster                                                                   |
| xml_etree_process        | 63.0 ms                                                                      | 61.5 ms: 1.03x faster                                                                  |
| xml_etree_generate       | 92.8 ms                                                                      | 90.5 ms: 1.03x faster                                                                  |
| nqueens                  | 110 ms                                                                       | 107 ms: 1.02x faster                                                                   |
| scimark_sor              | 148 ms                                                                       | 144 ms: 1.02x faster                                                                   |
| comprehensions           | 25.0 us                                                                      | 24.5 us: 1.02x faster                                                                  |
| tomli_loads              | 2.81 sec                                                                     | 2.75 sec: 1.02x faster                                                                 |
| typing_runtime_protocols | 127 us                                                                       | 124 us: 1.02x faster                                                                   |
| hexiom                   | 9.85 ms                                                                      | 9.70 ms: 1.02x faster                                                                  |
| regex_compile            | 173 ms                                                                       | 170 ms: 1.02x faster                                                                   |
| scimark_fft              | 429 ms                                                                       | 423 ms: 1.01x faster                                                                   |
| sqlglot_parse            | 1.46 ms                                                                      | 1.44 ms: 1.01x faster                                                                  |
| meteor_contest           | 140 ms                                                                       | 138 ms: 1.01x faster                                                                   |
| create_gc_cycles         | 1.63 ms                                                                      | 1.61 ms: 1.01x faster                                                                  |
| sqlglot_normalize        | 124 ms                                                                       | 122 ms: 1.01x faster                                                                   |
| sympy_str                | 327 ms                                                                       | 323 ms: 1.01x faster                                                                   |
| sympy_integrate          | 25.3 ms                                                                      | 25.0 ms: 1.01x faster                                                                  |
| sympy_sum                | 169 ms                                                                       | 167 ms: 1.01x faster                                                                   |
| pprint_safe_repr         | 929 ms                                                                       | 920 ms: 1.01x faster                                                                   |
| dulwich_log              | 72.4 ms                                                                      | 71.7 ms: 1.01x faster                                                                  |
| pprint_pformat           | 1.92 sec                                                                     | 1.90 sec: 1.01x faster                                                                 |
| scimark_lu               | 106 ms                                                                       | 105 ms: 1.01x faster                                                                   |
| sympy_expand             | 543 ms                                                                       | 538 ms: 1.01x faster                                                                   |
| json_loads               | 25.2 us                                                                      | 25.0 us: 1.01x faster                                                                  |
| scimark_monte_carlo      | 86.7 ms                                                                      | 86.1 ms: 1.01x faster                                                                  |
| crypto_pyaes             | 86.1 ms                                                                      | 85.4 ms: 1.01x faster                                                                  |
| sqlglot_transpile        | 1.87 ms                                                                      | 1.86 ms: 1.01x faster                                                                  |
| logging_format           | 7.49 us                                                                      | 7.45 us: 1.01x faster                                                                  |
| pidigits                 | 265 ms                                                                       | 263 ms: 1.01x faster                                                                   |
| 2to3                     | 311 ms                                                                       | 309 ms: 1.01x faster                                                                   |
| telco                    | 8.49 ms                                                                      | 8.45 ms: 1.00x faster                                                                  |
| mdp                      | 2.64 sec                                                                     | 2.62 sec: 1.00x faster                                                                 |
| sqlglot_optimize         | 63.6 ms                                                                      | 63.4 ms: 1.00x faster                                                                  |
| coroutines               | 22.0 ms                                                                      | 22.0 ms: 1.00x slower                                                                  |
| asyncio_tcp_ssl          | 1.59 sec                                                                     | 1.59 sec: 1.00x slower                                                                 |
| generators               | 33.8 ms                                                                      | 33.9 ms: 1.00x slower                                                                  |
| pickle_dict              | 30.5 us                                                                      | 30.7 us: 1.00x slower                                                                  |
| python_startup_no_site   | 11.0 ms                                                                      | 11.1 ms: 1.00x slower                                                                  |
| python_startup           | 12.5 ms                                                                      | 12.6 ms: 1.01x slower                                                                  |
| logging_simple           | 6.80 us                                                                      | 6.84 us: 1.01x slower                                                                  |
| fannkuch                 | 475 ms                                                                       | 478 ms: 1.01x slower                                                                   |
| float                    | 102 ms                                                                       | 103 ms: 1.01x slower                                                                   |
| deltablue                | 5.37 ms                                                                      | 5.42 ms: 1.01x slower                                                                  |
| deepcopy_memo            | 39.8 us                                                                      | 40.3 us: 1.01x slower                                                                  |
| go                       | 180 ms                                                                       | 182 ms: 1.01x slower                                                                   |
| pickle_pure_python       | 309 us                                                                       | 314 us: 1.02x slower                                                                   |
| deepcopy                 | 381 us                                                                       | 388 us: 1.02x slower                                                                   |
| pycparser                | 1.32 sec                                                                     | 1.34 sec: 1.02x slower                                                                 |
| regex_v8                 | 24.9 ms                                                                      | 25.5 ms: 1.02x slower                                                                  |
| pathlib                  | 19.3 ms                                                                      | 19.7 ms: 1.02x slower                                                                  |
| nbody                    | 126 ms                                                                       | 129 ms: 1.02x slower                                                                   |
| deepcopy_reduce          | 3.36 us                                                                      | 3.45 us: 1.03x slower                                                                  |
| unpickle_list            | 4.57 us                                                                      | 4.69 us: 1.03x slower                                                                  |
| richards_super           | 59.6 ms                                                                      | 61.3 ms: 1.03x slower                                                                  |
| unpickle                 | 14.7 us                                                                      | 15.2 us: 1.03x slower                                                                  |
| chameleon                | 7.82 ms                                                                      | 8.09 ms: 1.03x slower                                                                  |
| regex_dna                | 236 ms                                                                       | 245 ms: 1.04x slower                                                                   |
| richards                 | 52.8 ms                                                                      | 54.7 ms: 1.04x slower                                                                  |
| coverage                 | 79.9 ms                                                                      | 83.2 ms: 1.04x slower                                                                  |
| regex_effbot             | 3.44 ms                                                                      | 3.62 ms: 1.05x slower                                                                  |
| Geometric mean           | (ref)                                                                        | 1.00x faster                                                                           |

Benchmark hidden because not significant (26): bench_mp_pool, xml_etree_parse, async_tree_cpu_io_mixed_tg, pickle, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_io, async_tree_none, sqlite_synth, async_tree_memoization, bench_thread_pool, tornado_http, async_tree_io_tg, json, docutils, async_tree_memoization_tg, raytrace, chaos, unpack_sequence, json_dumps, logging_silent, asyncio_tcp, unpickle_pure_python, mypy2, dask, asyncio_websockets


# HPT report

- Reliability score: 98.57% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x