
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_cold
- machine: windows-x86
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 251 ms: 1.13x faster                                                         |
| chameleon      | 8.08 ms                                                         | 5.97 ms: 1.35x faster                                                        |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                       |
| tornado_http   | 118 ms                                                          | 97.1 ms: 1.22x faster                                                        |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 262 ms: 1.31x faster                                                         |
| async_tree_memoization     | 408 ms                                                          | 328 ms: 1.25x faster                                                         |
| async_tree_none_tg         | 301 ms                                                          | 244 ms: 1.23x faster                                                         |
| async_tree_io_tg           | 746 ms                                                          | 611 ms: 1.22x faster                                                         |
| async_tree_memoization_tg  | 378 ms                                                          | 311 ms: 1.21x faster                                                         |
| async_tree_io              | 754 ms                                                          | 637 ms: 1.18x faster                                                         |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 524 ms: 1.13x faster                                                         |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 515 ms: 1.12x faster                                                         |
| Geometric mean             | (ref)                                                           | 1.20x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 56.2 ms: 1.35x faster                                                        |
| nbody          | 126 ms                                                          | 97.0 ms: 1.30x faster                                                        |
| pidigits       | 203 ms                                                          | 204 ms: 1.00x slower                                                         |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 106 ms: 1.39x faster                                                         |
| regex_dna      | 122 ms                                                          | 121 ms: 1.01x faster                                                         |
| regex_effbot   | 1.82 ms                                                         | 1.94 ms: 1.06x slower                                                        |
| regex_v8       | 15.2 ms                                                         | 16.6 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 151 us: 1.53x faster                                                         |
| pickle_pure_python   | 309 us                                                          | 210 us: 1.47x faster                                                         |
| json_dumps           | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                        |
| tomli_loads          | 2.31 sec                                                        | 1.67 sec: 1.39x faster                                                       |
| xml_etree_process    | 55.0 ms                                                         | 42.2 ms: 1.30x faster                                                        |
| xml_etree_generate   | 71.6 ms                                                         | 61.3 ms: 1.17x faster                                                        |
| xml_etree_iterparse  | 75.6 ms                                                         | 69.9 ms: 1.08x faster                                                        |
| unpickle_list        | 3.28 us                                                         | 3.04 us: 1.08x faster                                                        |
| xml_etree_parse      | 114 ms                                                          | 111 ms: 1.03x faster                                                         |
| json_loads           | 20.0 us                                                         | 19.6 us: 1.02x faster                                                        |
| pickle_dict          | 20.1 us                                                         | 19.8 us: 1.01x faster                                                        |
| pickle_list          | 3.27 us                                                         | 3.22 us: 1.01x faster                                                        |
| pickle               | 7.99 us                                                         | 8.28 us: 1.04x slower                                                        |
| unpickle             | 9.23 us                                                         | 10.3 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.1 ms: 1.05x slower                                                        |
| python_startup_no_site | 18.8 ms                                                         | 21.0 ms: 1.12x slower                                                        |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.97 ms: 1.29x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 97.9 us: 4.89x faster                                                        |
| generators                 | 52.2 ms                                                         | 22.7 ms: 2.30x faster                                                        |
| logging_silent             | 119 ns                                                          | 61.6 ns: 1.94x faster                                                        |
| richards_super             | 58.7 ms                                                         | 33.1 ms: 1.77x faster                                                        |
| deepcopy_memo              | 40.0 us                                                         | 23.2 us: 1.72x faster                                                        |
| scimark_lu                 | 102 ms                                                          | 60.6 ms: 1.69x faster                                                        |
| richards                   | 48.8 ms                                                         | 29.0 ms: 1.68x faster                                                        |
| unpack_sequence            | 65.2 ns                                                         | 39.7 ns: 1.64x faster                                                        |
| coroutines                 | 23.7 ms                                                         | 14.5 ms: 1.64x faster                                                        |
| sqlglot_parse              | 1.49 ms                                                         | 918 us: 1.62x faster                                                         |
| deltablue                  | 4.10 ms                                                         | 2.52 ms: 1.62x faster                                                        |
| scimark_sor                | 135 ms                                                          | 83.4 ms: 1.62x faster                                                        |
| spectral_norm              | 122 ms                                                          | 78.2 ms: 1.55x faster                                                        |
| unpickle_pure_python       | 231 us                                                          | 151 us: 1.53x faster                                                         |
| sqlglot_transpile          | 1.78 ms                                                         | 1.18 ms: 1.51x faster                                                        |
| pickle_pure_python         | 309 us                                                          | 210 us: 1.47x faster                                                         |
| raytrace                   | 327 ms                                                          | 227 ms: 1.44x faster                                                         |
| json_dumps                 | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                        |
| chaos                      | 84.4 ms                                                         | 59.5 ms: 1.42x faster                                                        |
| comprehensions             | 22.1 us                                                         | 15.7 us: 1.40x faster                                                        |
| regex_compile              | 148 ms                                                          | 106 ms: 1.39x faster                                                         |
| tomli_loads                | 2.31 sec                                                        | 1.67 sec: 1.39x faster                                                       |
| deepcopy                   | 381 us                                                          | 278 us: 1.37x faster                                                         |
| deepcopy_reduce            | 3.32 us                                                         | 2.45 us: 1.35x faster                                                        |
| float                      | 76.1 ms                                                         | 56.2 ms: 1.35x faster                                                        |
| chameleon                  | 8.08 ms                                                         | 5.97 ms: 1.35x faster                                                        |
| sympy_sum                  | 149 ms                                                          | 112 ms: 1.33x faster                                                         |
| logging_simple             | 10.8 us                                                         | 8.19 us: 1.32x faster                                                        |
| logging_format             | 11.5 us                                                         | 8.71 us: 1.31x faster                                                        |
| async_tree_none            | 343 ms                                                          | 262 ms: 1.31x faster                                                         |
| xml_etree_process          | 55.0 ms                                                         | 42.2 ms: 1.30x faster                                                        |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.26 ms: 1.30x faster                                                        |
| nbody                      | 126 ms                                                          | 97.0 ms: 1.30x faster                                                        |
| sympy_str                  | 283 ms                                                          | 219 ms: 1.29x faster                                                         |
| mako                       | 10.3 ms                                                         | 7.97 ms: 1.29x faster                                                        |
| nqueens                    | 111 ms                                                          | 87.1 ms: 1.28x faster                                                        |
| fannkuch                   | 399 ms                                                          | 313 ms: 1.28x faster                                                         |
| pycparser                  | 1.04 sec                                                        | 830 ms: 1.26x faster                                                         |
| crypto_pyaes               | 79.4 ms                                                         | 63.3 ms: 1.25x faster                                                        |
| sympy_expand               | 462 ms                                                          | 369 ms: 1.25x faster                                                         |
| async_tree_memoization     | 408 ms                                                          | 328 ms: 1.25x faster                                                         |
| sympy_integrate            | 19.9 ms                                                         | 16.1 ms: 1.24x faster                                                        |
| go                         | 147 ms                                                          | 119 ms: 1.23x faster                                                         |
| async_tree_none_tg         | 301 ms                                                          | 244 ms: 1.23x faster                                                         |
| pyflate                    | 471 ms                                                          | 383 ms: 1.23x faster                                                         |
| async_tree_io_tg           | 746 ms                                                          | 611 ms: 1.22x faster                                                         |
| sqlglot_optimize           | 51.8 ms                                                         | 42.5 ms: 1.22x faster                                                        |
| tornado_http               | 118 ms                                                          | 97.1 ms: 1.22x faster                                                        |
| async_tree_memoization_tg  | 378 ms                                                          | 311 ms: 1.21x faster                                                         |
| pprint_safe_repr           | 819 ms                                                          | 688 ms: 1.19x faster                                                         |
| asyncio_tcp                | 787 ms                                                          | 665 ms: 1.18x faster                                                         |
| async_tree_io              | 754 ms                                                          | 637 ms: 1.18x faster                                                         |
| pprint_pformat             | 1.70 sec                                                        | 1.43 sec: 1.18x faster                                                       |
| json                       | 4.78 ms                                                         | 4.07 ms: 1.18x faster                                                        |
| xml_etree_generate         | 71.6 ms                                                         | 61.3 ms: 1.17x faster                                                        |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                       |
| sqlite_synth               | 2.15 us                                                         | 1.87 us: 1.15x faster                                                        |
| scimark_fft                | 291 ms                                                          | 254 ms: 1.15x faster                                                         |
| dask                       | 355 ms                                                          | 310 ms: 1.15x faster                                                         |
| 2to3                       | 282 ms                                                          | 251 ms: 1.13x faster                                                         |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 524 ms: 1.13x faster                                                         |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 515 ms: 1.12x faster                                                         |
| hexiom                     | 7.51 ms                                                         | 6.72 ms: 1.12x faster                                                        |
| xml_etree_iterparse        | 75.6 ms                                                         | 69.9 ms: 1.08x faster                                                        |
| unpickle_list              | 3.28 us                                                         | 3.04 us: 1.08x faster                                                        |
| mdp                        | 2.07 sec                                                        | 1.93 sec: 1.07x faster                                                       |
| bench_thread_pool          | 1.14 ms                                                         | 1.09 ms: 1.04x faster                                                        |
| meteor_contest             | 90.9 ms                                                         | 87.5 ms: 1.04x faster                                                        |
| xml_etree_parse            | 114 ms                                                          | 111 ms: 1.03x faster                                                         |
| json_loads                 | 20.0 us                                                         | 19.6 us: 1.02x faster                                                        |
| scimark_monte_carlo        | 70.8 ms                                                         | 69.4 ms: 1.02x faster                                                        |
| pickle_dict                | 20.1 us                                                         | 19.8 us: 1.01x faster                                                        |
| pickle_list                | 3.27 us                                                         | 3.22 us: 1.01x faster                                                        |
| regex_dna                  | 122 ms                                                          | 121 ms: 1.01x faster                                                         |
| pidigits                   | 203 ms                                                          | 204 ms: 1.00x slower                                                         |
| gc_traversal               | 1.38 ms                                                         | 1.42 ms: 1.03x slower                                                        |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                       |
| pickle                     | 7.99 us                                                         | 8.28 us: 1.04x slower                                                        |
| python_startup             | 22.0 ms                                                         | 23.1 ms: 1.05x slower                                                        |
| regex_effbot               | 1.82 ms                                                         | 1.94 ms: 1.06x slower                                                        |
| bench_mp_pool              | 70.9 ms                                                         | 75.7 ms: 1.07x slower                                                        |
| create_gc_cycles           | 618 us                                                          | 660 us: 1.07x slower                                                         |
| regex_v8                   | 15.2 ms                                                         | 16.6 ms: 1.10x slower                                                        |
| pathlib                    | 79.9 ms                                                         | 88.8 ms: 1.11x slower                                                        |
| python_startup_no_site     | 18.8 ms                                                         | 21.0 ms: 1.12x slower                                                        |
| unpickle                   | 9.23 us                                                         | 10.3 us: 1.12x slower                                                        |
| async_generators           | 260 ms                                                          | 294 ms: 1.13x slower                                                         |
| telco                      | 5.29 ms                                                         | 6.11 ms: 1.15x slower                                                        |
| sqlglot_normalize          | 113 ms                                                          | 221 ms: 1.95x slower                                                         |
| coverage                   | 58.0 ms                                                         | 480 ms: 8.28x slower                                                         |
| Geometric mean             | (ref)                                                           | 1.20x faster                                                                 |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown