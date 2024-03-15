# Results vs. 3.11.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: windows-x86
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 255 ms: 1.11x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.77 ms: 1.40x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.82 sec: 1.15x faster                                                          |
| tornado_http   | 118 ms                                                          | 95.2 ms: 1.24x faster                                                           |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 257 ms: 1.33x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 318 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 302 ms: 1.25x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 597 ms: 1.25x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| async_tree_io              | 754 ms                                                          | 612 ms: 1.23x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 507 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 523 ms: 1.13x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 54.7 ms: 1.39x faster                                                           |
| nbody          | 126 ms                                                          | 93.7 ms: 1.34x faster                                                           |
| pidigits       | 203 ms                                                          | 201 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 111 ms: 1.33x faster                                                            |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                           |
| regex_dna      | 122 ms                                                          | 130 ms: 1.07x slower                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.97 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.02x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 309 us                                                          | 214 us: 1.44x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.80 ms: 1.44x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.66 sec: 1.39x faster                                                          |
| unpickle_pure_python | 231 us                                                          | 167 us: 1.39x faster                                                            |
| xml_etree_process    | 55.0 ms                                                         | 41.9 ms: 1.31x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.65 us: 1.23x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 66.6 ms: 1.13x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 107 ms: 1.07x faster                                                            |
| pickle_list          | 3.27 us                                                         | 3.25 us: 1.01x faster                                                           |
| pickle               | 7.99 us                                                         | 8.02 us: 1.00x slower                                                           |
| pickle_dict          | 20.1 us                                                         | 20.3 us: 1.01x slower                                                           |
| json_loads           | 20.0 us                                                         | 20.5 us: 1.02x slower                                                           |
| unpickle             | 9.23 us                                                         | 9.86 us: 1.07x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.17x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 26.2 ms: 1.19x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 23.6 ms: 1.25x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.22x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.22 ms: 1.42x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 94.5 us: 5.06x faster                                                           |
| generators                 | 52.2 ms                                                         | 21.6 ms: 2.41x faster                                                           |
| logging_silent             | 119 ns                                                          | 60.2 ns: 1.98x faster                                                           |
| spectral_norm              | 122 ms                                                          | 71.1 ms: 1.71x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.1 ms: 1.68x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 24.2 us: 1.66x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.51 ms: 1.64x faster                                                           |
| comprehensions             | 22.1 us                                                         | 14.1 us: 1.57x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 958 us: 1.56x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.20 ms: 1.49x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 214 us: 1.44x faster                                                            |
| json_dumps                 | 9.80 ms                                                         | 6.80 ms: 1.44x faster                                                           |
| chaos                      | 84.4 ms                                                         | 58.6 ms: 1.44x faster                                                           |
| deepcopy                   | 381 us                                                          | 268 us: 1.42x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.22 ms: 1.42x faster                                                           |
| richards_super             | 58.7 ms                                                         | 41.6 ms: 1.41x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 5.77 ms: 1.40x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 107 ms: 1.39x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.66 sec: 1.39x faster                                                          |
| float                      | 76.1 ms                                                         | 54.7 ms: 1.39x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 167 us: 1.39x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.40 us: 1.38x faster                                                           |
| scimark_sor                | 135 ms                                                          | 98.4 ms: 1.37x faster                                                           |
| richards                   | 48.8 ms                                                         | 35.8 ms: 1.36x faster                                                           |
| sympy_str                  | 283 ms                                                          | 208 ms: 1.36x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 58.5 ms: 1.36x faster                                                           |
| nbody                      | 126 ms                                                          | 93.7 ms: 1.34x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.16 ms: 1.34x faster                                                           |
| async_tree_none            | 343 ms                                                          | 257 ms: 1.33x faster                                                            |
| regex_compile              | 148 ms                                                          | 111 ms: 1.33x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 41.9 ms: 1.31x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.23 us: 1.31x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.76 us: 1.31x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 15.3 ms: 1.30x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 318 ms: 1.28x faster                                                            |
| sympy_expand               | 462 ms                                                          | 362 ms: 1.28x faster                                                            |
| pyflate                    | 471 ms                                                          | 376 ms: 1.25x faster                                                            |
| raytrace                   | 327 ms                                                          | 261 ms: 1.25x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 302 ms: 1.25x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 597 ms: 1.25x faster                                                            |
| nqueens                    | 111 ms                                                          | 89.2 ms: 1.25x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| tornado_http               | 118 ms                                                          | 95.2 ms: 1.24x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.65 us: 1.23x faster                                                           |
| scimark_fft                | 291 ms                                                          | 236 ms: 1.23x faster                                                            |
| go                         | 147 ms                                                          | 119 ms: 1.23x faster                                                            |
| async_tree_io              | 754 ms                                                          | 612 ms: 1.23x faster                                                            |
| fannkuch                   | 399 ms                                                          | 325 ms: 1.23x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 850 ms: 1.23x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 641 ms: 1.23x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.70 sec: 1.22x faster                                                          |
| xml_etree_generate         | 71.6 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 6.35 ms: 1.18x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 44.6 ms: 1.16x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.82 sec: 1.15x faster                                                          |
| scimark_lu                 | 102 ms                                                          | 89.2 ms: 1.15x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 79.7 ms: 1.14x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 507 ms: 1.14x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 66.6 ms: 1.13x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.90 us: 1.13x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 523 ms: 1.13x faster                                                            |
| json                       | 4.78 ms                                                         | 4.25 ms: 1.13x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.51 sec: 1.12x faster                                                          |
| pprint_safe_repr           | 819 ms                                                          | 735 ms: 1.12x faster                                                            |
| 2to3                       | 282 ms                                                          | 255 ms: 1.11x faster                                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.11x faster                                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 65.4 ms: 1.08x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 61.0 ns: 1.07x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 107 ms: 1.07x faster                                                            |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.02x faster                                                          |
| pidigits                   | 203 ms                                                          | 201 ms: 1.01x faster                                                            |
| pickle_list                | 3.27 us                                                         | 3.25 us: 1.01x faster                                                           |
| pickle                     | 7.99 us                                                         | 8.02 us: 1.00x slower                                                           |
| pickle_dict                | 20.1 us                                                         | 20.3 us: 1.01x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.39 ms: 1.01x slower                                                           |
| json_loads                 | 20.0 us                                                         | 20.5 us: 1.02x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 73.7 ms: 1.04x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 84.6 ms: 1.06x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 656 us: 1.06x slower                                                            |
| regex_dna                  | 122 ms                                                          | 130 ms: 1.07x slower                                                            |
| unpickle                   | 9.23 us                                                         | 9.86 us: 1.07x slower                                                           |
| async_generators           | 260 ms                                                          | 278 ms: 1.07x slower                                                            |
| regex_effbot               | 1.82 ms                                                         | 1.97 ms: 1.08x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.26 ms: 1.18x slower                                                           |
| python_startup             | 22.0 ms                                                         | 26.2 ms: 1.19x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 23.6 ms: 1.25x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 218 ms: 1.93x slower                                                            |
| coverage                   | 58.0 ms                                                         | 301 ms: 5.19x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.21x faster                                                                    |
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown