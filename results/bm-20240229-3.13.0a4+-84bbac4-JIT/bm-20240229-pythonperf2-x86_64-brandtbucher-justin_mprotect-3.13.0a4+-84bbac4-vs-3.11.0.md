# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.03x faster \*
- HPT reliability: 85.79%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 305 ms: 1.06x slower                                                          |
| chameleon      | 7.92 ms                                                      | 7.52 ms: 1.05x faster                                                         |
| docutils       | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 435 ms: 1.19x faster                                                          |
| async_tree_memoization     | 629 ms                                                       | 549 ms: 1.15x faster                                                          |
| async_tree_none_tg         | 474 ms                                                       | 434 ms: 1.09x faster                                                          |
| async_tree_memoization_tg  | 600 ms                                                       | 554 ms: 1.08x faster                                                          |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 701 ms: 1.07x faster                                                          |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                                          |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 261 ms: 1.04x slower                                                          |
| float          | 74.9 ms                                                      | 78.5 ms: 1.05x slower                                                         |
| nbody          | 92.9 ms                                                      | 98.0 ms: 1.05x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 147 ms: 1.06x faster                                                          |
| regex_v8       | 24.4 ms                                                      | 26.0 ms: 1.07x slower                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.63 ms: 1.09x slower                                                         |
| regex_dna      | 227 ms                                                       | 248 ms: 1.09x slower                                                          |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                         |
| json_loads           | 28.9 us                                                      | 25.2 us: 1.15x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 145 ms: 1.07x faster                                                          |
| pickle_dict          | 32.3 us                                                      | 30.6 us: 1.06x faster                                                         |
| xml_etree_iterparse  | 107 ms                                                       | 102 ms: 1.04x faster                                                          |
| tomli_loads          | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 234 us: 1.02x faster                                                          |
| pickle_pure_python   | 316 us                                                       | 319 us: 1.01x slower                                                          |
| pickle               | 9.89 us                                                      | 10.1 us: 1.03x slower                                                         |
| xml_etree_process    | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                                         |
| xml_etree_generate   | 79.7 ms                                                      | 84.4 ms: 1.06x slower                                                         |
| pickle_list          | 3.94 us                                                      | 4.43 us: 1.12x slower                                                         |
| unpickle             | 13.3 us                                                      | 14.9 us: 1.13x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                                  |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 14.8 ms: 1.38x slower                                                         |
| python_startup_no_site | 7.73 ms                                                      | 13.3 ms: 1.72x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.54x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 9.96 ms: 1.11x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 119 us: 4.47x faster                                                          |
| asyncio_tcp                | 747 ms                                                       | 371 ms: 2.01x faster                                                          |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.94x faster                                                        |
| generators                 | 54.6 ms                                                      | 33.8 ms: 1.62x faster                                                         |
| comprehensions             | 25.1 us                                                      | 19.0 us: 1.32x faster                                                         |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                         |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                         |
| async_tree_none            | 518 ms                                                       | 435 ms: 1.19x faster                                                          |
| sympy_sum                  | 186 ms                                                       | 160 ms: 1.16x faster                                                          |
| json_loads                 | 28.9 us                                                      | 25.2 us: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 549 ms: 1.15x faster                                                          |
| logging_simple             | 7.24 us                                                      | 6.47 us: 1.12x faster                                                         |
| richards_super             | 63.6 ms                                                      | 57.3 ms: 1.11x faster                                                         |
| sympy_str                  | 337 ms                                                       | 305 ms: 1.11x faster                                                          |
| gc_traversal               | 4.15 ms                                                      | 3.75 ms: 1.11x faster                                                         |
| chaos                      | 74.9 ms                                                      | 67.8 ms: 1.11x faster                                                         |
| mako                       | 11.0 ms                                                      | 9.96 ms: 1.11x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 434 ms: 1.09x faster                                                          |
| async_tree_memoization_tg  | 600 ms                                                       | 554 ms: 1.08x faster                                                          |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.08x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.57 sec: 1.08x faster                                                        |
| sympy_expand               | 553 ms                                                       | 515 ms: 1.07x faster                                                          |
| logging_format             | 7.71 us                                                      | 7.18 us: 1.07x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 701 ms: 1.07x faster                                                          |
| fannkuch                   | 416 ms                                                       | 387 ms: 1.07x faster                                                          |
| crypto_pyaes               | 83.3 ms                                                      | 77.8 ms: 1.07x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 145 ms: 1.07x faster                                                          |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.42 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                                          |
| regex_compile              | 156 ms                                                       | 147 ms: 1.06x faster                                                          |
| pickle_dict                | 32.3 us                                                      | 30.6 us: 1.06x faster                                                         |
| chameleon                  | 7.92 ms                                                      | 7.52 ms: 1.05x faster                                                         |
| deltablue                  | 3.97 ms                                                      | 3.77 ms: 1.05x faster                                                         |
| json                       | 5.58 ms                                                      | 5.31 ms: 1.05x faster                                                         |
| sympy_integrate            | 25.8 ms                                                      | 24.6 ms: 1.05x faster                                                         |
| deepcopy                   | 391 us                                                       | 374 us: 1.04x faster                                                          |
| xml_etree_iterparse        | 107 ms                                                       | 102 ms: 1.04x faster                                                          |
| tomli_loads                | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.86 ms: 1.03x faster                                                         |
| logging_silent             | 100 ns                                                       | 97.7 ns: 1.03x faster                                                         |
| spectral_norm              | 95.1 ms                                                      | 92.7 ms: 1.03x faster                                                         |
| raytrace                   | 309 ms                                                       | 303 ms: 1.02x faster                                                          |
| unpickle_pure_python       | 238 us                                                       | 234 us: 1.02x faster                                                          |
| sqlglot_normalize          | 122 ms                                                       | 120 ms: 1.02x faster                                                          |
| create_gc_cycles           | 1.58 ms                                                      | 1.56 ms: 1.01x faster                                                         |
| asyncio_websockets         | 390 ms                                                       | 387 ms: 1.01x faster                                                          |
| meteor_contest             | 131 ms                                                       | 131 ms: 1.01x slower                                                          |
| pickle_pure_python         | 316 us                                                       | 319 us: 1.01x slower                                                          |
| richards                   | 49.7 ms                                                      | 50.4 ms: 1.01x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.70 sec: 1.02x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 68.8 ms: 1.02x slower                                                         |
| pickle                     | 9.89 us                                                      | 10.1 us: 1.03x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 827 ms: 1.03x slower                                                          |
| docutils                   | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                                        |
| pidigits                   | 251 ms                                                       | 261 ms: 1.04x slower                                                          |
| xml_etree_process          | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                                         |
| float                      | 74.9 ms                                                      | 78.5 ms: 1.05x slower                                                         |
| nbody                      | 92.9 ms                                                      | 98.0 ms: 1.05x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 84.4 ms: 1.06x slower                                                         |
| 2to3                       | 287 ms                                                       | 305 ms: 1.06x slower                                                          |
| scimark_lu                 | 114 ms                                                       | 121 ms: 1.06x slower                                                          |
| hexiom                     | 6.98 ms                                                      | 7.43 ms: 1.06x slower                                                         |
| regex_v8                   | 24.4 ms                                                      | 26.0 ms: 1.07x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.69 us: 1.07x slower                                                         |
| sqlglot_optimize           | 59.0 ms                                                      | 63.4 ms: 1.08x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.63 ms: 1.09x slower                                                         |
| go                         | 158 ms                                                       | 171 ms: 1.09x slower                                                          |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.42 ms: 1.09x slower                                                         |
| regex_dna                  | 227 ms                                                       | 248 ms: 1.09x slower                                                          |
| pickle_list                | 3.94 us                                                      | 4.43 us: 1.12x slower                                                         |
| unpickle                   | 13.3 us                                                      | 14.9 us: 1.13x slower                                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 80.0 ms: 1.15x slower                                                         |
| pyflate                    | 449 ms                                                       | 517 ms: 1.15x slower                                                          |
| scimark_fft                | 281 ms                                                       | 324 ms: 1.16x slower                                                          |
| telco                      | 6.81 ms                                                      | 8.04 ms: 1.18x slower                                                         |
| async_generators           | 322 ms                                                       | 381 ms: 1.18x slower                                                          |
| mypy2                      | 762 ms                                                       | 916 ms: 1.20x slower                                                          |
| coverage                   | 66.1 ms                                                      | 80.4 ms: 1.22x slower                                                         |
| unpack_sequence            | 45.7 ns                                                      | 61.4 ns: 1.34x slower                                                         |
| python_startup             | 10.7 ms                                                      | 14.8 ms: 1.38x slower                                                         |
| scimark_sor                | 110 ms                                                       | 153 ms: 1.39x slower                                                          |
| dask                       | 410 ms                                                       | 591 ms: 1.44x slower                                                          |
| python_startup_no_site     | 7.73 ms                                                      | 13.3 ms: 1.72x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.03x faster                                                                  |

Benchmark hidden because not significant (8): bench_thread_pool, nqueens, deepcopy_reduce, unpickle_list, pycparser, tornado_http, deepcopy_memo, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 85.79% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.25x