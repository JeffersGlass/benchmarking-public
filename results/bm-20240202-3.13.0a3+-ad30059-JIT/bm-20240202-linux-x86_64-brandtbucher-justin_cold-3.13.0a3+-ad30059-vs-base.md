# Results vs. base

- fork: brandtbucher
- ref: justin_cold
- machine: linux-x86_64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.01x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 274 ms                                                                 | 277 ms: 1.01x slower                                                |
| docutils       | 2.64 sec                                                               | 2.66 sec: 1.01x slower                                              |
| tornado_http   | 96.9 ms                                                                | 97.6 ms: 1.01x slower                                               |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|---------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_io             | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                              |
| async_tree_io_tg          | 1.20 sec                                                               | 1.20 sec: 1.00x slower                                              |
| async_tree_none_tg        | 449 ms                                                                 | 454 ms: 1.01x slower                                                |
| async_tree_memoization    | 560 ms                                                                 | 566 ms: 1.01x slower                                                |
| async_tree_memoization_tg | 579 ms                                                                 | 593 ms: 1.02x slower                                                |
| Geometric mean            | (ref)                                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x slower                                                |
| float          | 86.1 ms                                                                | 86.5 ms: 1.00x slower                                               |
| nbody          | 102 ms                                                                 | 106 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_v8       | 24.7 ms                                                                | 24.9 ms: 1.01x slower                                               |
| regex_dna      | 219 ms                                                                 | 222 ms: 1.01x slower                                                |
| regex_compile  | 140 ms                                                                 | 144 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|---------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_list         | 5.23 us                                                                | 5.20 us: 1.01x faster                                               |
| json_dumps          | 10.3 ms                                                                | 10.4 ms: 1.01x slower                                               |
| xml_etree_iterparse | 108 ms                                                                 | 109 ms: 1.01x slower                                                |
| pickle_dict         | 34.7 us                                                                | 35.1 us: 1.01x slower                                               |
| xml_etree_parse     | 156 ms                                                                 | 157 ms: 1.01x slower                                                |
| unpickle_list       | 4.97 us                                                                | 5.04 us: 1.01x slower                                               |
| unpickle            | 14.8 us                                                                | 15.3 us: 1.03x slower                                               |
| pickle              | 11.4 us                                                                | 11.9 us: 1.04x slower                                               |
| Geometric mean      | (ref)                                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (6): xml_etree_generate, unpickle_pure_python, json_loads, pickle_pure_python, xml_etree_process, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                               |
| python_startup_no_site | 8.76 ms                                                                | 8.83 ms: 1.01x slower                                               |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 12.4 ms                                                                | 12.7 ms: 1.02x slower                                               |

All benchmarks:
===============

