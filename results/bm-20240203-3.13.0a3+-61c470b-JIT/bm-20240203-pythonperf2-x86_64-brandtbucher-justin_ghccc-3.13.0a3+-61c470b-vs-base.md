# Results vs. base

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.01x faster
- HPT reliability: 97.67%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 300 ms                                                                       | 298 ms: 1.00x faster                                                       |
| chameleon      | 7.79 ms                                                                      | 7.60 ms: 1.02x faster                                                      |
| docutils       | 2.88 sec                                                                     | 2.90 sec: 1.01x slower                                                     |
| Geometric mean | (ref)                                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none_tg | 439 ms                                                                       | 436 ms: 1.01x faster                                                       |
| async_tree_io_tg   | 1.07 sec                                                                     | 1.07 sec: 1.00x slower                                                     |
| async_tree_io      | 1.07 sec                                                                     | 1.08 sec: 1.01x slower                                                     |
| Geometric mean     | (ref)                                                                        | 1.00x slower                                                               |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 107 ms                                                                       | 94.1 ms: 1.14x faster                                                      |
| float          | 81.7 ms                                                                      | 80.5 ms: 1.01x faster                                                      |
| pidigits       | 262 ms                                                                       | 262 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                                        | 1.05x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 147 ms                                                                       | 146 ms: 1.01x faster                                                       |
| regex_dna      | 242 ms                                                                       | 248 ms: 1.02x slower                                                       |
| regex_v8       | 25.4 ms                                                                      | 26.1 ms: 1.03x slower                                                      |
| regex_effbot   | 3.46 ms                                                                      | 3.61 ms: 1.04x slower                                                      |
| Geometric mean | (ref)                                                                        | 1.02x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                                      | 30.9 us: 1.05x faster                                                      |
| pickle               | 10.7 us                                                                      | 10.3 us: 1.04x faster                                                      |
| unpickle             | 15.6 us                                                                      | 15.1 us: 1.04x faster                                                      |
| json_loads           | 25.7 us                                                                      | 25.0 us: 1.03x faster                                                      |
| xml_etree_generate   | 86.5 ms                                                                      | 85.9 ms: 1.01x faster                                                      |
| json_dumps           | 10.7 ms                                                                      | 10.6 ms: 1.01x faster                                                      |
| pickle_list          | 4.48 us                                                                      | 4.46 us: 1.01x faster                                                      |
| xml_etree_process    | 59.4 ms                                                                      | 59.1 ms: 1.01x faster                                                      |
| unpickle_pure_python | 231 us                                                                       | 230 us: 1.00x faster                                                       |
| unpickle_list        | 4.87 us                                                                      | 4.93 us: 1.01x slower                                                      |
| xml_etree_parse      | 145 ms                                                                       | 148 ms: 1.02x slower                                                       |
| Geometric mean       | (ref)                                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (3): tomli_loads, xml_etree_iterparse, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 12.6 ms                                                                      | 12.7 ms: 1.00x slower                                                      |
| python_startup_no_site | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                      |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                                      | 11.6 ms: 1.02x faster                                                      |

All benchmarks:
===============

| Benchmark                | bm-20240130-pythonperf2-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody                    | 107 ms                                                                       | 94.1 ms: 1.14x faster                                                      |
| crypto_pyaes             | 80.7 ms                                                                      | 75.0 ms: 1.08x faster                                                      |
| scimark_fft              | 367 ms                                                                       | 346 ms: 1.06x faster                                                       |
| chaos                    | 70.8 ms                                                                      | 66.8 ms: 1.06x faster                                                      |
| coverage                 | 83.8 ms                                                                      | 79.3 ms: 1.06x faster                                                      |
| pickle_dict              | 32.5 us                                                                      | 30.9 us: 1.05x faster                                                      |
| spectral_norm            | 118 ms                                                                       | 112 ms: 1.05x faster                                                       |
| pickle                   | 10.7 us                                                                      | 10.3 us: 1.04x faster                                                      |
| scimark_monte_carlo      | 79.2 ms                                                                      | 75.8 ms: 1.04x faster                                                      |
| unpickle                 | 15.6 us                                                                      | 15.1 us: 1.04x faster                                                      |
| json_loads               | 25.7 us                                                                      | 25.0 us: 1.03x faster                                                      |
| pycparser                | 1.32 sec                                                                     | 1.29 sec: 1.03x faster                                                     |
| raytrace                 | 277 ms                                                                       | 270 ms: 1.03x faster                                                       |
| chameleon                | 7.79 ms                                                                      | 7.60 ms: 1.02x faster                                                      |
| mako                     | 11.9 ms                                                                      | 11.6 ms: 1.02x faster                                                      |
| hexiom                   | 7.77 ms                                                                      | 7.60 ms: 1.02x faster                                                      |
| deepcopy_reduce          | 3.37 us                                                                      | 3.29 us: 1.02x faster                                                      |
| logging_format           | 7.43 us                                                                      | 7.27 us: 1.02x faster                                                      |
| deltablue                | 3.99 ms                                                                      | 3.91 ms: 1.02x faster                                                      |
| json                     | 5.28 ms                                                                      | 5.18 ms: 1.02x faster                                                      |
| scimark_sparse_mat_mult  | 5.12 ms                                                                      | 5.03 ms: 1.02x faster                                                      |
| logging_simple           | 6.69 us                                                                      | 6.57 us: 1.02x faster                                                      |
| pyflate                  | 514 ms                                                                       | 506 ms: 1.02x faster                                                       |
| fannkuch                 | 415 ms                                                                       | 409 ms: 1.02x faster                                                       |
| float                    | 81.7 ms                                                                      | 80.5 ms: 1.01x faster                                                      |
| meteor_contest           | 133 ms                                                                       | 131 ms: 1.01x faster                                                       |
| sympy_str                | 301 ms                                                                       | 297 ms: 1.01x faster                                                       |
| async_generators         | 371 ms                                                                       | 366 ms: 1.01x faster                                                       |
| nqueens                  | 97.1 ms                                                                      | 95.8 ms: 1.01x faster                                                      |
| create_gc_cycles         | 1.54 ms                                                                      | 1.52 ms: 1.01x faster                                                      |
| scimark_sor              | 142 ms                                                                       | 140 ms: 1.01x faster                                                       |
| richards_super           | 57.0 ms                                                                      | 56.4 ms: 1.01x faster                                                      |
| deepcopy                 | 374 us                                                                       | 371 us: 1.01x faster                                                       |
| sqlglot_parse            | 1.40 ms                                                                      | 1.39 ms: 1.01x faster                                                      |
| dulwich_log              | 68.5 ms                                                                      | 67.9 ms: 1.01x faster                                                      |
| sqlglot_transpile        | 1.82 ms                                                                      | 1.81 ms: 1.01x faster                                                      |
| regex_compile            | 147 ms                                                                       | 146 ms: 1.01x faster                                                       |
| async_tree_none_tg       | 439 ms                                                                       | 436 ms: 1.01x faster                                                       |
| xml_etree_generate       | 86.5 ms                                                                      | 85.9 ms: 1.01x faster                                                      |
| comprehensions           | 20.5 us                                                                      | 20.3 us: 1.01x faster                                                      |
| sympy_expand             | 504 ms                                                                       | 501 ms: 1.01x faster                                                       |
| json_dumps               | 10.7 ms                                                                      | 10.6 ms: 1.01x faster                                                      |
| pickle_list              | 4.48 us                                                                      | 4.46 us: 1.01x faster                                                      |
| xml_etree_process        | 59.4 ms                                                                      | 59.1 ms: 1.01x faster                                                      |
| sympy_integrate          | 24.2 ms                                                                      | 24.1 ms: 1.00x faster                                                      |
| 2to3                     | 300 ms                                                                       | 298 ms: 1.00x faster                                                       |
| asyncio_tcp              | 372 ms                                                                       | 370 ms: 1.00x faster                                                       |
| richards                 | 50.8 ms                                                                      | 50.6 ms: 1.00x faster                                                      |
| sympy_sum                | 159 ms                                                                       | 158 ms: 1.00x faster                                                       |
| unpickle_pure_python     | 231 us                                                                       | 230 us: 1.00x faster                                                       |
| generators               | 34.5 ms                                                                      | 34.4 ms: 1.00x faster                                                      |
| asyncio_tcp_ssl          | 1.58 sec                                                                     | 1.57 sec: 1.00x faster                                                     |
| pidigits                 | 262 ms                                                                       | 262 ms: 1.00x faster                                                       |
| python_startup           | 12.6 ms                                                                      | 12.7 ms: 1.00x slower                                                      |
| async_tree_io_tg         | 1.07 sec                                                                     | 1.07 sec: 1.00x slower                                                     |
| python_startup_no_site   | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                      |
| scimark_lu               | 101 ms                                                                       | 102 ms: 1.01x slower                                                       |
| logging_silent           | 95.1 ns                                                                      | 95.8 ns: 1.01x slower                                                      |
| async_tree_io            | 1.07 sec                                                                     | 1.08 sec: 1.01x slower                                                     |
| docutils                 | 2.88 sec                                                                     | 2.90 sec: 1.01x slower                                                     |
| mdp                      | 2.53 sec                                                                     | 2.55 sec: 1.01x slower                                                     |
| sqlglot_normalize        | 119 ms                                                                       | 120 ms: 1.01x slower                                                       |
| unpickle_list            | 4.87 us                                                                      | 4.93 us: 1.01x slower                                                      |
| coroutines               | 22.4 ms                                                                      | 22.7 ms: 1.01x slower                                                      |
| deepcopy_memo            | 37.4 us                                                                      | 37.9 us: 1.02x slower                                                      |
| pprint_pformat           | 1.76 sec                                                                     | 1.79 sec: 1.02x slower                                                     |
| regex_dna                | 242 ms                                                                       | 248 ms: 1.02x slower                                                       |
| xml_etree_parse          | 145 ms                                                                       | 148 ms: 1.02x slower                                                       |
| typing_runtime_protocols | 118 us                                                                       | 121 us: 1.02x slower                                                       |
| regex_v8                 | 25.4 ms                                                                      | 26.1 ms: 1.03x slower                                                      |
| regex_effbot             | 3.46 ms                                                                      | 3.61 ms: 1.04x slower                                                      |
| unpack_sequence          | 43.8 ns                                                                      | 45.8 ns: 1.04x slower                                                      |
| gc_traversal             | 3.66 ms                                                                      | 3.88 ms: 1.06x slower                                                      |
| Geometric mean           | (ref)                                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (20): bench_thread_pool, tomli_loads, pprint_safe_repr, xml_etree_iterparse, sqlite_synth, bench_mp_pool, pathlib, async_tree_cpu_io_mixed, telco, pickle_pure_python, sqlglot_optimize, asyncio_websockets, async_tree_memoization_tg, async_tree_memoization, dask, mypy2, async_tree_cpu_io_mixed_tg, go, async_tree_none, tornado_http


# HPT report

- Reliability score: 97.67% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x