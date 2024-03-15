# Results vs. base

- fork: brandtbucher
- ref: justin_cold
- machine: windows-x86
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.01x slower
- HPT reliability: 99.86%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 253 ms                                                                          | 251 ms: 1.01x faster                                                         |
| chameleon      | 6.14 ms                                                                         | 5.97 ms: 1.03x faster                                                        |
| docutils       | 1.82 sec                                                                        | 1.81 sec: 1.01x faster                                                       |
| tornado_http   | 101 ms                                                                          | 97.1 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                                           | 1.02x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none_tg         | 249 ms                                                                          | 244 ms: 1.02x faster                                                         |
| async_tree_cpu_io_mixed    | 517 ms                                                                          | 524 ms: 1.01x slower                                                         |
| async_tree_io              | 626 ms                                                                          | 637 ms: 1.02x slower                                                         |
| async_tree_memoization     | 321 ms                                                                          | 328 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 505 ms                                                                          | 515 ms: 1.02x slower                                                         |
| Geometric mean             | (ref)                                                                           | 1.01x slower                                                                 |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_io_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 202 ms                                                                          | 204 ms: 1.01x slower                                                         |
| float          | 55.4 ms                                                                         | 56.2 ms: 1.01x slower                                                        |
| nbody          | 92.5 ms                                                                         | 97.0 ms: 1.05x slower                                                        |
| Geometric mean | (ref)                                                                           | 1.02x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 105 ms                                                                          | 106 ms: 1.01x slower                                                         |
| regex_dna      | 117 ms                                                                          | 121 ms: 1.03x slower                                                         |
| regex_effbot   | 1.88 ms                                                                         | 1.94 ms: 1.03x slower                                                        |
| regex_v8       | 15.9 ms                                                                         | 16.6 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                                           | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_list        | 3.30 us                                                                         | 3.04 us: 1.08x faster                                                        |
| json_loads           | 20.1 us                                                                         | 19.6 us: 1.02x faster                                                        |
| pickle_list          | 3.28 us                                                                         | 3.22 us: 1.02x faster                                                        |
| unpickle_pure_python | 153 us                                                                          | 151 us: 1.01x faster                                                         |
| pickle_dict          | 19.9 us                                                                         | 19.8 us: 1.00x faster                                                        |
| pickle_pure_python   | 208 us                                                                          | 210 us: 1.01x slower                                                         |
| tomli_loads          | 1.64 sec                                                                        | 1.67 sec: 1.02x slower                                                       |
| xml_etree_process    | 41.4 ms                                                                         | 42.2 ms: 1.02x slower                                                        |
| unpickle             | 10.1 us                                                                         | 10.3 us: 1.02x slower                                                        |
| xml_etree_generate   | 59.5 ms                                                                         | 61.3 ms: 1.03x slower                                                        |
| xml_etree_parse      | 108 ms                                                                          | 111 ms: 1.03x slower                                                         |
| xml_etree_iterparse  | 66.8 ms                                                                         | 69.9 ms: 1.05x slower                                                        |
| Geometric mean       | (ref)                                                                           | 1.00x slower                                                                 |

Benchmark hidden because not significant (2): json_dumps, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 20.2 ms                                                                         | 21.0 ms: 1.04x slower                                                        |
| python_startup         | 22.3 ms                                                                         | 23.1 ms: 1.04x slower                                                        |
| Geometric mean         | (ref)                                                                           | 1.04x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 7.89 ms                                                                         | 7.97 ms: 1.01x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20240201-pythonperf1_win32-x86-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_list              | 3.30 us                                                                         | 3.04 us: 1.08x faster                                                        |
| coverage                   | 502 ms                                                                          | 480 ms: 1.05x faster                                                         |
| richards                   | 30.3 ms                                                                         | 29.0 ms: 1.04x faster                                                        |
| tornado_http               | 101 ms                                                                          | 97.1 ms: 1.04x faster                                                        |
| pycparser                  | 862 ms                                                                          | 830 ms: 1.04x faster                                                         |
| fannkuch                   | 323 ms                                                                          | 313 ms: 1.03x faster                                                         |
| unpack_sequence            | 40.8 ns                                                                         | 39.7 ns: 1.03x faster                                                        |
| chameleon                  | 6.14 ms                                                                         | 5.97 ms: 1.03x faster                                                        |
| pathlib                    | 91.2 ms                                                                         | 88.8 ms: 1.03x faster                                                        |
| json                       | 4.16 ms                                                                         | 4.07 ms: 1.02x faster                                                        |
| richards_super             | 33.9 ms                                                                         | 33.1 ms: 1.02x faster                                                        |
| json_loads                 | 20.1 us                                                                         | 19.6 us: 1.02x faster                                                        |
| async_tree_none_tg         | 249 ms                                                                          | 244 ms: 1.02x faster                                                         |
| deepcopy_memo              | 23.6 us                                                                         | 23.2 us: 1.02x faster                                                        |
| pickle_list                | 3.28 us                                                                         | 3.22 us: 1.02x faster                                                        |
| scimark_lu                 | 61.5 ms                                                                         | 60.6 ms: 1.02x faster                                                        |
| unpickle_pure_python       | 153 us                                                                          | 151 us: 1.01x faster                                                         |
| raytrace                   | 230 ms                                                                          | 227 ms: 1.01x faster                                                         |
| coroutines                 | 14.7 ms                                                                         | 14.5 ms: 1.01x faster                                                        |
| pprint_pformat             | 1.45 sec                                                                        | 1.43 sec: 1.01x faster                                                       |
| deepcopy_reduce            | 2.47 us                                                                         | 2.45 us: 1.01x faster                                                        |
| 2to3                       | 253 ms                                                                          | 251 ms: 1.01x faster                                                         |
| go                         | 120 ms                                                                          | 119 ms: 1.01x faster                                                         |
| docutils                   | 1.82 sec                                                                        | 1.81 sec: 1.01x faster                                                       |
| pprint_safe_repr           | 692 ms                                                                          | 688 ms: 1.01x faster                                                         |
| pickle_dict                | 19.9 us                                                                         | 19.8 us: 1.00x faster                                                        |
| regex_compile              | 105 ms                                                                          | 106 ms: 1.01x slower                                                         |
| sympy_expand               | 366 ms                                                                          | 369 ms: 1.01x slower                                                         |
| pidigits                   | 202 ms                                                                          | 204 ms: 1.01x slower                                                         |
| pickle_pure_python         | 208 us                                                                          | 210 us: 1.01x slower                                                         |
| dask                       | 307 ms                                                                          | 310 ms: 1.01x slower                                                         |
| mako                       | 7.89 ms                                                                         | 7.97 ms: 1.01x slower                                                        |
| crypto_pyaes               | 62.5 ms                                                                         | 63.3 ms: 1.01x slower                                                        |
| sqlglot_normalize          | 218 ms                                                                          | 221 ms: 1.01x slower                                                         |
| nqueens                    | 86.0 ms                                                                         | 87.1 ms: 1.01x slower                                                        |
| scimark_monte_carlo        | 68.5 ms                                                                         | 69.4 ms: 1.01x slower                                                        |
| sqlglot_optimize           | 41.9 ms                                                                         | 42.5 ms: 1.01x slower                                                        |
| logging_format             | 8.60 us                                                                         | 8.71 us: 1.01x slower                                                        |
| async_tree_cpu_io_mixed    | 517 ms                                                                          | 524 ms: 1.01x slower                                                         |
| float                      | 55.4 ms                                                                         | 56.2 ms: 1.01x slower                                                        |
| telco                      | 6.02 ms                                                                         | 6.11 ms: 1.01x slower                                                        |
| tomli_loads                | 1.64 sec                                                                        | 1.67 sec: 1.02x slower                                                       |
| sympy_integrate            | 15.8 ms                                                                         | 16.1 ms: 1.02x slower                                                        |
| bench_mp_pool              | 74.4 ms                                                                         | 75.7 ms: 1.02x slower                                                        |
| gc_traversal               | 1.39 ms                                                                         | 1.42 ms: 1.02x slower                                                        |
| async_tree_io              | 626 ms                                                                          | 637 ms: 1.02x slower                                                         |
| xml_etree_process          | 41.4 ms                                                                         | 42.2 ms: 1.02x slower                                                        |
| logging_silent             | 60.4 ns                                                                         | 61.6 ns: 1.02x slower                                                        |
| async_tree_memoization     | 321 ms                                                                          | 328 ms: 1.02x slower                                                         |
| sympy_sum                  | 110 ms                                                                          | 112 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 505 ms                                                                          | 515 ms: 1.02x slower                                                         |
| spectral_norm              | 76.6 ms                                                                         | 78.2 ms: 1.02x slower                                                        |
| unpickle                   | 10.1 us                                                                         | 10.3 us: 1.02x slower                                                        |
| async_generators           | 287 ms                                                                          | 294 ms: 1.02x slower                                                         |
| sqlglot_transpile          | 1.15 ms                                                                         | 1.18 ms: 1.02x slower                                                        |
| sqlite_synth               | 1.82 us                                                                         | 1.87 us: 1.03x slower                                                        |
| meteor_contest             | 85.3 ms                                                                         | 87.5 ms: 1.03x slower                                                        |
| typing_runtime_protocols   | 95.4 us                                                                         | 97.9 us: 1.03x slower                                                        |
| scimark_fft                | 247 ms                                                                          | 254 ms: 1.03x slower                                                         |
| sqlglot_parse              | 894 us                                                                          | 918 us: 1.03x slower                                                         |
| pyflate                    | 372 ms                                                                          | 383 ms: 1.03x slower                                                         |
| regex_dna                  | 117 ms                                                                          | 121 ms: 1.03x slower                                                         |
| sympy_str                  | 213 ms                                                                          | 219 ms: 1.03x slower                                                         |
| logging_simple             | 7.96 us                                                                         | 8.19 us: 1.03x slower                                                        |
| hexiom                     | 6.52 ms                                                                         | 6.72 ms: 1.03x slower                                                        |
| xml_etree_generate         | 59.5 ms                                                                         | 61.3 ms: 1.03x slower                                                        |
| xml_etree_parse            | 108 ms                                                                          | 111 ms: 1.03x slower                                                         |
| regex_effbot               | 1.88 ms                                                                         | 1.94 ms: 1.03x slower                                                        |
| scimark_sor                | 80.7 ms                                                                         | 83.4 ms: 1.03x slower                                                        |
| scimark_sparse_mat_mult    | 3.15 ms                                                                         | 3.26 ms: 1.03x slower                                                        |
| python_startup_no_site     | 20.2 ms                                                                         | 21.0 ms: 1.04x slower                                                        |
| python_startup             | 22.3 ms                                                                         | 23.1 ms: 1.04x slower                                                        |
| bench_thread_pool          | 1.04 ms                                                                         | 1.09 ms: 1.04x slower                                                        |
| regex_v8                   | 15.9 ms                                                                         | 16.6 ms: 1.04x slower                                                        |
| xml_etree_iterparse        | 66.8 ms                                                                         | 69.9 ms: 1.05x slower                                                        |
| nbody                      | 92.5 ms                                                                         | 97.0 ms: 1.05x slower                                                        |
| asyncio_tcp                | 626 ms                                                                          | 665 ms: 1.06x slower                                                         |
| mdp                        | 1.82 sec                                                                        | 1.93 sec: 1.06x slower                                                       |
| comprehensions             | 14.6 us                                                                         | 15.7 us: 1.08x slower                                                        |
| Geometric mean             | (ref)                                                                           | 1.01x slower                                                                 |

Benchmark hidden because not significant (11): deepcopy, async_tree_memoization_tg, generators, async_tree_io_tg, deltablue, create_gc_cycles, json_dumps, asyncio_tcp_ssl, chaos, async_tree_none, pickle


# HPT report

- Reliability score: 99.86% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown