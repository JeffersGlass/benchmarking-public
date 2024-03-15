
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: windows-x86
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 262 ms: 1.07x faster                                                          |
| chameleon      | 7.75 ms                                                         | 5.99 ms: 1.29x faster                                                         |
| docutils       | 1.98 sec                                                        | 1.85 sec: 1.07x faster                                                        |
| tornado_http   | 105 ms                                                          | 97.8 ms: 1.07x faster                                                         |
| Geometric mean | (ref)                                                           | 1.12x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 259 ms: 1.15x faster                                                          |
| async_tree_memoization_tg  | 350 ms                                                          | 307 ms: 1.14x faster                                                          |
| async_tree_none_tg         | 278 ms                                                          | 244 ms: 1.14x faster                                                          |
| async_tree_memoization     | 364 ms                                                          | 323 ms: 1.12x faster                                                          |
| async_tree_io_tg           | 677 ms                                                          | 604 ms: 1.12x faster                                                          |
| async_tree_io              | 693 ms                                                          | 621 ms: 1.12x faster                                                          |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 511 ms: 1.10x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 497 ms: 1.10x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 55.1 ms: 1.39x faster                                                         |
| nbody          | 127 ms                                                          | 94.5 ms: 1.34x faster                                                         |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                  |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 117 ms: 1.11x faster                                                          |
| regex_dna      | 127 ms                                                          | 118 ms: 1.08x faster                                                          |
| regex_effbot   | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                         |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                         |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                        | 1.71 sec: 1.28x faster                                                        |
| pickle_pure_python   | 286 us                                                          | 228 us: 1.25x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 42.7 ms: 1.25x faster                                                         |
| xml_etree_generate   | 72.1 ms                                                         | 60.5 ms: 1.19x faster                                                         |
| xml_etree_iterparse  | 77.6 ms                                                         | 67.0 ms: 1.16x faster                                                         |
| unpickle_pure_python | 210 us                                                          | 181 us: 1.16x faster                                                          |
| json_dumps           | 7.40 ms                                                         | 6.90 ms: 1.07x faster                                                         |
| xml_etree_parse      | 113 ms                                                          | 108 ms: 1.05x faster                                                          |
| pickle_list          | 3.37 us                                                         | 3.25 us: 1.04x faster                                                         |
| unpickle_list        | 2.95 us                                                         | 2.85 us: 1.03x faster                                                         |
| json_loads           | 20.4 us                                                         | 20.1 us: 1.01x faster                                                         |
| pickle_dict          | 19.9 us                                                         | 19.8 us: 1.00x faster                                                         |
| pickle               | 7.79 us                                                         | 7.92 us: 1.02x slower                                                         |
| unpickle             | 9.71 us                                                         | 10.0 us: 1.03x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 26.3 ms: 1.18x slower                                                         |
| python_startup_no_site | 19.1 ms                                                         | 23.8 ms: 1.25x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.21x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.25 ms: 1.37x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 24.6 ms: 1.57x faster                                                         |
| spectral_norm              | 104 ms                                                          | 70.7 ms: 1.47x faster                                                         |
| logging_silent             | 101 ns                                                          | 69.0 ns: 1.46x faster                                                         |
| deepcopy_memo              | 38.4 us                                                         | 27.4 us: 1.40x faster                                                         |
| float                      | 76.7 ms                                                         | 55.1 ms: 1.39x faster                                                         |
| mako                       | 9.96 ms                                                         | 7.25 ms: 1.37x faster                                                         |
| coroutines                 | 20.9 ms                                                         | 15.3 ms: 1.36x faster                                                         |
| nbody                      | 127 ms                                                          | 94.5 ms: 1.34x faster                                                         |
| deltablue                  | 3.58 ms                                                         | 2.74 ms: 1.31x faster                                                         |
| comprehensions             | 19.2 us                                                         | 14.7 us: 1.30x faster                                                         |
| chameleon                  | 7.75 ms                                                         | 5.99 ms: 1.29x faster                                                         |
| tomli_loads                | 2.20 sec                                                        | 1.71 sec: 1.28x faster                                                        |
| typing_runtime_protocols   | 126 us                                                          | 99.3 us: 1.27x faster                                                         |
| pickle_pure_python         | 286 us                                                          | 228 us: 1.25x faster                                                          |
| xml_etree_process          | 53.2 ms                                                         | 42.7 ms: 1.25x faster                                                         |
| deepcopy_reduce            | 3.23 us                                                         | 2.59 us: 1.24x faster                                                         |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.11 ms: 1.24x faster                                                         |
| sqlglot_parse              | 1.25 ms                                                         | 1.01 ms: 1.24x faster                                                         |
| scimark_sor                | 130 ms                                                          | 107 ms: 1.21x faster                                                          |
| chaos                      | 69.4 ms                                                         | 57.3 ms: 1.21x faster                                                         |
| deepcopy                   | 360 us                                                          | 298 us: 1.21x faster                                                          |
| sqlglot_transpile          | 1.53 ms                                                         | 1.28 ms: 1.20x faster                                                         |
| xml_etree_generate         | 72.1 ms                                                         | 60.5 ms: 1.19x faster                                                         |
| raytrace                   | 308 ms                                                          | 263 ms: 1.17x faster                                                          |
| xml_etree_iterparse        | 77.6 ms                                                         | 67.0 ms: 1.16x faster                                                         |
| unpickle_pure_python       | 210 us                                                          | 181 us: 1.16x faster                                                          |
| async_tree_none            | 298 ms                                                          | 259 ms: 1.15x faster                                                          |
| logging_simple             | 9.75 us                                                         | 8.50 us: 1.15x faster                                                         |
| logging_format             | 10.4 us                                                         | 9.08 us: 1.15x faster                                                         |
| scimark_fft                | 271 ms                                                          | 237 ms: 1.14x faster                                                          |
| async_tree_memoization_tg  | 350 ms                                                          | 307 ms: 1.14x faster                                                          |
| crypto_pyaes               | 69.2 ms                                                         | 60.8 ms: 1.14x faster                                                         |
| async_tree_none_tg         | 278 ms                                                          | 244 ms: 1.14x faster                                                          |
| pycparser                  | 978 ms                                                          | 869 ms: 1.12x faster                                                          |
| async_tree_memoization     | 364 ms                                                          | 323 ms: 1.12x faster                                                          |
| sympy_sum                  | 123 ms                                                          | 109 ms: 1.12x faster                                                          |
| async_tree_io_tg           | 677 ms                                                          | 604 ms: 1.12x faster                                                          |
| async_tree_io              | 693 ms                                                          | 621 ms: 1.12x faster                                                          |
| go                         | 137 ms                                                          | 123 ms: 1.11x faster                                                          |
| regex_compile              | 129 ms                                                          | 117 ms: 1.11x faster                                                          |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 511 ms: 1.10x faster                                                          |
| pyflate                    | 424 ms                                                          | 384 ms: 1.10x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 497 ms: 1.10x faster                                                          |
| sympy_str                  | 240 ms                                                          | 218 ms: 1.10x faster                                                          |
| mdp                        | 1.91 sec                                                        | 1.74 sec: 1.10x faster                                                        |
| sympy_integrate            | 17.5 ms                                                         | 16.0 ms: 1.10x faster                                                         |
| scimark_lu                 | 93.2 ms                                                         | 85.7 ms: 1.09x faster                                                         |
| regex_dna                  | 127 ms                                                          | 118 ms: 1.08x faster                                                          |
| pathlib                    | 91.4 ms                                                         | 84.9 ms: 1.08x faster                                                         |
| tornado_http               | 105 ms                                                          | 97.8 ms: 1.07x faster                                                         |
| json_dumps                 | 7.40 ms                                                         | 6.90 ms: 1.07x faster                                                         |
| regex_effbot               | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                         |
| docutils                   | 1.98 sec                                                        | 1.85 sec: 1.07x faster                                                        |
| fannkuch                   | 354 ms                                                          | 330 ms: 1.07x faster                                                          |
| 2to3                       | 280 ms                                                          | 262 ms: 1.07x faster                                                          |
| async_generators           | 313 ms                                                          | 294 ms: 1.07x faster                                                          |
| richards_super             | 46.5 ms                                                         | 43.7 ms: 1.06x faster                                                         |
| asyncio_tcp                | 662 ms                                                          | 624 ms: 1.06x faster                                                          |
| meteor_contest             | 86.9 ms                                                         | 82.1 ms: 1.06x faster                                                         |
| richards                   | 41.3 ms                                                         | 39.1 ms: 1.06x faster                                                         |
| sqlglot_optimize           | 48.5 ms                                                         | 46.0 ms: 1.05x faster                                                         |
| hexiom                     | 6.82 ms                                                         | 6.47 ms: 1.05x faster                                                         |
| sqlite_synth               | 2.07 us                                                         | 1.97 us: 1.05x faster                                                         |
| xml_etree_parse            | 113 ms                                                          | 108 ms: 1.05x faster                                                          |
| bench_thread_pool          | 1.10 ms                                                         | 1.05 ms: 1.05x faster                                                         |
| gc_traversal               | 1.44 ms                                                         | 1.38 ms: 1.04x faster                                                         |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.9 sec: 1.04x faster                                                        |
| sympy_expand               | 398 ms                                                          | 384 ms: 1.04x faster                                                          |
| pickle_list                | 3.37 us                                                         | 3.25 us: 1.04x faster                                                         |
| unpickle_list              | 2.95 us                                                         | 2.85 us: 1.03x faster                                                         |
| nqueens                    | 93.7 ms                                                         | 91.3 ms: 1.03x faster                                                         |
| pprint_pformat             | 1.50 sec                                                        | 1.46 sec: 1.02x faster                                                        |
| json_loads                 | 20.4 us                                                         | 20.1 us: 1.01x faster                                                         |
| scimark_monte_carlo        | 66.4 ms                                                         | 65.5 ms: 1.01x faster                                                         |
| bench_mp_pool              | 75.4 ms                                                         | 74.8 ms: 1.01x faster                                                         |
| pickle_dict                | 19.9 us                                                         | 19.8 us: 1.00x faster                                                         |
| pickle                     | 7.79 us                                                         | 7.92 us: 1.02x slower                                                         |
| json                       | 4.15 ms                                                         | 4.28 ms: 1.03x slower                                                         |
| unpickle                   | 9.71 us                                                         | 10.0 us: 1.03x slower                                                         |
| unpack_sequence            | 62.5 ns                                                         | 64.6 ns: 1.03x slower                                                         |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                         |
| telco                      | 5.51 ms                                                         | 6.46 ms: 1.17x slower                                                         |
| python_startup             | 22.4 ms                                                         | 26.3 ms: 1.18x slower                                                         |
| python_startup_no_site     | 19.1 ms                                                         | 23.8 ms: 1.25x slower                                                         |
| sqlglot_normalize          | 100 ms                                                          | 227 ms: 2.26x slower                                                          |
| coverage                   | 48.4 ms                                                         | 478 ms: 9.86x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.08x faster                                                                  |

Benchmark hidden because not significant (3): pidigits, pprint_safe_repr, create_gc_cycles
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown