
# Results vs. 3.12.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.17x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 241 ms: 1.16x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.62 ms: 1.38x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.77 sec: 1.12x faster                                                          |
| tornado_http   | 105 ms                                                          | 97.5 ms: 1.08x faster                                                           |
| Geometric mean | (ref)                                                           | 1.18x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 234 ms: 1.19x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 296 ms: 1.18x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 313 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 585 ms: 1.16x faster                                                            |
| async_tree_io              | 693 ms                                                          | 602 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 507 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 495 ms: 1.10x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.16x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 79.5 ms: 1.60x faster                                                           |
| float          | 76.7 ms                                                         | 56.4 ms: 1.36x faster                                                           |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.30x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 104 ms: 1.24x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| regex_dna      | 127 ms                                                          | 120 ms: 1.06x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 148 us: 1.42x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 206 us: 1.39x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.65 sec: 1.33x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 40.4 ms: 1.32x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 58.5 ms: 1.23x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 66.3 ms: 1.17x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.72 ms: 1.10x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 108 ms: 1.05x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| json_loads           | 20.4 us                                                         | 19.9 us: 1.02x faster                                                           |
| unpickle_list        | 2.95 us                                                         | 2.89 us: 1.02x faster                                                           |
| unpickle             | 9.71 us                                                         | 9.82 us: 1.01x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.14x faster                                                                    |

Benchmark hidden because not significant (2): pickle_dict, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.1 ms: 1.01x faster                                                           |
| python_startup_no_site | 19.1 ms                                                         | 19.9 ms: 1.04x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.02x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.57 ms: 1.32x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.3 ms: 1.72x faster                                                           |
| logging_silent             | 101 ns                                                          | 59.1 ns: 1.71x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 23.1 us: 1.66x faster                                                           |
| scimark_sor                | 130 ms                                                          | 78.4 ms: 1.66x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 38.6 ns: 1.62x faster                                                           |
| nbody                      | 127 ms                                                          | 79.5 ms: 1.60x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.31 ms: 1.55x faster                                                           |
| comprehensions             | 19.2 us                                                         | 12.6 us: 1.52x faster                                                           |
| raytrace                   | 308 ms                                                          | 205 ms: 1.50x faster                                                            |
| scimark_lu                 | 93.2 ms                                                         | 62.3 ms: 1.50x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.2 ms: 1.47x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 88.4 us: 1.43x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 148 us: 1.42x faster                                                            |
| richards_super             | 46.5 ms                                                         | 33.5 ms: 1.39x faster                                                           |
| richards                   | 41.3 ms                                                         | 29.8 ms: 1.39x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 206 us: 1.39x faster                                                            |
| sqlglot_parse              | 1.25 ms                                                         | 905 us: 1.38x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.62 ms: 1.38x faster                                                           |
| float                      | 76.7 ms                                                         | 56.4 ms: 1.36x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 5.06 ms: 1.35x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.14 ms: 1.34x faster                                                           |
| deepcopy                   | 360 us                                                          | 270 us: 1.33x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.65 sec: 1.33x faster                                                          |
| spectral_norm              | 104 ms                                                          | 78.1 ms: 1.33x faster                                                           |
| go                         | 137 ms                                                          | 103 ms: 1.33x faster                                                            |
| xml_etree_process          | 53.2 ms                                                         | 40.4 ms: 1.32x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.57 ms: 1.32x faster                                                           |
| chaos                      | 69.4 ms                                                         | 53.5 ms: 1.30x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 51.3 ms: 1.29x faster                                                           |
| pyflate                    | 424 ms                                                          | 329 ms: 1.29x faster                                                            |
| scimark_fft                | 271 ms                                                          | 211 ms: 1.28x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.52 us: 1.28x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 73.6 ms: 1.27x faster                                                           |
| regex_compile              | 129 ms                                                          | 104 ms: 1.24x faster                                                            |
| fannkuch                   | 354 ms                                                          | 287 ms: 1.23x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 58.5 ms: 1.23x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.22 sec: 1.23x faster                                                          |
| logging_simple             | 9.75 us                                                         | 7.95 us: 1.23x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.15 ms: 1.22x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 56.6 ms: 1.22x faster                                                           |
| logging_format             | 10.4 us                                                         | 8.57 us: 1.21x faster                                                           |
| pprint_safe_repr           | 721 ms                                                          | 598 ms: 1.21x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 40.4 ms: 1.20x faster                                                           |
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 234 ms: 1.19x faster                                                            |
| async_generators           | 313 ms                                                          | 265 ms: 1.18x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 296 ms: 1.18x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 66.3 ms: 1.17x faster                                                           |
| pycparser                  | 978 ms                                                          | 837 ms: 1.17x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.0 ms: 1.17x faster                                                           |
| async_tree_memoization     | 364 ms                                                          | 313 ms: 1.16x faster                                                            |
| 2to3                       | 280 ms                                                          | 241 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 585 ms: 1.16x faster                                                            |
| async_tree_io              | 693 ms                                                          | 602 ms: 1.15x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 108 ms: 1.14x faster                                                            |
| sympy_str                  | 240 ms                                                          | 211 ms: 1.14x faster                                                            |
| meteor_contest             | 86.9 ms                                                         | 76.8 ms: 1.13x faster                                                           |
| mdp                        | 1.91 sec                                                        | 1.70 sec: 1.13x faster                                                          |
| docutils                   | 1.98 sec                                                        | 1.77 sec: 1.12x faster                                                          |
| sqlite_synth               | 2.07 us                                                         | 1.86 us: 1.11x faster                                                           |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 507 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 495 ms: 1.10x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.00 ms: 1.10x faster                                                           |
| json_dumps                 | 7.40 ms                                                         | 6.72 ms: 1.10x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 84.0 ms: 1.09x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 69.5 ms: 1.08x faster                                                           |
| asyncio_tcp                | 662 ms                                                          | 611 ms: 1.08x faster                                                            |
| sympy_expand               | 398 ms                                                          | 369 ms: 1.08x faster                                                            |
| tornado_http               | 105 ms                                                          | 97.5 ms: 1.08x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| dask                       | 323 ms                                                          | 302 ms: 1.07x faster                                                            |
| regex_dna                  | 127 ms                                                          | 120 ms: 1.06x faster                                                            |
| xml_etree_parse            | 113 ms                                                          | 108 ms: 1.05x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.37 ms: 1.05x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                          |
| pickle_list                | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| json_loads                 | 20.4 us                                                         | 19.9 us: 1.02x faster                                                           |
| unpickle_list              | 2.95 us                                                         | 2.89 us: 1.02x faster                                                           |
| python_startup             | 22.4 ms                                                         | 22.1 ms: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| json                       | 4.15 ms                                                         | 4.19 ms: 1.01x slower                                                           |
| unpickle                   | 9.71 us                                                         | 9.82 us: 1.01x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 19.9 ms: 1.04x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.86 ms: 1.06x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 207 ms: 2.06x slower                                                            |
| coverage                   | 48.4 ms                                                         | 469 ms: 9.69x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                    |

Benchmark hidden because not significant (3): create_gc_cycles, pickle_dict, pickle
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown