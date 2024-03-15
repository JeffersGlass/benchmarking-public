
# Results vs. 3.12.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: windows-x86
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 246 ms: 1.14x faster                                                            |
| chameleon      | 7.75 ms                                                         | 6.02 ms: 1.29x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.78 sec: 1.11x faster                                                          |
| tornado_http   | 105 ms                                                          | 95.7 ms: 1.10x faster                                                           |
| Geometric mean | (ref)                                                           | 1.16x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 298 ms: 1.18x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 237 ms: 1.17x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 311 ms: 1.17x faster                                                            |
| async_tree_io              | 693 ms                                                          | 597 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 585 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 510 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 501 ms: 1.09x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 53.8 ms: 1.42x faster                                                           |
| nbody          | 127 ms                                                          | 90.6 ms: 1.40x faster                                                           |
| pidigits       | 199 ms                                                          | 203 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 105 ms: 1.23x faster                                                            |
| regex_dna      | 127 ms                                                          | 117 ms: 1.09x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.08x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 150 us: 1.40x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 205 us: 1.40x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.59 sec: 1.38x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 41.4 ms: 1.29x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 65.5 ms: 1.19x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.71 ms: 1.10x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 104 ms: 1.09x faster                                                            |
| json_loads           | 20.4 us                                                         | 20.0 us: 1.02x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| pickle               | 7.79 us                                                         | 8.13 us: 1.04x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.2 us: 1.05x slower                                                           |
| unpickle_list        | 2.95 us                                                         | 3.10 us: 1.05x slower                                                           |
| pickle_list          | 3.37 us                                                         | 3.66 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.12x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 19.1 ms                                                         | 20.1 ms: 1.06x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.64 ms: 1.30x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.4 ms: 1.72x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 22.7 us: 1.69x faster                                                           |
| logging_silent             | 101 ns                                                          | 60.5 ns: 1.67x faster                                                           |
| scimark_sor                | 130 ms                                                          | 79.9 ms: 1.62x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 60.1 ms: 1.55x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 41.2 ns: 1.52x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.38 ms: 1.51x faster                                                           |
| richards                   | 41.3 ms                                                         | 28.4 ms: 1.45x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.4 ms: 1.45x faster                                                           |
| richards_super             | 46.5 ms                                                         | 32.3 ms: 1.44x faster                                                           |
| float                      | 76.7 ms                                                         | 53.8 ms: 1.42x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 150 us: 1.40x faster                                                            |
| nbody                      | 127 ms                                                          | 90.6 ms: 1.40x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 205 us: 1.40x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.59 sec: 1.38x faster                                                          |
| deepcopy_reduce            | 3.23 us                                                         | 2.37 us: 1.36x faster                                                           |
| raytrace                   | 308 ms                                                          | 228 ms: 1.35x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 93.8 us: 1.35x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 932 us: 1.34x faster                                                            |
| spectral_norm              | 104 ms                                                          | 78.4 ms: 1.32x faster                                                           |
| comprehensions             | 19.2 us                                                         | 14.7 us: 1.31x faster                                                           |
| deepcopy                   | 360 us                                                          | 276 us: 1.31x faster                                                            |
| mako                       | 9.96 ms                                                         | 7.64 ms: 1.30x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.18 ms: 1.30x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 41.4 ms: 1.29x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 6.02 ms: 1.29x faster                                                           |
| regex_compile              | 129 ms                                                          | 105 ms: 1.23x faster                                                            |
| logging_simple             | 9.75 us                                                         | 7.97 us: 1.22x faster                                                           |
| logging_format             | 10.4 us                                                         | 8.57 us: 1.21x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.19 ms: 1.21x faster                                                           |
| fannkuch                   | 354 ms                                                          | 293 ms: 1.21x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 65.5 ms: 1.19x faster                                                           |
| go                         | 137 ms                                                          | 116 ms: 1.18x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 298 ms: 1.18x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 237 ms: 1.17x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 311 ms: 1.17x faster                                                            |
| async_tree_io              | 693 ms                                                          | 597 ms: 1.16x faster                                                            |
| pycparser                  | 978 ms                                                          | 843 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 585 ms: 1.16x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 60.4 ms: 1.15x faster                                                           |
| 2to3                       | 280 ms                                                          | 246 ms: 1.14x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 42.8 ms: 1.13x faster                                                           |
| async_generators           | 313 ms                                                          | 277 ms: 1.13x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.84 us: 1.13x faster                                                           |
| chaos                      | 69.4 ms                                                         | 61.8 ms: 1.12x faster                                                           |
| sympy_integrate            | 17.5 ms                                                         | 15.6 ms: 1.12x faster                                                           |
| sympy_str                  | 240 ms                                                          | 214 ms: 1.12x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 110 ms: 1.11x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.78 sec: 1.11x faster                                                          |
| pyflate                    | 424 ms                                                          | 383 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 510 ms: 1.11x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.71 ms: 1.10x faster                                                           |
| tornado_http               | 105 ms                                                          | 95.7 ms: 1.10x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 501 ms: 1.09x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 83.9 ms: 1.09x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 104 ms: 1.09x faster                                                            |
| nqueens                    | 93.7 ms                                                         | 86.1 ms: 1.09x faster                                                           |
| asyncio_tcp                | 662 ms                                                          | 609 ms: 1.09x faster                                                            |
| regex_dna                  | 127 ms                                                          | 117 ms: 1.09x faster                                                            |
| dask                       | 323 ms                                                          | 298 ms: 1.08x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.02 ms: 1.08x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 6.30 ms: 1.08x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.39 sec: 1.08x faster                                                          |
| scimark_fft                | 271 ms                                                          | 251 ms: 1.08x faster                                                            |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| sympy_expand               | 398 ms                                                          | 372 ms: 1.07x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 674 ms: 1.07x faster                                                            |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                          |
| meteor_contest             | 86.9 ms                                                         | 82.6 ms: 1.05x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 72.0 ms: 1.05x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.38 ms: 1.04x faster                                                           |
| create_gc_cycles           | 652 us                                                          | 640 us: 1.02x faster                                                            |
| json                       | 4.15 ms                                                         | 4.08 ms: 1.02x faster                                                           |
| json_loads                 | 20.4 us                                                         | 20.0 us: 1.02x faster                                                           |
| mdp                        | 1.91 sec                                                        | 1.89 sec: 1.01x faster                                                          |
| pickle_dict                | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 203 ms: 1.02x slower                                                            |
| scimark_monte_carlo        | 66.4 ms                                                         | 68.8 ms: 1.04x slower                                                           |
| pickle                     | 7.79 us                                                         | 8.13 us: 1.04x slower                                                           |
| unpickle                   | 9.71 us                                                         | 10.2 us: 1.05x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 3.10 us: 1.05x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.1 ms: 1.06x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                           |
| pickle_list                | 3.37 us                                                         | 3.66 us: 1.09x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.11 ms: 1.11x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 219 ms: 2.19x slower                                                            |
| coverage                   | 48.4 ms                                                         | 465 ms: 9.59x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (1): python_startup
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown