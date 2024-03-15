
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_cold
- machine: windows-x86
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 251 ms: 1.12x faster                                                         |
| chameleon      | 7.75 ms                                                         | 5.97 ms: 1.30x faster                                                        |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                       |
| tornado_http   | 105 ms                                                          | 97.1 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none_tg         | 278 ms                                                          | 244 ms: 1.14x faster                                                         |
| async_tree_none            | 298 ms                                                          | 262 ms: 1.14x faster                                                         |
| async_tree_memoization_tg  | 350 ms                                                          | 311 ms: 1.13x faster                                                         |
| async_tree_memoization     | 364 ms                                                          | 328 ms: 1.11x faster                                                         |
| async_tree_io_tg           | 677 ms                                                          | 611 ms: 1.11x faster                                                         |
| async_tree_io              | 693 ms                                                          | 637 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 524 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 515 ms: 1.06x faster                                                         |
| Geometric mean             | (ref)                                                           | 1.10x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 56.2 ms: 1.36x faster                                                        |
| nbody          | 127 ms                                                          | 97.0 ms: 1.31x faster                                                        |
| pidigits       | 199 ms                                                          | 204 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                           | 1.20x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 106 ms: 1.22x faster                                                         |
| regex_dna      | 127 ms                                                          | 121 ms: 1.05x faster                                                         |
| regex_effbot   | 2.04 ms                                                         | 1.94 ms: 1.05x faster                                                        |
| regex_v8       | 15.0 ms                                                         | 16.6 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 151 us: 1.39x faster                                                         |
| pickle_pure_python   | 286 us                                                          | 210 us: 1.36x faster                                                         |
| tomli_loads          | 2.20 sec                                                        | 1.67 sec: 1.32x faster                                                       |
| xml_etree_process    | 53.2 ms                                                         | 42.2 ms: 1.26x faster                                                        |
| xml_etree_generate   | 72.1 ms                                                         | 61.3 ms: 1.18x faster                                                        |
| xml_etree_iterparse  | 77.6 ms                                                         | 69.9 ms: 1.11x faster                                                        |
| json_dumps           | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                        |
| pickle_list          | 3.37 us                                                         | 3.22 us: 1.04x faster                                                        |
| json_loads           | 20.4 us                                                         | 19.6 us: 1.04x faster                                                        |
| xml_etree_parse      | 113 ms                                                          | 111 ms: 1.02x faster                                                         |
| pickle_dict          | 19.9 us                                                         | 19.8 us: 1.01x faster                                                        |
| unpickle_list        | 2.95 us                                                         | 3.04 us: 1.03x slower                                                        |
| pickle               | 7.79 us                                                         | 8.28 us: 1.06x slower                                                        |
| unpickle             | 9.71 us                                                         | 10.3 us: 1.07x slower                                                        |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.1 ms: 1.03x slower                                                        |
| python_startup_no_site | 19.1 ms                                                         | 21.0 ms: 1.10x slower                                                        |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.97 ms: 1.25x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.7 ms: 1.70x faster                                                        |
| deepcopy_memo              | 38.4 us                                                         | 23.2 us: 1.65x faster                                                        |
| logging_silent             | 101 ns                                                          | 61.6 ns: 1.64x faster                                                        |
| unpack_sequence            | 62.5 ns                                                         | 39.7 ns: 1.57x faster                                                        |
| scimark_sor                | 130 ms                                                          | 83.4 ms: 1.56x faster                                                        |
| scimark_lu                 | 93.2 ms                                                         | 60.6 ms: 1.54x faster                                                        |
| coroutines                 | 20.9 ms                                                         | 14.5 ms: 1.44x faster                                                        |
| richards                   | 41.3 ms                                                         | 29.0 ms: 1.42x faster                                                        |
| deltablue                  | 3.58 ms                                                         | 2.52 ms: 1.42x faster                                                        |
| richards_super             | 46.5 ms                                                         | 33.1 ms: 1.40x faster                                                        |
| unpickle_pure_python       | 210 us                                                          | 151 us: 1.39x faster                                                         |
| float                      | 76.7 ms                                                         | 56.2 ms: 1.36x faster                                                        |
| pickle_pure_python         | 286 us                                                          | 210 us: 1.36x faster                                                         |
| sqlglot_parse              | 1.25 ms                                                         | 918 us: 1.36x faster                                                         |
| raytrace                   | 308 ms                                                          | 227 ms: 1.36x faster                                                         |
| spectral_norm              | 104 ms                                                          | 78.2 ms: 1.33x faster                                                        |
| deepcopy_reduce            | 3.23 us                                                         | 2.45 us: 1.32x faster                                                        |
| tomli_loads                | 2.20 sec                                                        | 1.67 sec: 1.32x faster                                                       |
| nbody                      | 127 ms                                                          | 97.0 ms: 1.31x faster                                                        |
| sqlglot_transpile          | 1.53 ms                                                         | 1.18 ms: 1.30x faster                                                        |
| chameleon                  | 7.75 ms                                                         | 5.97 ms: 1.30x faster                                                        |
| deepcopy                   | 360 us                                                          | 278 us: 1.29x faster                                                         |
| typing_runtime_protocols   | 126 us                                                          | 97.9 us: 1.29x faster                                                        |
| xml_etree_process          | 53.2 ms                                                         | 42.2 ms: 1.26x faster                                                        |
| mako                       | 9.96 ms                                                         | 7.97 ms: 1.25x faster                                                        |
| comprehensions             | 19.2 us                                                         | 15.7 us: 1.22x faster                                                        |
| regex_compile              | 129 ms                                                          | 106 ms: 1.22x faster                                                         |
| logging_format             | 10.4 us                                                         | 8.71 us: 1.19x faster                                                        |
| logging_simple             | 9.75 us                                                         | 8.19 us: 1.19x faster                                                        |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.26 ms: 1.18x faster                                                        |
| pycparser                  | 978 ms                                                          | 830 ms: 1.18x faster                                                         |
| xml_etree_generate         | 72.1 ms                                                         | 61.3 ms: 1.18x faster                                                        |
| chaos                      | 69.4 ms                                                         | 59.5 ms: 1.17x faster                                                        |
| go                         | 137 ms                                                          | 119 ms: 1.15x faster                                                         |
| sqlglot_optimize           | 48.5 ms                                                         | 42.5 ms: 1.14x faster                                                        |
| async_tree_none_tg         | 278 ms                                                          | 244 ms: 1.14x faster                                                         |
| async_tree_none            | 298 ms                                                          | 262 ms: 1.14x faster                                                         |
| fannkuch                   | 354 ms                                                          | 313 ms: 1.13x faster                                                         |
| async_tree_memoization_tg  | 350 ms                                                          | 311 ms: 1.13x faster                                                         |
| 2to3                       | 280 ms                                                          | 251 ms: 1.12x faster                                                         |
| xml_etree_iterparse        | 77.6 ms                                                         | 69.9 ms: 1.11x faster                                                        |
| async_tree_memoization     | 364 ms                                                          | 328 ms: 1.11x faster                                                         |
| async_tree_io_tg           | 677 ms                                                          | 611 ms: 1.11x faster                                                         |
| sqlite_synth               | 2.07 us                                                         | 1.87 us: 1.11x faster                                                        |
| pyflate                    | 424 ms                                                          | 383 ms: 1.11x faster                                                         |
| sympy_sum                  | 123 ms                                                          | 112 ms: 1.10x faster                                                         |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                       |
| sympy_str                  | 240 ms                                                          | 219 ms: 1.10x faster                                                         |
| crypto_pyaes               | 69.2 ms                                                         | 63.3 ms: 1.09x faster                                                        |
| sympy_integrate            | 17.5 ms                                                         | 16.1 ms: 1.09x faster                                                        |
| async_tree_io              | 693 ms                                                          | 637 ms: 1.09x faster                                                         |
| tornado_http               | 105 ms                                                          | 97.1 ms: 1.08x faster                                                        |
| sympy_expand               | 398 ms                                                          | 369 ms: 1.08x faster                                                         |
| json_dumps                 | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 524 ms: 1.08x faster                                                         |
| nqueens                    | 93.7 ms                                                         | 87.1 ms: 1.07x faster                                                        |
| scimark_fft                | 271 ms                                                          | 254 ms: 1.07x faster                                                         |
| async_generators           | 313 ms                                                          | 294 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 515 ms: 1.06x faster                                                         |
| regex_dna                  | 127 ms                                                          | 121 ms: 1.05x faster                                                         |
| regex_effbot               | 2.04 ms                                                         | 1.94 ms: 1.05x faster                                                        |
| pprint_safe_repr           | 721 ms                                                          | 688 ms: 1.05x faster                                                         |
| pickle_list                | 3.37 us                                                         | 3.22 us: 1.04x faster                                                        |
| dask                       | 323 ms                                                          | 310 ms: 1.04x faster                                                         |
| pprint_pformat             | 1.50 sec                                                        | 1.43 sec: 1.04x faster                                                       |
| json_loads                 | 20.4 us                                                         | 19.6 us: 1.04x faster                                                        |
| pathlib                    | 91.4 ms                                                         | 88.8 ms: 1.03x faster                                                        |
| json                       | 4.15 ms                                                         | 4.07 ms: 1.02x faster                                                        |
| xml_etree_parse            | 113 ms                                                          | 111 ms: 1.02x faster                                                         |
| hexiom                     | 6.82 ms                                                         | 6.72 ms: 1.02x faster                                                        |
| gc_traversal               | 1.44 ms                                                         | 1.42 ms: 1.01x faster                                                        |
| pickle_dict                | 19.9 us                                                         | 19.8 us: 1.01x faster                                                        |
| meteor_contest             | 86.9 ms                                                         | 87.5 ms: 1.01x slower                                                        |
| mdp                        | 1.91 sec                                                        | 1.93 sec: 1.01x slower                                                       |
| create_gc_cycles           | 652 us                                                          | 660 us: 1.01x slower                                                         |
| pidigits                   | 199 ms                                                          | 204 ms: 1.02x slower                                                         |
| unpickle_list              | 2.95 us                                                         | 3.04 us: 1.03x slower                                                        |
| python_startup             | 22.4 ms                                                         | 23.1 ms: 1.03x slower                                                        |
| scimark_monte_carlo        | 66.4 ms                                                         | 69.4 ms: 1.04x slower                                                        |
| pickle                     | 7.79 us                                                         | 8.28 us: 1.06x slower                                                        |
| unpickle                   | 9.71 us                                                         | 10.3 us: 1.07x slower                                                        |
| python_startup_no_site     | 19.1 ms                                                         | 21.0 ms: 1.10x slower                                                        |
| regex_v8                   | 15.0 ms                                                         | 16.6 ms: 1.10x slower                                                        |
| telco                      | 5.51 ms                                                         | 6.11 ms: 1.11x slower                                                        |
| sqlglot_normalize          | 100 ms                                                          | 221 ms: 2.20x slower                                                         |
| coverage                   | 48.4 ms                                                         | 480 ms: 9.92x slower                                                         |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                                 |

Benchmark hidden because not significant (4): bench_thread_pool, asyncio_tcp_ssl, asyncio_tcp, bench_mp_pool
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown