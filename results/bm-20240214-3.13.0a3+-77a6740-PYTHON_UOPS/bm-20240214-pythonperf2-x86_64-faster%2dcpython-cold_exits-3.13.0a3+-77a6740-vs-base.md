# Results vs. base

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 77a6740
- commit date: 2024-02-14
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 306 ms                                                                       | 319 ms: 1.04x slower                                                         |
| chameleon      | 7.58 ms                                                                      | 7.97 ms: 1.05x slower                                                        |
| docutils       | 2.93 sec                                                                     | 3.06 sec: 1.05x slower                                                       |
| Geometric mean | (ref)                                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|------------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none_tg     | 442 ms                                                                       | 445 ms: 1.01x slower                                                         |
| async_tree_io_tg       | 1.09 sec                                                                     | 1.10 sec: 1.01x slower                                                       |
| async_tree_io          | 1.09 sec                                                                     | 1.10 sec: 1.01x slower                                                       |
| async_tree_memoization | 555 ms                                                                       | 563 ms: 1.02x slower                                                         |
| async_tree_none        | 441 ms                                                                       | 450 ms: 1.02x slower                                                         |
| Geometric mean         | (ref)                                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 264 ms                                                                       | 266 ms: 1.01x slower                                                         |
| nbody          | 117 ms                                                                       | 123 ms: 1.05x slower                                                         |
| float          | 92.1 ms                                                                      | 102 ms: 1.11x slower                                                         |
| Geometric mean | (ref)                                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 237 ms                                                                       | 235 ms: 1.01x faster                                                         |
| regex_v8       | 26.2 ms                                                                      | 26.4 ms: 1.01x slower                                                        |
| regex_effbot   | 3.46 ms                                                                      | 3.58 ms: 1.04x slower                                                        |
| regex_compile  | 165 ms                                                                       | 192 ms: 1.17x slower                                                         |
| Geometric mean | (ref)                                                                        | 1.05x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_loads           | 25.4 us                                                                      | 25.1 us: 1.01x faster                                                        |
| unpickle             | 15.0 us                                                                      | 14.8 us: 1.01x faster                                                        |
| xml_etree_parse      | 148 ms                                                                       | 147 ms: 1.01x faster                                                         |
| json_dumps           | 10.8 ms                                                                      | 10.8 ms: 1.01x slower                                                        |
| pickle_pure_python   | 310 us                                                                       | 314 us: 1.01x slower                                                         |
| pickle_list          | 4.39 us                                                                      | 4.45 us: 1.01x slower                                                        |
| pickle_dict          | 33.0 us                                                                      | 33.6 us: 1.02x slower                                                        |
| unpickle_list        | 4.61 us                                                                      | 4.74 us: 1.03x slower                                                        |
| xml_etree_generate   | 87.9 ms                                                                      | 91.2 ms: 1.04x slower                                                        |
| xml_etree_process    | 60.0 ms                                                                      | 62.5 ms: 1.04x slower                                                        |
| xml_etree_iterparse  | 110 ms                                                                       | 116 ms: 1.05x slower                                                         |
| tomli_loads          | 2.66 sec                                                                     | 2.87 sec: 1.08x slower                                                       |
| unpickle_pure_python | 229 us                                                                       | 310 us: 1.36x slower                                                         |
| Geometric mean       | (ref)                                                                        | 1.04x slower                                                                 |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|------------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 12.6 ms                                                                      | 12.7 ms: 1.01x slower                                                        |
| python_startup_no_site | 11.1 ms                                                                      | 11.2 ms: 1.01x slower                                                        |
| Geometric mean         | (ref)                                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|-----------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 13.2 ms                                                                      | 14.1 ms: 1.07x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20240214-pythonperf2-x86_64-python-6755c4e0c8803a246e63-3.13.0a3+-6755c4e | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|--------------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| coverage                 | 85.3 ms                                                                      | 80.0 ms: 1.07x faster                                                        |
| json_loads               | 25.4 us                                                                      | 25.1 us: 1.01x faster                                                        |
| unpickle                 | 15.0 us                                                                      | 14.8 us: 1.01x faster                                                        |
| logging_simple           | 6.99 us                                                                      | 6.91 us: 1.01x faster                                                        |
| regex_dna                | 237 ms                                                                       | 235 ms: 1.01x faster                                                         |
| xml_etree_parse          | 148 ms                                                                       | 147 ms: 1.01x faster                                                         |
| logging_format           | 7.63 us                                                                      | 7.56 us: 1.01x faster                                                        |
| asyncio_websockets       | 389 ms                                                                       | 386 ms: 1.01x faster                                                         |
| coroutines               | 22.5 ms                                                                      | 22.3 ms: 1.01x faster                                                        |
| deepcopy                 | 385 us                                                                       | 387 us: 1.01x slower                                                         |
| json_dumps               | 10.8 ms                                                                      | 10.8 ms: 1.01x slower                                                        |
| asyncio_tcp_ssl          | 1.58 sec                                                                     | 1.59 sec: 1.01x slower                                                       |
| regex_v8                 | 26.2 ms                                                                      | 26.4 ms: 1.01x slower                                                        |
| pidigits                 | 264 ms                                                                       | 266 ms: 1.01x slower                                                         |
| async_tree_none_tg       | 442 ms                                                                       | 445 ms: 1.01x slower                                                         |
| async_tree_io_tg         | 1.09 sec                                                                     | 1.10 sec: 1.01x slower                                                       |
| python_startup           | 12.6 ms                                                                      | 12.7 ms: 1.01x slower                                                        |
| gc_traversal             | 3.53 ms                                                                      | 3.57 ms: 1.01x slower                                                        |
| deepcopy_reduce          | 3.45 us                                                                      | 3.48 us: 1.01x slower                                                        |
| asyncio_tcp              | 370 ms                                                                       | 374 ms: 1.01x slower                                                         |
| python_startup_no_site   | 11.1 ms                                                                      | 11.2 ms: 1.01x slower                                                        |
| async_generators         | 377 ms                                                                       | 381 ms: 1.01x slower                                                         |
| pickle_pure_python       | 310 us                                                                       | 314 us: 1.01x slower                                                         |
| async_tree_io            | 1.09 sec                                                                     | 1.10 sec: 1.01x slower                                                       |
| mdp                      | 2.61 sec                                                                     | 2.64 sec: 1.01x slower                                                       |
| pickle_list              | 4.39 us                                                                      | 4.45 us: 1.01x slower                                                        |
| telco                    | 8.26 ms                                                                      | 8.38 ms: 1.01x slower                                                        |
| async_tree_memoization   | 555 ms                                                                       | 563 ms: 1.02x slower                                                         |
| chaos                    | 74.3 ms                                                                      | 75.5 ms: 1.02x slower                                                        |
| pickle_dict              | 33.0 us                                                                      | 33.6 us: 1.02x slower                                                        |
| sqlite_synth             | 2.80 us                                                                      | 2.85 us: 1.02x slower                                                        |
| async_tree_none          | 441 ms                                                                       | 450 ms: 1.02x slower                                                         |
| logging_silent           | 97.4 ns                                                                      | 99.8 ns: 1.02x slower                                                        |
| typing_runtime_protocols | 121 us                                                                       | 124 us: 1.03x slower                                                         |
| unpickle_list            | 4.61 us                                                                      | 4.74 us: 1.03x slower                                                        |
| sqlglot_normalize        | 119 ms                                                                       | 123 ms: 1.03x slower                                                         |
| regex_effbot             | 3.46 ms                                                                      | 3.58 ms: 1.04x slower                                                        |
| xml_etree_generate       | 87.9 ms                                                                      | 91.2 ms: 1.04x slower                                                        |
| meteor_contest           | 134 ms                                                                       | 139 ms: 1.04x slower                                                         |
| 2to3                     | 306 ms                                                                       | 319 ms: 1.04x slower                                                         |
| xml_etree_process        | 60.0 ms                                                                      | 62.5 ms: 1.04x slower                                                        |
| sympy_integrate          | 24.2 ms                                                                      | 25.3 ms: 1.04x slower                                                        |
| xml_etree_iterparse      | 110 ms                                                                       | 116 ms: 1.05x slower                                                         |
| sympy_sum                | 165 ms                                                                       | 172 ms: 1.05x slower                                                         |
| sqlglot_transpile        | 1.87 ms                                                                      | 1.96 ms: 1.05x slower                                                        |
| docutils                 | 2.93 sec                                                                     | 3.06 sec: 1.05x slower                                                       |
| sympy_str                | 315 ms                                                                       | 330 ms: 1.05x slower                                                         |
| sympy_expand             | 532 ms                                                                       | 559 ms: 1.05x slower                                                         |
| chameleon                | 7.58 ms                                                                      | 7.97 ms: 1.05x slower                                                        |
| spectral_norm            | 141 ms                                                                       | 149 ms: 1.05x slower                                                         |
| nbody                    | 117 ms                                                                       | 123 ms: 1.05x slower                                                         |
| deltablue                | 3.83 ms                                                                      | 4.05 ms: 1.06x slower                                                        |
| dulwich_log              | 71.8 ms                                                                      | 76.0 ms: 1.06x slower                                                        |
| sqlglot_parse            | 1.45 ms                                                                      | 1.53 ms: 1.06x slower                                                        |
| sqlglot_optimize         | 62.0 ms                                                                      | 66.0 ms: 1.06x slower                                                        |
| crypto_pyaes             | 81.5 ms                                                                      | 86.8 ms: 1.07x slower                                                        |
| deepcopy_memo            | 39.0 us                                                                      | 41.7 us: 1.07x slower                                                        |
| scimark_fft              | 393 ms                                                                       | 420 ms: 1.07x slower                                                         |
| mako                     | 13.2 ms                                                                      | 14.1 ms: 1.07x slower                                                        |
| tomli_loads              | 2.66 sec                                                                     | 2.87 sec: 1.08x slower                                                       |
| pycparser                | 1.33 sec                                                                     | 1.43 sec: 1.08x slower                                                       |
| pprint_safe_repr         | 864 ms                                                                       | 952 ms: 1.10x slower                                                         |
| pprint_pformat           | 1.78 sec                                                                     | 1.96 sec: 1.10x slower                                                       |
| nqueens                  | 103 ms                                                                       | 114 ms: 1.11x slower                                                         |
| go                       | 178 ms                                                                       | 197 ms: 1.11x slower                                                         |
| float                    | 92.1 ms                                                                      | 102 ms: 1.11x slower                                                         |
| scimark_sor              | 146 ms                                                                       | 163 ms: 1.12x slower                                                         |
| comprehensions           | 22.0 us                                                                      | 24.5 us: 1.12x slower                                                        |
| raytrace                 | 299 ms                                                                       | 339 ms: 1.13x slower                                                         |
| fannkuch                 | 442 ms                                                                       | 512 ms: 1.16x slower                                                         |
| richards_super           | 58.9 ms                                                                      | 68.5 ms: 1.16x slower                                                        |
| regex_compile            | 165 ms                                                                       | 192 ms: 1.17x slower                                                         |
| richards                 | 52.5 ms                                                                      | 62.0 ms: 1.18x slower                                                        |
| pyflate                  | 562 ms                                                                       | 676 ms: 1.20x slower                                                         |
| hexiom                   | 8.71 ms                                                                      | 10.5 ms: 1.20x slower                                                        |
| scimark_monte_carlo      | 81.4 ms                                                                      | 104 ms: 1.28x slower                                                         |
| unpickle_pure_python     | 229 us                                                                       | 310 us: 1.36x slower                                                         |
| scimark_lu               | 101 ms                                                                       | 140 ms: 1.39x slower                                                         |
| unpack_sequence          | 47.2 ns                                                                      | 66.9 ns: 1.42x slower                                                        |
| Geometric mean           | (ref)                                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (14): create_gc_cycles, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, pickle, tornado_http, generators, bench_thread_pool, pathlib, json, bench_mp_pool, dask, async_tree_memoization_tg, scimark_sparse_mat_mult, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.01x