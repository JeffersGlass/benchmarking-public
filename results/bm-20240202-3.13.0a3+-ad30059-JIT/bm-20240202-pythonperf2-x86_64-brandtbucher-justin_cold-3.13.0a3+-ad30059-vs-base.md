# Results vs. base

- fork: brandtbucher
- ref: justin_cold
- machine: linux-x86_64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.01x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 300 ms                                                                       | 302 ms: 1.01x slower                                                      |
| chameleon      | 7.71 ms                                                                      | 7.93 ms: 1.03x slower                                                     |
| tornado_http   | 128 ms                                                                       | 125 ms: 1.02x faster                                                      |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                              |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none_tg | 439 ms                                                                       | 443 ms: 1.01x slower                                                      |
| Geometric mean     | (ref)                                                                        | 1.00x slower                                                              |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none, async_tree_io_tg, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 264 ms                                                                       | 263 ms: 1.00x faster                                                      |
| float          | 82.3 ms                                                                      | 83.1 ms: 1.01x slower                                                     |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                              |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_effbot   | 3.55 ms                                                                      | 3.50 ms: 1.02x faster                                                     |
| regex_compile  | 147 ms                                                                       | 148 ms: 1.01x slower                                                      |
| regex_v8       | 25.7 ms                                                                      | 26.1 ms: 1.02x slower                                                     |
| regex_dna      | 238 ms                                                                       | 251 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                                        | 1.02x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_list        | 4.86 us                                                                      | 4.77 us: 1.02x faster                                                     |
| pickle_pure_python   | 311 us                                                                       | 308 us: 1.01x faster                                                      |
| json_dumps           | 10.7 ms                                                                      | 10.6 ms: 1.01x faster                                                     |
| xml_etree_generate   | 86.8 ms                                                                      | 87.1 ms: 1.00x slower                                                     |
| xml_etree_process    | 59.3 ms                                                                      | 59.5 ms: 1.00x slower                                                     |
| xml_etree_parse      | 145 ms                                                                       | 147 ms: 1.01x slower                                                      |
| tomli_loads          | 2.34 sec                                                                     | 2.38 sec: 1.01x slower                                                    |
| unpickle_pure_python | 228 us                                                                       | 232 us: 1.02x slower                                                      |
| xml_etree_iterparse  | 106 ms                                                                       | 108 ms: 1.02x slower                                                      |
| unpickle             | 14.9 us                                                                      | 15.5 us: 1.04x slower                                                     |
| Geometric mean       | (ref)                                                                        | 1.01x slower                                                              |

Benchmark hidden because not significant (4): pickle, json_loads, pickle_dict, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 12.7 ms                                                                      | 12.7 ms: 1.01x faster                                                     |
| python_startup_no_site | 11.2 ms                                                                      | 11.1 ms: 1.00x faster                                                     |
| Geometric mean         | (ref)                                                                        | 1.01x faster                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 11.8 ms                                                                      | 11.9 ms: 1.01x slower                                                     |

All benchmarks:
===============

| Benchmark                | bm-20240201-pythonperf2-x86_64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf2-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------------|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpack_sequence          | 47.1 ns                                                                      | 43.7 ns: 1.08x faster                                                     |
| dulwich_log              | 71.3 ms                                                                      | 68.9 ms: 1.03x faster                                                     |
| scimark_sor              | 146 ms                                                                       | 142 ms: 1.03x faster                                                      |
| meteor_contest           | 133 ms                                                                       | 130 ms: 1.02x faster                                                      |
| unpickle_list            | 4.86 us                                                                      | 4.77 us: 1.02x faster                                                     |
| tornado_http             | 128 ms                                                                       | 125 ms: 1.02x faster                                                      |
| regex_effbot             | 3.55 ms                                                                      | 3.50 ms: 1.02x faster                                                     |
| json                     | 5.34 ms                                                                      | 5.26 ms: 1.02x faster                                                     |
| scimark_lu               | 101 ms                                                                       | 99.4 ms: 1.01x faster                                                     |
| richards                 | 51.3 ms                                                                      | 50.7 ms: 1.01x faster                                                     |
| pickle_pure_python       | 311 us                                                                       | 308 us: 1.01x faster                                                      |
| python_startup           | 12.7 ms                                                                      | 12.7 ms: 1.01x faster                                                     |
| json_dumps               | 10.7 ms                                                                      | 10.6 ms: 1.01x faster                                                     |
| sympy_sum                | 162 ms                                                                       | 161 ms: 1.01x faster                                                      |
| telco                    | 8.26 ms                                                                      | 8.22 ms: 1.01x faster                                                     |
| python_startup_no_site   | 11.2 ms                                                                      | 11.1 ms: 1.00x faster                                                     |
| sqlglot_optimize         | 62.0 ms                                                                      | 61.8 ms: 1.00x faster                                                     |
| pidigits                 | 264 ms                                                                       | 263 ms: 1.00x faster                                                      |
| asyncio_tcp_ssl          | 1.58 sec                                                                     | 1.58 sec: 1.00x slower                                                    |
| generators               | 34.4 ms                                                                      | 34.5 ms: 1.00x slower                                                     |
| xml_etree_generate       | 86.8 ms                                                                      | 87.1 ms: 1.00x slower                                                     |
| sqlglot_normalize        | 121 ms                                                                       | 121 ms: 1.00x slower                                                      |
| xml_etree_process        | 59.3 ms                                                                      | 59.5 ms: 1.00x slower                                                     |
| sympy_expand             | 507 ms                                                                       | 509 ms: 1.00x slower                                                      |
| crypto_pyaes             | 81.1 ms                                                                      | 81.5 ms: 1.01x slower                                                     |
| sqlite_synth             | 2.72 us                                                                      | 2.74 us: 1.01x slower                                                     |
| pathlib                  | 18.9 ms                                                                      | 19.1 ms: 1.01x slower                                                     |
| 2to3                     | 300 ms                                                                       | 302 ms: 1.01x slower                                                      |
| regex_compile            | 147 ms                                                                       | 148 ms: 1.01x slower                                                      |
| async_tree_none_tg       | 439 ms                                                                       | 443 ms: 1.01x slower                                                      |
| deepcopy                 | 382 us                                                                       | 386 us: 1.01x slower                                                      |
| float                    | 82.3 ms                                                                      | 83.1 ms: 1.01x slower                                                     |
| scimark_fft              | 365 ms                                                                       | 369 ms: 1.01x slower                                                      |
| deltablue                | 4.00 ms                                                                      | 4.05 ms: 1.01x slower                                                     |
| mako                     | 11.8 ms                                                                      | 11.9 ms: 1.01x slower                                                     |
| xml_etree_parse          | 145 ms                                                                       | 147 ms: 1.01x slower                                                      |
| mdp                      | 2.53 sec                                                                     | 2.57 sec: 1.01x slower                                                    |
| asyncio_websockets       | 387 ms                                                                       | 392 ms: 1.01x slower                                                      |
| pycparser                | 1.27 sec                                                                     | 1.29 sec: 1.01x slower                                                    |
| tomli_loads              | 2.34 sec                                                                     | 2.38 sec: 1.01x slower                                                    |
| deepcopy_memo            | 38.1 us                                                                      | 38.7 us: 1.01x slower                                                     |
| regex_v8                 | 25.7 ms                                                                      | 26.1 ms: 1.02x slower                                                     |
| unpickle_pure_python     | 228 us                                                                       | 232 us: 1.02x slower                                                      |
| xml_etree_iterparse      | 106 ms                                                                       | 108 ms: 1.02x slower                                                      |
| richards_super           | 57.1 ms                                                                      | 58.2 ms: 1.02x slower                                                     |
| scimark_sparse_mat_mult  | 5.13 ms                                                                      | 5.22 ms: 1.02x slower                                                     |
| pprint_safe_repr         | 861 ms                                                                       | 878 ms: 1.02x slower                                                      |
| async_generators         | 371 ms                                                                       | 379 ms: 1.02x slower                                                      |
| typing_runtime_protocols | 121 us                                                                       | 124 us: 1.02x slower                                                      |
| fannkuch                 | 422 ms                                                                       | 431 ms: 1.02x slower                                                      |
| comprehensions           | 20.4 us                                                                      | 20.9 us: 1.02x slower                                                     |
| logging_format           | 7.35 us                                                                      | 7.55 us: 1.03x slower                                                     |
| chameleon                | 7.71 ms                                                                      | 7.93 ms: 1.03x slower                                                     |
| go                       | 168 ms                                                                       | 173 ms: 1.03x slower                                                      |
| spectral_norm            | 118 ms                                                                       | 122 ms: 1.03x slower                                                      |
| hexiom                   | 7.80 ms                                                                      | 8.10 ms: 1.04x slower                                                     |
| nqueens                  | 98.0 ms                                                                      | 102 ms: 1.04x slower                                                      |
| unpickle                 | 14.9 us                                                                      | 15.5 us: 1.04x slower                                                     |
| logging_simple           | 6.62 us                                                                      | 6.92 us: 1.04x slower                                                     |
| coverage                 | 80.2 ms                                                                      | 84.1 ms: 1.05x slower                                                     |
| regex_dna                | 238 ms                                                                       | 251 ms: 1.05x slower                                                      |
| gc_traversal             | 3.87 ms                                                                      | 4.09 ms: 1.06x slower                                                     |
| Geometric mean           | (ref)                                                                        | 1.01x slower                                                              |

Benchmark hidden because not significant (31): mypy2, dask, async_tree_cpu_io_mixed, pickle, async_tree_io, json_loads, pprint_pformat, bench_thread_pool, logging_silent, sympy_integrate, pickle_dict, create_gc_cycles, async_tree_memoization, asyncio_tcp, sqlglot_transpile, docutils, nbody, sympy_str, async_tree_none, async_tree_io_tg, sqlglot_parse, chaos, pyflate, scimark_monte_carlo, pickle_list, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, deepcopy_reduce, bench_mp_pool, coroutines, raytrace


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x