| Benchmark                 | bm-20240201-linux-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|---------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| mdp                       | 2.80 sec                                                               | 2.64 sec: 1.06x faster                                              |
| coroutines                | 22.9 ms                                                                | 22.3 ms: 1.03x faster                                               |
| logging_silent            | 102 ns                                                                 | 99.3 ns: 1.03x faster                                               |
| deepcopy_memo             | 38.3 us                                                                | 37.4 us: 1.02x faster                                               |
| fannkuch                  | 436 ms                                                                 | 428 ms: 1.02x faster                                                |
| scimark_sor               | 122 ms                                                                 | 120 ms: 1.02x faster                                                |
| logging_format            | 6.46 us                                                                | 6.36 us: 1.02x faster                                               |
| gc_traversal              | 3.87 ms                                                                | 3.81 ms: 1.02x faster                                               |
| logging_simple            | 5.83 us                                                                | 5.77 us: 1.01x faster                                               |
| coverage                  | 94.7 ms                                                                | 93.8 ms: 1.01x faster                                               |
| sqlite_synth              | 2.83 us                                                                | 2.81 us: 1.01x faster                                               |
| async_tree_io             | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                              |
| pickle_list               | 5.23 us                                                                | 5.20 us: 1.01x faster                                               |
| async_tree_io_tg          | 1.20 sec                                                               | 1.20 sec: 1.00x slower                                              |
| pidigits                  | 188 ms                                                                 | 188 ms: 1.00x slower                                                |
| asyncio_tcp_ssl           | 1.80 sec                                                               | 1.81 sec: 1.00x slower                                              |
| float                     | 86.1 ms                                                                | 86.5 ms: 1.00x slower                                               |
| dulwich_log               | 67.6 ms                                                                | 68.0 ms: 1.01x slower                                               |
| python_startup            | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                               |
| sqlglot_optimize          | 55.5 ms                                                                | 55.9 ms: 1.01x slower                                               |
| python_startup_no_site    | 8.76 ms                                                                | 8.83 ms: 1.01x slower                                               |
| tornado_http              | 96.9 ms                                                                | 97.6 ms: 1.01x slower                                               |
| sqlglot_transpile         | 1.61 ms                                                                | 1.62 ms: 1.01x slower                                               |
| sqlglot_parse             | 1.28 ms                                                                | 1.29 ms: 1.01x slower                                               |
| json_dumps                | 10.3 ms                                                                | 10.4 ms: 1.01x slower                                               |
| xml_etree_iterparse       | 108 ms                                                                 | 109 ms: 1.01x slower                                                |
| sympy_str                 | 285 ms                                                                 | 288 ms: 1.01x slower                                                |
| regex_v8                  | 24.7 ms                                                                | 24.9 ms: 1.01x slower                                               |
| 2to3                      | 274 ms                                                                 | 277 ms: 1.01x slower                                                |
| docutils                  | 2.64 sec                                                               | 2.66 sec: 1.01x slower                                              |
| bench_thread_pool         | 836 us                                                                 | 845 us: 1.01x slower                                                |
| async_tree_none_tg        | 449 ms                                                                 | 454 ms: 1.01x slower                                                |
| pickle_dict               | 34.7 us                                                                | 35.1 us: 1.01x slower                                               |
| async_tree_memoization    | 560 ms                                                                 | 566 ms: 1.01x slower                                                |
| sympy_integrate           | 20.9 ms                                                                | 21.1 ms: 1.01x slower                                               |
| xml_etree_parse           | 156 ms                                                                 | 157 ms: 1.01x slower                                                |
| scimark_lu                | 114 ms                                                                 | 116 ms: 1.01x slower                                                |
| typing_runtime_protocols  | 110 us                                                                 | 111 us: 1.01x slower                                                |
| regex_dna                 | 219 ms                                                                 | 222 ms: 1.01x slower                                                |
| scimark_sparse_mat_mult   | 5.55 ms                                                                | 5.62 ms: 1.01x slower                                               |
| asyncio_tcp               | 489 ms                                                                 | 496 ms: 1.01x slower                                                |
| sqlglot_normalize         | 108 ms                                                                 | 110 ms: 1.01x slower                                                |
| unpickle_list             | 4.97 us                                                                | 5.04 us: 1.01x slower                                               |
| meteor_contest            | 110 ms                                                                 | 111 ms: 1.01x slower                                                |
| generators                | 29.5 ms                                                                | 30.0 ms: 1.02x slower                                               |
| scimark_monte_carlo       | 75.6 ms                                                                | 76.9 ms: 1.02x slower                                               |
| pprint_pformat            | 1.68 sec                                                               | 1.71 sec: 1.02x slower                                              |
| sympy_expand              | 474 ms                                                                 | 482 ms: 1.02x slower                                                |
| sympy_sum                 | 159 ms                                                                 | 162 ms: 1.02x slower                                                |
| mako                      | 12.4 ms                                                                | 12.7 ms: 1.02x slower                                               |
| scimark_fft               | 375 ms                                                                 | 383 ms: 1.02x slower                                                |
| telco                     | 8.31 ms                                                                | 8.49 ms: 1.02x slower                                               |
| regex_compile             | 140 ms                                                                 | 144 ms: 1.02x slower                                                |
| async_tree_memoization_tg | 579 ms                                                                 | 593 ms: 1.02x slower                                                |
| async_generators          | 462 ms                                                                 | 473 ms: 1.02x slower                                                |
| nqueens                   | 89.7 ms                                                                | 92.0 ms: 1.03x slower                                               |
| go                        | 150 ms                                                                 | 154 ms: 1.03x slower                                                |
| unpickle                  | 14.8 us                                                                | 15.3 us: 1.03x slower                                               |
| nbody                     | 102 ms                                                                 | 106 ms: 1.03x slower                                                |
| hexiom                    | 8.00 ms                                                                | 8.28 ms: 1.04x slower                                               |
| crypto_pyaes              | 77.7 ms                                                                | 80.5 ms: 1.04x slower                                               |
| pickle                    | 11.4 us                                                                | 11.9 us: 1.04x slower                                               |
| Geometric mean            | (ref)                                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (31): deepcopy, richards_super, raytrace, xml_etree_generate, json, unpickle_pure_python, chaos, pyflate, pathlib, json_loads, pickle_pure_python, create_gc_cycles, unpack_sequence, richards, deltablue, bench_mp_pool, xml_etree_process, deepcopy_reduce, asyncio_websockets, regex_effbot, pycparser, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, tomli_loads, chameleon, comprehensions, spectral_norm, dask, async_tree_none, pprint_safe_repr, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x