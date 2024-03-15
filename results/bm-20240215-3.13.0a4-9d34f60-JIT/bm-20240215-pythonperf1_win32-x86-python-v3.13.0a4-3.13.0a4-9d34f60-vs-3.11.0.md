# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a4
- machine: windows-x86
- commit hash: 9d34f60
- commit date: 2024-02-15
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 256 ms: 1.10x faster                                                |
| chameleon      | 8.08 ms                                                         | 6.01 ms: 1.34x faster                                               |
| docutils       | 2.10 sec                                                        | 1.82 sec: 1.15x faster                                              |
| tornado_http   | 118 ms                                                          | 99.9 ms: 1.19x faster                                               |
| Geometric mean | (ref)                                                           | 1.19x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 260 ms: 1.32x faster                                                |
| async_tree_memoization     | 408 ms                                                          | 325 ms: 1.26x faster                                                |
| async_tree_none_tg         | 301 ms                                                          | 246 ms: 1.22x faster                                                |
| async_tree_io_tg           | 746 ms                                                          | 612 ms: 1.22x faster                                                |
| async_tree_io              | 754 ms                                                          | 624 ms: 1.21x faster                                                |
| async_tree_memoization_tg  | 378 ms                                                          | 313 ms: 1.21x faster                                                |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 503 ms: 1.15x faster                                                |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 515 ms: 1.15x faster                                                |
| Geometric mean             | (ref)                                                           | 1.22x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 53.9 ms: 1.41x faster                                               |
| nbody          | 126 ms                                                          | 89.7 ms: 1.40x faster                                               |
| pidigits       | 203 ms                                                          | 202 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                           | 1.26x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 110 ms: 1.34x faster                                                |
| regex_dna      | 122 ms                                                          | 120 ms: 1.02x faster                                                |
| regex_effbot   | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                               |
| regex_v8       | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                               |
| Geometric mean | (ref)                                                           | 1.05x faster                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 156 us: 1.48x faster                                                |
| json_dumps           | 9.80 ms                                                         | 6.95 ms: 1.41x faster                                               |
| tomli_loads          | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                              |
| pickle_pure_python   | 309 us                                                          | 223 us: 1.38x faster                                                |
| xml_etree_process    | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                               |
| xml_etree_generate   | 71.6 ms                                                         | 60.2 ms: 1.19x faster                                               |
| xml_etree_iterparse  | 75.6 ms                                                         | 65.9 ms: 1.15x faster                                               |
| unpickle_list        | 3.28 us                                                         | 2.87 us: 1.14x faster                                               |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.04x faster                                                |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                               |
| json_loads           | 20.0 us                                                         | 20.3 us: 1.01x slower                                               |
| pickle               | 7.99 us                                                         | 8.11 us: 1.02x slower                                               |
| pickle_list          | 3.27 us                                                         | 3.35 us: 1.03x slower                                               |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.10x slower                                               |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.5 ms: 1.03x slower                                               |
| python_startup_no_site | 18.8 ms                                                         | 20.3 ms: 1.08x slower                                               |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.43 ms: 1.38x faster                                               |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 98.7 us: 4.84x faster                                               |
| generators                 | 52.2 ms                                                         | 24.6 ms: 2.12x faster                                               |
| logging_silent             | 119 ns                                                          | 67.1 ns: 1.78x faster                                               |
| spectral_norm              | 122 ms                                                          | 73.2 ms: 1.66x faster                                               |
| richards_super             | 58.7 ms                                                         | 36.5 ms: 1.61x faster                                               |
| coroutines                 | 23.7 ms                                                         | 14.9 ms: 1.59x faster                                               |
| deltablue                  | 4.10 ms                                                         | 2.58 ms: 1.59x faster                                               |
| deepcopy_memo              | 40.0 us                                                         | 25.3 us: 1.58x faster                                               |
| comprehensions             | 22.1 us                                                         | 14.1 us: 1.56x faster                                               |
| scimark_lu                 | 102 ms                                                          | 65.6 ms: 1.56x faster                                               |
| sqlglot_parse              | 1.49 ms                                                         | 961 us: 1.55x faster                                                |
| unpack_sequence            | 65.2 ns                                                         | 42.6 ns: 1.53x faster                                               |
| richards                   | 48.8 ms                                                         | 32.2 ms: 1.52x faster                                               |
| scimark_sor                | 135 ms                                                          | 89.6 ms: 1.51x faster                                               |
| unpickle_pure_python       | 231 us                                                          | 156 us: 1.48x faster                                                |
| sqlglot_transpile          | 1.78 ms                                                         | 1.21 ms: 1.47x faster                                               |
| float                      | 76.1 ms                                                         | 53.9 ms: 1.41x faster                                               |
| json_dumps                 | 9.80 ms                                                         | 6.95 ms: 1.41x faster                                               |
| nbody                      | 126 ms                                                          | 89.7 ms: 1.40x faster                                               |
| tomli_loads                | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                              |
| pickle_pure_python         | 309 us                                                          | 223 us: 1.38x faster                                                |
| chaos                      | 84.4 ms                                                         | 61.0 ms: 1.38x faster                                               |
| mako                       | 10.3 ms                                                         | 7.43 ms: 1.38x faster                                               |
| raytrace                   | 327 ms                                                          | 240 ms: 1.36x faster                                                |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.12 ms: 1.36x faster                                               |
| sympy_sum                  | 149 ms                                                          | 110 ms: 1.35x faster                                                |
| chameleon                  | 8.08 ms                                                         | 6.01 ms: 1.34x faster                                               |
| regex_compile              | 148 ms                                                          | 110 ms: 1.34x faster                                                |
| deepcopy                   | 381 us                                                          | 285 us: 1.34x faster                                                |
| deepcopy_reduce            | 3.32 us                                                         | 2.51 us: 1.32x faster                                               |
| async_tree_none            | 343 ms                                                          | 260 ms: 1.32x faster                                                |
| crypto_pyaes               | 79.4 ms                                                         | 61.0 ms: 1.30x faster                                               |
| sympy_str                  | 283 ms                                                          | 218 ms: 1.30x faster                                                |
| logging_simple             | 10.8 us                                                         | 8.35 us: 1.29x faster                                               |
| xml_etree_process          | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                               |
| logging_format             | 11.5 us                                                         | 8.97 us: 1.28x faster                                               |
| pyflate                    | 471 ms                                                          | 370 ms: 1.27x faster                                                |
| async_tree_memoization     | 408 ms                                                          | 325 ms: 1.26x faster                                                |
| nqueens                    | 111 ms                                                          | 88.7 ms: 1.26x faster                                               |
| sympy_integrate            | 19.9 ms                                                         | 16.0 ms: 1.25x faster                                               |
| asyncio_tcp                | 787 ms                                                          | 632 ms: 1.25x faster                                                |
| fannkuch                   | 399 ms                                                          | 322 ms: 1.24x faster                                                |
| async_tree_none_tg         | 301 ms                                                          | 246 ms: 1.22x faster                                                |
| async_tree_io_tg           | 746 ms                                                          | 612 ms: 1.22x faster                                                |
| scimark_fft                | 291 ms                                                          | 239 ms: 1.22x faster                                                |
| sympy_expand               | 462 ms                                                          | 379 ms: 1.22x faster                                                |
| async_tree_io              | 754 ms                                                          | 624 ms: 1.21x faster                                                |
| async_tree_memoization_tg  | 378 ms                                                          | 313 ms: 1.21x faster                                                |
| go                         | 147 ms                                                          | 123 ms: 1.20x faster                                                |
| xml_etree_generate         | 71.6 ms                                                         | 60.2 ms: 1.19x faster                                               |
| sqlglot_optimize           | 51.8 ms                                                         | 43.7 ms: 1.19x faster                                               |
| tornado_http               | 118 ms                                                          | 99.9 ms: 1.19x faster                                               |
| pycparser                  | 1.04 sec                                                        | 891 ms: 1.17x faster                                                |
| sqlite_synth               | 2.15 us                                                         | 1.85 us: 1.16x faster                                               |
| docutils                   | 2.10 sec                                                        | 1.82 sec: 1.15x faster                                              |
| pprint_pformat             | 1.70 sec                                                        | 1.47 sec: 1.15x faster                                              |
| pprint_safe_repr           | 819 ms                                                          | 713 ms: 1.15x faster                                                |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 503 ms: 1.15x faster                                                |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 515 ms: 1.15x faster                                                |
| xml_etree_iterparse        | 75.6 ms                                                         | 65.9 ms: 1.15x faster                                               |
| unpickle_list              | 3.28 us                                                         | 2.87 us: 1.14x faster                                               |
| hexiom                     | 7.51 ms                                                         | 6.61 ms: 1.14x faster                                               |
| mdp                        | 2.07 sec                                                        | 1.85 sec: 1.12x faster                                              |
| json                       | 4.78 ms                                                         | 4.27 ms: 1.12x faster                                               |
| bench_thread_pool          | 1.14 ms                                                         | 1.02 ms: 1.11x faster                                               |
| 2to3                       | 282 ms                                                          | 256 ms: 1.10x faster                                                |
| meteor_contest             | 90.9 ms                                                         | 83.8 ms: 1.08x faster                                               |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.04x faster                                                |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.7 sec: 1.02x faster                                              |
| regex_dna                  | 122 ms                                                          | 120 ms: 1.02x faster                                                |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                               |
| pidigits                   | 203 ms                                                          | 202 ms: 1.01x faster                                                |
| bench_mp_pool              | 70.9 ms                                                         | 71.5 ms: 1.01x slower                                               |
| scimark_monte_carlo        | 70.8 ms                                                         | 71.6 ms: 1.01x slower                                               |
| json_loads                 | 20.0 us                                                         | 20.3 us: 1.01x slower                                               |
| pickle                     | 7.99 us                                                         | 8.11 us: 1.02x slower                                               |
| python_startup             | 22.0 ms                                                         | 22.5 ms: 1.03x slower                                               |
| pickle_list                | 3.27 us                                                         | 3.35 us: 1.03x slower                                               |
| gc_traversal               | 1.38 ms                                                         | 1.42 ms: 1.03x slower                                               |
| create_gc_cycles           | 618 us                                                          | 646 us: 1.05x slower                                                |
| regex_effbot               | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                               |
| pathlib                    | 79.9 ms                                                         | 84.3 ms: 1.05x slower                                               |
| regex_v8                   | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                               |
| python_startup_no_site     | 18.8 ms                                                         | 20.3 ms: 1.08x slower                                               |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.10x slower                                               |
| async_generators           | 260 ms                                                          | 300 ms: 1.15x slower                                                |
| dask                       | 355 ms                                                          | 432 ms: 1.22x slower                                                |
| telco                      | 5.29 ms                                                         | 6.55 ms: 1.24x slower                                               |
| sqlglot_normalize          | 113 ms                                                          | 224 ms: 1.98x slower                                                |
| coverage                   | 58.0 ms                                                         | 464 ms: 8.01x slower                                                |
| Geometric mean             | (ref)                                                           | 1.19x faster                                                        |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown