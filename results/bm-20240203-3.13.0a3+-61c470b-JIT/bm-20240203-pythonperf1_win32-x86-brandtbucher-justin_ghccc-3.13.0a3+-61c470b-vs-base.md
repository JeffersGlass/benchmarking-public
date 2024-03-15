# Results vs. base

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-x86
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.06x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 252 ms                                                                          | 247 ms: 1.02x faster                                                          |
| chameleon      | 6.21 ms                                                                         | 5.72 ms: 1.08x faster                                                         |
| docutils       | 1.83 sec                                                                        | 1.81 sec: 1.01x faster                                                        |
| tornado_http   | 97.9 ms                                                                         | 99.1 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                                           | 1.03x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 313 ms                                                                          | 292 ms: 1.07x faster                                                          |
| async_tree_none            | 263 ms                                                                          | 246 ms: 1.07x faster                                                          |
| async_tree_memoization     | 329 ms                                                                          | 314 ms: 1.05x faster                                                          |
| async_tree_io              | 628 ms                                                                          | 599 ms: 1.05x faster                                                          |
| async_tree_cpu_io_mixed_tg | 534 ms                                                                          | 510 ms: 1.05x faster                                                          |
| async_tree_cpu_io_mixed    | 540 ms                                                                          | 522 ms: 1.03x faster                                                          |
| async_tree_none_tg         | 242 ms                                                                          | 236 ms: 1.02x faster                                                          |
| async_tree_io_tg           | 610 ms                                                                          | 596 ms: 1.02x faster                                                          |
| Geometric mean             | (ref)                                                                           | 1.05x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody          | 91.3 ms                                                                         | 61.4 ms: 1.49x faster                                                         |
| float          | 55.0 ms                                                                         | 49.8 ms: 1.10x faster                                                         |
| pidigits       | 203 ms                                                                          | 202 ms: 1.00x faster                                                          |
| Geometric mean | (ref)                                                                           | 1.18x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 108 ms                                                                          | 99.2 ms: 1.09x faster                                                         |
| regex_dna      | 125 ms                                                                          | 121 ms: 1.04x faster                                                          |
| Geometric mean | (ref)                                                                           | 1.03x faster                                                                  |

Benchmark hidden because not significant (2): regex_effbot, regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| tomli_loads          | 1.63 sec                                                                        | 1.46 sec: 1.12x faster                                                        |
| xml_etree_process    | 41.9 ms                                                                         | 40.5 ms: 1.04x faster                                                         |
| xml_etree_iterparse  | 67.2 ms                                                                         | 65.0 ms: 1.03x faster                                                         |
| xml_etree_generate   | 59.7 ms                                                                         | 57.8 ms: 1.03x faster                                                         |
| unpickle_pure_python | 151 us                                                                          | 147 us: 1.03x faster                                                          |
| json_dumps           | 6.81 ms                                                                         | 6.66 ms: 1.02x faster                                                         |
| unpickle_list        | 3.10 us                                                                         | 3.04 us: 1.02x faster                                                         |
| json_loads           | 20.6 us                                                                         | 20.3 us: 1.01x faster                                                         |
| pickle_pure_python   | 212 us                                                                          | 209 us: 1.01x faster                                                          |
| unpickle             | 10.3 us                                                                         | 10.2 us: 1.01x faster                                                         |
| pickle_dict          | 19.9 us                                                                         | 19.8 us: 1.01x faster                                                         |
| xml_etree_parse      | 108 ms                                                                          | 110 ms: 1.01x slower                                                          |
| Geometric mean       | (ref)                                                                           | 1.02x faster                                                                  |

Benchmark hidden because not significant (2): pickle_list, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup | 23.3 ms                                                                         | 23.2 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                                  |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 7.79 ms                                                                         | 6.37 ms: 1.22x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20240130-pythonperf1_win32-x86-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody                      | 91.3 ms                                                                         | 61.4 ms: 1.49x faster                                                         |
| scimark_fft                | 255 ms                                                                          | 197 ms: 1.30x faster                                                          |
| scimark_monte_carlo        | 74.0 ms                                                                         | 58.6 ms: 1.26x faster                                                         |
| spectral_norm              | 79.0 ms                                                                         | 63.2 ms: 1.25x faster                                                         |
| mako                       | 7.79 ms                                                                         | 6.37 ms: 1.22x faster                                                         |
| comprehensions             | 14.7 us                                                                         | 12.1 us: 1.22x faster                                                         |
| scimark_sparse_mat_mult    | 3.24 ms                                                                         | 2.69 ms: 1.20x faster                                                         |
| crypto_pyaes               | 61.3 ms                                                                         | 51.1 ms: 1.20x faster                                                         |
| nqueens                    | 88.5 ms                                                                         | 73.7 ms: 1.20x faster                                                         |
| pprint_pformat             | 1.47 sec                                                                        | 1.23 sec: 1.19x faster                                                        |
| fannkuch                   | 312 ms                                                                          | 263 ms: 1.19x faster                                                          |
| pprint_safe_repr           | 703 ms                                                                          | 593 ms: 1.18x faster                                                          |
| chaos                      | 59.9 ms                                                                         | 51.6 ms: 1.16x faster                                                         |
| deltablue                  | 2.50 ms                                                                         | 2.18 ms: 1.15x faster                                                         |
| pyflate                    | 366 ms                                                                          | 325 ms: 1.13x faster                                                          |
| hexiom                     | 6.37 ms                                                                         | 5.70 ms: 1.12x faster                                                         |
| tomli_loads                | 1.63 sec                                                                        | 1.46 sec: 1.12x faster                                                        |
| telco                      | 6.31 ms                                                                         | 5.68 ms: 1.11x faster                                                         |
| raytrace                   | 235 ms                                                                          | 213 ms: 1.11x faster                                                          |
| float                      | 55.0 ms                                                                         | 49.8 ms: 1.10x faster                                                         |
| regex_compile              | 108 ms                                                                          | 99.2 ms: 1.09x faster                                                         |
| chameleon                  | 6.21 ms                                                                         | 5.72 ms: 1.08x faster                                                         |
| deepcopy                   | 287 us                                                                          | 266 us: 1.08x faster                                                          |
| logging_simple             | 8.22 us                                                                         | 7.63 us: 1.08x faster                                                         |
| async_tree_memoization_tg  | 313 ms                                                                          | 292 ms: 1.07x faster                                                          |
| async_tree_none            | 263 ms                                                                          | 246 ms: 1.07x faster                                                          |
| sqlglot_optimize           | 42.9 ms                                                                         | 40.2 ms: 1.07x faster                                                         |
| sqlglot_normalize          | 217 ms                                                                          | 203 ms: 1.07x faster                                                          |
| mdp                        | 1.87 sec                                                                        | 1.75 sec: 1.07x faster                                                        |
| logging_format             | 8.91 us                                                                         | 8.38 us: 1.06x faster                                                         |
| sympy_str                  | 218 ms                                                                          | 205 ms: 1.06x faster                                                          |
| meteor_contest             | 84.2 ms                                                                         | 79.4 ms: 1.06x faster                                                         |
| sympy_sum                  | 112 ms                                                                          | 106 ms: 1.05x faster                                                          |
| sqlglot_transpile          | 1.18 ms                                                                         | 1.12 ms: 1.05x faster                                                         |
| scimark_lu                 | 63.8 ms                                                                         | 60.7 ms: 1.05x faster                                                         |
| async_tree_memoization     | 329 ms                                                                          | 314 ms: 1.05x faster                                                          |
| async_tree_io              | 628 ms                                                                          | 599 ms: 1.05x faster                                                          |
| async_tree_cpu_io_mixed_tg | 534 ms                                                                          | 510 ms: 1.05x faster                                                          |
| sqlglot_parse              | 926 us                                                                          | 884 us: 1.05x faster                                                          |
| sympy_expand               | 372 ms                                                                          | 357 ms: 1.04x faster                                                          |
| sqlite_synth               | 1.89 us                                                                         | 1.82 us: 1.04x faster                                                         |
| regex_dna                  | 125 ms                                                                          | 121 ms: 1.04x faster                                                          |
| sympy_integrate            | 15.8 ms                                                                         | 15.2 ms: 1.04x faster                                                         |
| xml_etree_process          | 41.9 ms                                                                         | 40.5 ms: 1.04x faster                                                         |
| xml_etree_iterparse        | 67.2 ms                                                                         | 65.0 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed    | 540 ms                                                                          | 522 ms: 1.03x faster                                                          |
| xml_etree_generate         | 59.7 ms                                                                         | 57.8 ms: 1.03x faster                                                         |
| richards                   | 30.4 ms                                                                         | 29.5 ms: 1.03x faster                                                         |
| pycparser                  | 847 ms                                                                          | 822 ms: 1.03x faster                                                          |
| deepcopy_memo              | 23.4 us                                                                         | 22.8 us: 1.03x faster                                                         |
| go                         | 116 ms                                                                          | 113 ms: 1.03x faster                                                          |
| unpickle_pure_python       | 151 us                                                                          | 147 us: 1.03x faster                                                          |
| richards_super             | 34.3 ms                                                                         | 33.4 ms: 1.02x faster                                                         |
| async_tree_none_tg         | 242 ms                                                                          | 236 ms: 1.02x faster                                                          |
| deepcopy_reduce            | 2.45 us                                                                         | 2.40 us: 1.02x faster                                                         |
| async_tree_io_tg           | 610 ms                                                                          | 596 ms: 1.02x faster                                                          |
| json_dumps                 | 6.81 ms                                                                         | 6.66 ms: 1.02x faster                                                         |
| bench_thread_pool          | 1.07 ms                                                                         | 1.05 ms: 1.02x faster                                                         |
| 2to3                       | 252 ms                                                                          | 247 ms: 1.02x faster                                                          |
| unpickle_list              | 3.10 us                                                                         | 3.04 us: 1.02x faster                                                         |
| dask                       | 312 ms                                                                          | 306 ms: 1.02x faster                                                          |
| json_loads                 | 20.6 us                                                                         | 20.3 us: 1.01x faster                                                         |
| pickle_pure_python         | 212 us                                                                          | 209 us: 1.01x faster                                                          |
| gc_traversal               | 1.42 ms                                                                         | 1.40 ms: 1.01x faster                                                         |
| bench_mp_pool              | 75.4 ms                                                                         | 74.4 ms: 1.01x faster                                                         |
| async_generators           | 285 ms                                                                          | 282 ms: 1.01x faster                                                          |
| docutils                   | 1.83 sec                                                                        | 1.81 sec: 1.01x faster                                                        |
| scimark_sor                | 83.0 ms                                                                         | 82.3 ms: 1.01x faster                                                         |
| unpickle                   | 10.3 us                                                                         | 10.2 us: 1.01x faster                                                         |
| pickle_dict                | 19.9 us                                                                         | 19.8 us: 1.01x faster                                                         |
| coverage                   | 476 ms                                                                          | 473 ms: 1.01x faster                                                          |
| python_startup             | 23.3 ms                                                                         | 23.2 ms: 1.01x faster                                                         |
| pidigits                   | 203 ms                                                                          | 202 ms: 1.00x faster                                                          |
| tornado_http               | 97.9 ms                                                                         | 99.1 ms: 1.01x slower                                                         |
| typing_runtime_protocols   | 96.7 us                                                                         | 98.0 us: 1.01x slower                                                         |
| xml_etree_parse            | 108 ms                                                                          | 110 ms: 1.01x slower                                                          |
| coroutines                 | 14.4 ms                                                                         | 14.6 ms: 1.02x slower                                                         |
| Geometric mean             | (ref)                                                                           | 1.06x faster                                                                  |

Benchmark hidden because not significant (13): json, asyncio_tcp, asyncio_tcp_ssl, regex_effbot, logging_silent, regex_v8, pickle_list, generators, unpack_sequence, pathlib, python_startup_no_site, pickle, create_gc_cycles


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown