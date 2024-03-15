# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-x86
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 260 ms: 1.08x faster                                                             |
| chameleon      | 7.75 ms                                                         | 5.66 ms: 1.37x faster                                                            |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.09x faster                                                           |
| tornado_http   | 105 ms                                                          | 96.7 ms: 1.09x faster                                                            |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 258 ms: 1.15x faster                                                             |
| async_tree_memoization_tg  | 350 ms                                                          | 304 ms: 1.15x faster                                                             |
| async_tree_none_tg         | 278 ms                                                          | 242 ms: 1.15x faster                                                             |
| async_tree_memoization     | 364 ms                                                          | 323 ms: 1.13x faster                                                             |
| async_tree_io_tg           | 677 ms                                                          | 605 ms: 1.12x faster                                                             |
| async_tree_io              | 693 ms                                                          | 624 ms: 1.11x faster                                                             |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 517 ms: 1.09x faster                                                             |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 504 ms: 1.08x faster                                                             |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 54.9 ms: 1.40x faster                                                            |
| nbody          | 127 ms                                                          | 96.4 ms: 1.32x faster                                                            |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 109 ms: 1.18x faster                                                             |
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                            |
| regex_dna      | 127 ms                                                          | 121 ms: 1.05x faster                                                             |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 286 us                                                          | 210 us: 1.36x faster                                                             |
| tomli_loads          | 2.20 sec                                                        | 1.72 sec: 1.28x faster                                                           |
| xml_etree_process    | 53.2 ms                                                         | 42.1 ms: 1.27x faster                                                            |
| unpickle_pure_python | 210 us                                                          | 171 us: 1.23x faster                                                             |
| xml_etree_generate   | 72.1 ms                                                         | 59.6 ms: 1.21x faster                                                            |
| xml_etree_iterparse  | 77.6 ms                                                         | 67.3 ms: 1.15x faster                                                            |
| json_dumps           | 7.40 ms                                                         | 6.86 ms: 1.08x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.17 us: 1.06x faster                                                            |
| unpickle_list        | 2.95 us                                                         | 2.81 us: 1.05x faster                                                            |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.03x faster                                                             |
| json_loads           | 20.4 us                                                         | 20.1 us: 1.01x faster                                                            |
| pickle_dict          | 19.9 us                                                         | 20.0 us: 1.00x slower                                                            |
| pickle               | 7.79 us                                                         | 7.94 us: 1.02x slower                                                            |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 25.7 ms: 1.15x slower                                                            |
| python_startup_no_site | 19.1 ms                                                         | 23.6 ms: 1.24x slower                                                            |
| Geometric mean         | (ref)                                                           | 1.19x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.30 ms: 1.36x faster                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 59.6 ns: 1.69x faster                                                            |
| generators                 | 38.5 ms                                                         | 23.0 ms: 1.67x faster                                                            |
| deepcopy_memo              | 38.4 us                                                         | 24.3 us: 1.58x faster                                                            |
| coroutines                 | 20.9 ms                                                         | 14.1 ms: 1.48x faster                                                            |
| spectral_norm              | 104 ms                                                          | 71.2 ms: 1.46x faster                                                            |
| unpack_sequence            | 62.5 ns                                                         | 43.1 ns: 1.45x faster                                                            |
| float                      | 76.7 ms                                                         | 54.9 ms: 1.40x faster                                                            |
| deltablue                  | 3.58 ms                                                         | 2.59 ms: 1.38x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 92.1 us: 1.37x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.66 ms: 1.37x faster                                                            |
| mako                       | 9.96 ms                                                         | 7.30 ms: 1.36x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 210 us: 1.36x faster                                                             |
| nbody                      | 127 ms                                                          | 96.4 ms: 1.32x faster                                                            |
| comprehensions             | 19.2 us                                                         | 14.6 us: 1.31x faster                                                            |
| scimark_sor                | 130 ms                                                          | 100 ms: 1.30x faster                                                             |
| deepcopy                   | 360 us                                                          | 278 us: 1.29x faster                                                             |
| deepcopy_reduce            | 3.23 us                                                         | 2.51 us: 1.29x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.72 sec: 1.28x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 979 us: 1.27x faster                                                             |
| xml_etree_process          | 53.2 ms                                                         | 42.1 ms: 1.27x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.23 ms: 1.25x faster                                                            |
| unpickle_pure_python       | 210 us                                                          | 171 us: 1.23x faster                                                             |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.15 ms: 1.22x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 59.6 ms: 1.21x faster                                                            |
| logging_simple             | 9.75 us                                                         | 8.15 us: 1.20x faster                                                            |
| logging_format             | 10.4 us                                                         | 8.74 us: 1.19x faster                                                            |
| richards                   | 41.3 ms                                                         | 34.9 ms: 1.19x faster                                                            |
| richards_super             | 46.5 ms                                                         | 39.2 ms: 1.18x faster                                                            |
| regex_compile              | 129 ms                                                          | 109 ms: 1.18x faster                                                             |
| scimark_fft                | 271 ms                                                          | 233 ms: 1.16x faster                                                             |
| xml_etree_iterparse        | 77.6 ms                                                         | 67.3 ms: 1.15x faster                                                            |
| async_tree_none            | 298 ms                                                          | 258 ms: 1.15x faster                                                             |
| async_tree_memoization_tg  | 350 ms                                                          | 304 ms: 1.15x faster                                                             |
| chaos                      | 69.4 ms                                                         | 60.3 ms: 1.15x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 107 ms: 1.15x faster                                                             |
| crypto_pyaes               | 69.2 ms                                                         | 60.3 ms: 1.15x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 242 ms: 1.15x faster                                                             |
| sympy_integrate            | 17.5 ms                                                         | 15.4 ms: 1.14x faster                                                            |
| go                         | 137 ms                                                          | 120 ms: 1.14x faster                                                             |
| pycparser                  | 978 ms                                                          | 859 ms: 1.14x faster                                                             |
| sympy_str                  | 240 ms                                                          | 210 ms: 1.14x faster                                                             |
| async_tree_memoization     | 364 ms                                                          | 323 ms: 1.13x faster                                                             |
| raytrace                   | 308 ms                                                          | 275 ms: 1.12x faster                                                             |
| async_tree_io_tg           | 677 ms                                                          | 605 ms: 1.12x faster                                                             |
| scimark_lu                 | 93.2 ms                                                         | 83.5 ms: 1.12x faster                                                            |
| pyflate                    | 424 ms                                                          | 382 ms: 1.11x faster                                                             |
| async_tree_io              | 693 ms                                                          | 624 ms: 1.11x faster                                                             |
| mdp                        | 1.91 sec                                                        | 1.74 sec: 1.10x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 6.21 ms: 1.10x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.09x faster                                                           |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 517 ms: 1.09x faster                                                             |
| pathlib                    | 91.4 ms                                                         | 84.2 ms: 1.09x faster                                                            |
| tornado_http               | 105 ms                                                          | 96.7 ms: 1.09x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 504 ms: 1.08x faster                                                             |
| json_dumps                 | 7.40 ms                                                         | 6.86 ms: 1.08x faster                                                            |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                            |
| 2to3                       | 280 ms                                                          | 260 ms: 1.08x faster                                                             |
| sympy_expand               | 398 ms                                                          | 370 ms: 1.08x faster                                                             |
| async_generators           | 313 ms                                                          | 292 ms: 1.07x faster                                                             |
| sqlite_synth               | 2.07 us                                                         | 1.93 us: 1.07x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 45.3 ms: 1.07x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.03 ms: 1.07x faster                                                            |
| pickle_list                | 3.37 us                                                         | 3.17 us: 1.06x faster                                                            |
| regex_dna                  | 127 ms                                                          | 121 ms: 1.05x faster                                                             |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 82.8 ms: 1.05x faster                                                            |
| unpickle_list              | 2.95 us                                                         | 2.81 us: 1.05x faster                                                            |
| asyncio_tcp                | 662 ms                                                          | 638 ms: 1.04x faster                                                             |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.03x faster                                                             |
| fannkuch                   | 354 ms                                                          | 344 ms: 1.03x faster                                                             |
| nqueens                    | 93.7 ms                                                         | 91.4 ms: 1.02x faster                                                            |
| scimark_monte_carlo        | 66.4 ms                                                         | 64.9 ms: 1.02x faster                                                            |
| bench_mp_pool              | 75.4 ms                                                         | 73.9 ms: 1.02x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.42 ms: 1.01x faster                                                            |
| json_loads                 | 20.4 us                                                         | 20.1 us: 1.01x faster                                                            |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                             |
| pickle_dict                | 19.9 us                                                         | 20.0 us: 1.00x slower                                                            |
| json                       | 4.15 ms                                                         | 4.19 ms: 1.01x slower                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.51 sec: 1.01x slower                                                           |
| pickle                     | 7.79 us                                                         | 7.94 us: 1.02x slower                                                            |
| pprint_safe_repr           | 721 ms                                                          | 735 ms: 1.02x slower                                                             |
| create_gc_cycles           | 652 us                                                          | 665 us: 1.02x slower                                                             |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                                            |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                            |
| python_startup             | 22.4 ms                                                         | 25.7 ms: 1.15x slower                                                            |
| telco                      | 5.51 ms                                                         | 6.43 ms: 1.17x slower                                                            |
| python_startup_no_site     | 19.1 ms                                                         | 23.6 ms: 1.24x slower                                                            |
| dask                       | 323 ms                                                          | 413 ms: 1.28x slower                                                             |
| sqlglot_normalize          | 100 ms                                                          | 216 ms: 2.15x slower                                                             |
| coverage                   | 48.4 ms                                                         | 477 ms: 9.84x slower                                                             |
| Geometric mean             | (ref)                                                           | 1.10x faster                                                                     |
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown