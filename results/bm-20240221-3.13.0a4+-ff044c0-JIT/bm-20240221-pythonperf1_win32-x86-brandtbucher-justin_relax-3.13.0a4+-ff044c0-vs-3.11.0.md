
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: windows-x86
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.17x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 262 ms: 1.08x faster                                                          |
| chameleon      | 8.08 ms                                                         | 5.99 ms: 1.35x faster                                                         |
| docutils       | 2.10 sec                                                        | 1.85 sec: 1.13x faster                                                        |
| tornado_http   | 118 ms                                                          | 97.8 ms: 1.21x faster                                                         |
| Geometric mean | (ref)                                                           | 1.19x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 259 ms: 1.33x faster                                                          |
| async_tree_memoization     | 408 ms                                                          | 323 ms: 1.26x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 604 ms: 1.24x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 244 ms: 1.23x faster                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 307 ms: 1.23x faster                                                          |
| async_tree_io              | 754 ms                                                          | 621 ms: 1.21x faster                                                          |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 497 ms: 1.16x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.16x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 55.1 ms: 1.38x faster                                                         |
| nbody          | 126 ms                                                          | 94.5 ms: 1.33x faster                                                         |
| pidigits       | 203 ms                                                          | 199 ms: 1.02x faster                                                          |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 117 ms: 1.27x faster                                                          |
| regex_dna      | 122 ms                                                          | 118 ms: 1.03x faster                                                          |
| regex_effbot   | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                         |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 6.90 ms: 1.42x faster                                                         |
| pickle_pure_python   | 309 us                                                          | 228 us: 1.35x faster                                                          |
| tomli_loads          | 2.31 sec                                                        | 1.71 sec: 1.35x faster                                                        |
| xml_etree_process    | 55.0 ms                                                         | 42.7 ms: 1.29x faster                                                         |
| unpickle_pure_python | 231 us                                                          | 181 us: 1.27x faster                                                          |
| xml_etree_generate   | 71.6 ms                                                         | 60.5 ms: 1.19x faster                                                         |
| unpickle_list        | 3.28 us                                                         | 2.85 us: 1.15x faster                                                         |
| xml_etree_iterparse  | 75.6 ms                                                         | 67.0 ms: 1.13x faster                                                         |
| xml_etree_parse      | 114 ms                                                          | 108 ms: 1.06x faster                                                          |
| pickle_dict          | 20.1 us                                                         | 19.8 us: 1.01x faster                                                         |
| pickle_list          | 3.27 us                                                         | 3.25 us: 1.00x faster                                                         |
| unpickle             | 9.23 us                                                         | 10.0 us: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.14x faster                                                                  |

Benchmark hidden because not significant (2): pickle, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 26.3 ms: 1.20x slower                                                         |
| python_startup_no_site | 18.8 ms                                                         | 23.8 ms: 1.26x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.23x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.25 ms: 1.42x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 99.3 us: 4.82x faster                                                         |
| generators                 | 52.2 ms                                                         | 24.6 ms: 2.13x faster                                                         |
| logging_silent             | 119 ns                                                          | 69.0 ns: 1.73x faster                                                         |
| spectral_norm              | 122 ms                                                          | 70.7 ms: 1.72x faster                                                         |
| coroutines                 | 23.7 ms                                                         | 15.3 ms: 1.55x faster                                                         |
| comprehensions             | 22.1 us                                                         | 14.7 us: 1.50x faster                                                         |
| deltablue                  | 4.10 ms                                                         | 2.74 ms: 1.49x faster                                                         |
| sqlglot_parse              | 1.49 ms                                                         | 1.01 ms: 1.48x faster                                                         |
| chaos                      | 84.4 ms                                                         | 57.3 ms: 1.47x faster                                                         |
| deepcopy_memo              | 40.0 us                                                         | 27.4 us: 1.46x faster                                                         |
| json_dumps                 | 9.80 ms                                                         | 6.90 ms: 1.42x faster                                                         |
| mako                       | 10.3 ms                                                         | 7.25 ms: 1.42x faster                                                         |
| sqlglot_transpile          | 1.78 ms                                                         | 1.28 ms: 1.40x faster                                                         |
| float                      | 76.1 ms                                                         | 55.1 ms: 1.38x faster                                                         |
| sympy_sum                  | 149 ms                                                          | 109 ms: 1.36x faster                                                          |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.11 ms: 1.36x faster                                                         |
| pickle_pure_python         | 309 us                                                          | 228 us: 1.35x faster                                                          |
| tomli_loads                | 2.31 sec                                                        | 1.71 sec: 1.35x faster                                                        |
| chameleon                  | 8.08 ms                                                         | 5.99 ms: 1.35x faster                                                         |
| richards_super             | 58.7 ms                                                         | 43.7 ms: 1.34x faster                                                         |
| nbody                      | 126 ms                                                          | 94.5 ms: 1.33x faster                                                         |
| async_tree_none            | 343 ms                                                          | 259 ms: 1.33x faster                                                          |
| crypto_pyaes               | 79.4 ms                                                         | 60.8 ms: 1.31x faster                                                         |
| sympy_str                  | 283 ms                                                          | 218 ms: 1.30x faster                                                          |
| xml_etree_process          | 55.0 ms                                                         | 42.7 ms: 1.29x faster                                                         |
| deepcopy_reduce            | 3.32 us                                                         | 2.59 us: 1.28x faster                                                         |
| deepcopy                   | 381 us                                                          | 298 us: 1.28x faster                                                          |
| unpickle_pure_python       | 231 us                                                          | 181 us: 1.27x faster                                                          |
| logging_simple             | 10.8 us                                                         | 8.50 us: 1.27x faster                                                         |
| regex_compile              | 148 ms                                                          | 117 ms: 1.27x faster                                                          |
| scimark_sor                | 135 ms                                                          | 107 ms: 1.27x faster                                                          |
| async_tree_memoization     | 408 ms                                                          | 323 ms: 1.26x faster                                                          |
| logging_format             | 11.5 us                                                         | 9.08 us: 1.26x faster                                                         |
| asyncio_tcp                | 787 ms                                                          | 624 ms: 1.26x faster                                                          |
| richards                   | 48.8 ms                                                         | 39.1 ms: 1.25x faster                                                         |
| raytrace                   | 327 ms                                                          | 263 ms: 1.25x faster                                                          |
| sympy_integrate            | 19.9 ms                                                         | 16.0 ms: 1.24x faster                                                         |
| async_tree_io_tg           | 746 ms                                                          | 604 ms: 1.24x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 244 ms: 1.23x faster                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 307 ms: 1.23x faster                                                          |
| scimark_fft                | 291 ms                                                          | 237 ms: 1.23x faster                                                          |
| pyflate                    | 471 ms                                                          | 384 ms: 1.23x faster                                                          |
| nqueens                    | 111 ms                                                          | 91.3 ms: 1.22x faster                                                         |
| async_tree_io              | 754 ms                                                          | 621 ms: 1.21x faster                                                          |
| tornado_http               | 118 ms                                                          | 97.8 ms: 1.21x faster                                                         |
| fannkuch                   | 399 ms                                                          | 330 ms: 1.21x faster                                                          |
| sympy_expand               | 462 ms                                                          | 384 ms: 1.20x faster                                                          |
| pycparser                  | 1.04 sec                                                        | 869 ms: 1.20x faster                                                          |
| scimark_lu                 | 102 ms                                                          | 85.7 ms: 1.19x faster                                                         |
| go                         | 147 ms                                                          | 123 ms: 1.19x faster                                                          |
| mdp                        | 2.07 sec                                                        | 1.74 sec: 1.19x faster                                                        |
| xml_etree_generate         | 71.6 ms                                                         | 60.5 ms: 1.19x faster                                                         |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 497 ms: 1.16x faster                                                          |
| hexiom                     | 7.51 ms                                                         | 6.47 ms: 1.16x faster                                                         |
| pprint_pformat             | 1.70 sec                                                        | 1.46 sec: 1.16x faster                                                        |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.16x faster                                                          |
| unpickle_list              | 3.28 us                                                         | 2.85 us: 1.15x faster                                                         |
| pprint_safe_repr           | 819 ms                                                          | 719 ms: 1.14x faster                                                          |
| docutils                   | 2.10 sec                                                        | 1.85 sec: 1.13x faster                                                        |
| sqlglot_optimize           | 51.8 ms                                                         | 46.0 ms: 1.13x faster                                                         |
| xml_etree_iterparse        | 75.6 ms                                                         | 67.0 ms: 1.13x faster                                                         |
| json                       | 4.78 ms                                                         | 4.28 ms: 1.12x faster                                                         |
| meteor_contest             | 90.9 ms                                                         | 82.1 ms: 1.11x faster                                                         |
| sqlite_synth               | 2.15 us                                                         | 1.97 us: 1.09x faster                                                         |
| scimark_monte_carlo        | 70.8 ms                                                         | 65.5 ms: 1.08x faster                                                         |
| 2to3                       | 282 ms                                                          | 262 ms: 1.08x faster                                                          |
| bench_thread_pool          | 1.14 ms                                                         | 1.05 ms: 1.08x faster                                                         |
| xml_etree_parse            | 114 ms                                                          | 108 ms: 1.06x faster                                                          |
| regex_dna                  | 122 ms                                                          | 118 ms: 1.03x faster                                                          |
| pidigits                   | 203 ms                                                          | 199 ms: 1.02x faster                                                          |
| pickle_dict                | 20.1 us                                                         | 19.8 us: 1.01x faster                                                         |
| unpack_sequence            | 65.2 ns                                                         | 64.6 ns: 1.01x faster                                                         |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.9 sec: 1.01x faster                                                        |
| pickle_list                | 3.27 us                                                         | 3.25 us: 1.00x faster                                                         |
| regex_effbot               | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                         |
| bench_mp_pool              | 70.9 ms                                                         | 74.8 ms: 1.05x slower                                                         |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                         |
| pathlib                    | 79.9 ms                                                         | 84.9 ms: 1.06x slower                                                         |
| create_gc_cycles           | 618 us                                                          | 656 us: 1.06x slower                                                          |
| unpickle                   | 9.23 us                                                         | 10.0 us: 1.09x slower                                                         |
| async_generators           | 260 ms                                                          | 294 ms: 1.13x slower                                                          |
| python_startup             | 22.0 ms                                                         | 26.3 ms: 1.20x slower                                                         |
| telco                      | 5.29 ms                                                         | 6.46 ms: 1.22x slower                                                         |
| python_startup_no_site     | 18.8 ms                                                         | 23.8 ms: 1.26x slower                                                         |
| sqlglot_normalize          | 113 ms                                                          | 227 ms: 2.01x slower                                                          |
| coverage                   | 58.0 ms                                                         | 478 ms: 8.23x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                  |

Benchmark hidden because not significant (3): pickle, json_loads, gc_traversal
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown