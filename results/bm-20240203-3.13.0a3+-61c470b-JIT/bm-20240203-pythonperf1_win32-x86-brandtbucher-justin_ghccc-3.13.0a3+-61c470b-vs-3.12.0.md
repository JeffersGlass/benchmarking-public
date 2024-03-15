
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-x86
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.17x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 247 ms: 1.13x faster                                                          |
| chameleon      | 7.75 ms                                                         | 5.72 ms: 1.35x faster                                                         |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                        |
| tornado_http   | 105 ms                                                          | 99.1 ms: 1.06x faster                                                         |
| Geometric mean | (ref)                                                           | 1.16x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 246 ms: 1.21x faster                                                          |
| async_tree_memoization_tg  | 350 ms                                                          | 292 ms: 1.20x faster                                                          |
| async_tree_none_tg         | 278 ms                                                          | 236 ms: 1.17x faster                                                          |
| async_tree_memoization     | 364 ms                                                          | 314 ms: 1.16x faster                                                          |
| async_tree_io              | 693 ms                                                          | 599 ms: 1.16x faster                                                          |
| async_tree_io_tg           | 677 ms                                                          | 596 ms: 1.14x faster                                                          |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 522 ms: 1.08x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 510 ms: 1.07x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.15x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 61.4 ms: 2.07x faster                                                         |
| float          | 76.7 ms                                                         | 49.8 ms: 1.54x faster                                                         |
| pidigits       | 199 ms                                                          | 202 ms: 1.01x slower                                                          |
| Geometric mean | (ref)                                                           | 1.46x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 99.2 ms: 1.30x faster                                                         |
| regex_effbot   | 2.04 ms                                                         | 1.93 ms: 1.06x faster                                                         |
| regex_dna      | 127 ms                                                          | 121 ms: 1.05x faster                                                          |
| regex_v8       | 15.0 ms                                                         | 16.4 ms: 1.09x slower                                                         |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                        | 1.46 sec: 1.51x faster                                                        |
| unpickle_pure_python | 210 us                                                          | 147 us: 1.42x faster                                                          |
| pickle_pure_python   | 286 us                                                          | 209 us: 1.37x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 40.5 ms: 1.32x faster                                                         |
| xml_etree_generate   | 72.1 ms                                                         | 57.8 ms: 1.25x faster                                                         |
| xml_etree_iterparse  | 77.6 ms                                                         | 65.0 ms: 1.19x faster                                                         |
| json_dumps           | 7.40 ms                                                         | 6.66 ms: 1.11x faster                                                         |
| pickle_list          | 3.37 us                                                         | 3.24 us: 1.04x faster                                                         |
| xml_etree_parse      | 113 ms                                                          | 110 ms: 1.03x faster                                                          |
| pickle_dict          | 19.9 us                                                         | 19.8 us: 1.01x faster                                                         |
| unpickle_list        | 2.95 us                                                         | 3.04 us: 1.03x slower                                                         |
| pickle               | 7.79 us                                                         | 8.11 us: 1.04x slower                                                         |
| unpickle             | 9.71 us                                                         | 10.2 us: 1.05x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.14x faster                                                                  |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.2 ms: 1.04x slower                                                         |
| python_startup_no_site | 19.1 ms                                                         | 21.1 ms: 1.11x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 6.37 ms: 1.56x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody                      | 127 ms                                                          | 61.4 ms: 2.07x faster                                                         |
| generators                 | 38.5 ms                                                         | 22.2 ms: 1.73x faster                                                         |
| deepcopy_memo              | 38.4 us                                                         | 22.8 us: 1.68x faster                                                         |
| logging_silent             | 101 ns                                                          | 61.2 ns: 1.65x faster                                                         |
| deltablue                  | 3.58 ms                                                         | 2.18 ms: 1.65x faster                                                         |
| spectral_norm              | 104 ms                                                          | 63.2 ms: 1.64x faster                                                         |
| comprehensions             | 19.2 us                                                         | 12.1 us: 1.59x faster                                                         |
| scimark_sor                | 130 ms                                                          | 82.3 ms: 1.58x faster                                                         |
| mako                       | 9.96 ms                                                         | 6.37 ms: 1.56x faster                                                         |
| float                      | 76.7 ms                                                         | 49.8 ms: 1.54x faster                                                         |
| scimark_lu                 | 93.2 ms                                                         | 60.7 ms: 1.54x faster                                                         |
| tomli_loads                | 2.20 sec                                                        | 1.46 sec: 1.51x faster                                                        |
| unpack_sequence            | 62.5 ns                                                         | 42.7 ns: 1.46x faster                                                         |
| raytrace                   | 308 ms                                                          | 213 ms: 1.45x faster                                                          |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 2.69 ms: 1.43x faster                                                         |
| coroutines                 | 20.9 ms                                                         | 14.6 ms: 1.43x faster                                                         |
| unpickle_pure_python       | 210 us                                                          | 147 us: 1.42x faster                                                          |
| sqlglot_parse              | 1.25 ms                                                         | 884 us: 1.41x faster                                                          |
| richards                   | 41.3 ms                                                         | 29.5 ms: 1.40x faster                                                         |
| richards_super             | 46.5 ms                                                         | 33.4 ms: 1.39x faster                                                         |
| scimark_fft                | 271 ms                                                          | 197 ms: 1.38x faster                                                          |
| pickle_pure_python         | 286 us                                                          | 209 us: 1.37x faster                                                          |
| sqlglot_transpile          | 1.53 ms                                                         | 1.12 ms: 1.36x faster                                                         |
| crypto_pyaes               | 69.2 ms                                                         | 51.1 ms: 1.36x faster                                                         |
| chameleon                  | 7.75 ms                                                         | 5.72 ms: 1.35x faster                                                         |
| deepcopy                   | 360 us                                                          | 266 us: 1.35x faster                                                          |
| deepcopy_reduce            | 3.23 us                                                         | 2.40 us: 1.35x faster                                                         |
| fannkuch                   | 354 ms                                                          | 263 ms: 1.35x faster                                                          |
| chaos                      | 69.4 ms                                                         | 51.6 ms: 1.34x faster                                                         |
| xml_etree_process          | 53.2 ms                                                         | 40.5 ms: 1.32x faster                                                         |
| pyflate                    | 424 ms                                                          | 325 ms: 1.31x faster                                                          |
| regex_compile              | 129 ms                                                          | 99.2 ms: 1.30x faster                                                         |
| typing_runtime_protocols   | 126 us                                                          | 98.0 us: 1.29x faster                                                         |
| logging_simple             | 9.75 us                                                         | 7.63 us: 1.28x faster                                                         |
| nqueens                    | 93.7 ms                                                         | 73.7 ms: 1.27x faster                                                         |
| xml_etree_generate         | 72.1 ms                                                         | 57.8 ms: 1.25x faster                                                         |
| logging_format             | 10.4 us                                                         | 8.38 us: 1.24x faster                                                         |
| pprint_pformat             | 1.50 sec                                                        | 1.23 sec: 1.22x faster                                                        |
| pprint_safe_repr           | 721 ms                                                          | 593 ms: 1.21x faster                                                          |
| go                         | 137 ms                                                          | 113 ms: 1.21x faster                                                          |
| async_tree_none            | 298 ms                                                          | 246 ms: 1.21x faster                                                          |
| sqlglot_optimize           | 48.5 ms                                                         | 40.2 ms: 1.21x faster                                                         |
| async_tree_memoization_tg  | 350 ms                                                          | 292 ms: 1.20x faster                                                          |
| hexiom                     | 6.82 ms                                                         | 5.70 ms: 1.20x faster                                                         |
| xml_etree_iterparse        | 77.6 ms                                                         | 65.0 ms: 1.19x faster                                                         |
| pycparser                  | 978 ms                                                          | 822 ms: 1.19x faster                                                          |
| async_tree_none_tg         | 278 ms                                                          | 236 ms: 1.17x faster                                                          |
| sympy_str                  | 240 ms                                                          | 205 ms: 1.17x faster                                                          |
| sympy_sum                  | 123 ms                                                          | 106 ms: 1.16x faster                                                          |
| async_tree_memoization     | 364 ms                                                          | 314 ms: 1.16x faster                                                          |
| async_tree_io              | 693 ms                                                          | 599 ms: 1.16x faster                                                          |
| sympy_integrate            | 17.5 ms                                                         | 15.2 ms: 1.15x faster                                                         |
| sqlite_synth               | 2.07 us                                                         | 1.82 us: 1.14x faster                                                         |
| async_tree_io_tg           | 677 ms                                                          | 596 ms: 1.14x faster                                                          |
| scimark_monte_carlo        | 66.4 ms                                                         | 58.6 ms: 1.13x faster                                                         |
| 2to3                       | 280 ms                                                          | 247 ms: 1.13x faster                                                          |
| sympy_expand               | 398 ms                                                          | 357 ms: 1.11x faster                                                          |
| async_generators           | 313 ms                                                          | 282 ms: 1.11x faster                                                          |
| json_dumps                 | 7.40 ms                                                         | 6.66 ms: 1.11x faster                                                         |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                        |
| meteor_contest             | 86.9 ms                                                         | 79.4 ms: 1.09x faster                                                         |
| mdp                        | 1.91 sec                                                        | 1.75 sec: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 522 ms: 1.08x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 510 ms: 1.07x faster                                                          |
| tornado_http               | 105 ms                                                          | 99.1 ms: 1.06x faster                                                         |
| regex_effbot               | 2.04 ms                                                         | 1.93 ms: 1.06x faster                                                         |
| dask                       | 323 ms                                                          | 306 ms: 1.06x faster                                                          |
| regex_dna                  | 127 ms                                                          | 121 ms: 1.05x faster                                                          |
| bench_thread_pool          | 1.10 ms                                                         | 1.05 ms: 1.05x faster                                                         |
| pickle_list                | 3.37 us                                                         | 3.24 us: 1.04x faster                                                         |
| pathlib                    | 91.4 ms                                                         | 88.8 ms: 1.03x faster                                                         |
| xml_etree_parse            | 113 ms                                                          | 110 ms: 1.03x faster                                                          |
| gc_traversal               | 1.44 ms                                                         | 1.40 ms: 1.03x faster                                                         |
| bench_mp_pool              | 75.4 ms                                                         | 74.4 ms: 1.01x faster                                                         |
| pickle_dict                | 19.9 us                                                         | 19.8 us: 1.01x faster                                                         |
| pidigits                   | 199 ms                                                          | 202 ms: 1.01x slower                                                          |
| create_gc_cycles           | 652 us                                                          | 668 us: 1.02x slower                                                          |
| telco                      | 5.51 ms                                                         | 5.68 ms: 1.03x slower                                                         |
| unpickle_list              | 2.95 us                                                         | 3.04 us: 1.03x slower                                                         |
| python_startup             | 22.4 ms                                                         | 23.2 ms: 1.04x slower                                                         |
| pickle                     | 7.79 us                                                         | 8.11 us: 1.04x slower                                                         |
| unpickle                   | 9.71 us                                                         | 10.2 us: 1.05x slower                                                         |
| regex_v8                   | 15.0 ms                                                         | 16.4 ms: 1.09x slower                                                         |
| python_startup_no_site     | 19.1 ms                                                         | 21.1 ms: 1.11x slower                                                         |
| sqlglot_normalize          | 100 ms                                                          | 203 ms: 2.03x slower                                                          |
| coverage                   | 48.4 ms                                                         | 473 ms: 9.76x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                  |

Benchmark hidden because not significant (4): asyncio_tcp, asyncio_tcp_ssl, json_loads, json
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown