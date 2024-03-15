
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0
- machine: windows-x86
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.09x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 282 ms: 1.01x slower                                            |
| chameleon      | 7.75 ms                                                         | 8.08 ms: 1.04x slower                                           |
| docutils       | 1.98 sec                                                        | 2.10 sec: 1.06x slower                                          |
| tornado_http   | 105 ms                                                          | 118 ms: 1.13x slower                                            |
| Geometric mean | (ref)                                                           | 1.06x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 564 ms                                                          | 590 ms: 1.05x slower                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 577 ms: 1.06x slower                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 378 ms: 1.08x slower                                            |
| async_tree_none_tg         | 278 ms                                                          | 301 ms: 1.08x slower                                            |
| async_tree_io              | 693 ms                                                          | 754 ms: 1.09x slower                                            |
| async_tree_io_tg           | 677 ms                                                          | 746 ms: 1.10x slower                                            |
| async_tree_memoization     | 364 ms                                                          | 408 ms: 1.12x slower                                            |
| async_tree_none            | 298 ms                                                          | 343 ms: 1.15x slower                                            |
| Geometric mean             | (ref)                                                           | 1.09x slower                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 76.1 ms: 1.01x faster                                           |
| pidigits       | 199 ms                                                          | 203 ms: 1.02x slower                                            |
| Geometric mean | (ref)                                                           | 1.00x slower                                                    |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 2.04 ms                                                         | 1.82 ms: 1.12x faster                                           |
| regex_dna      | 127 ms                                                          | 122 ms: 1.04x faster                                            |
| regex_v8       | 15.0 ms                                                         | 15.2 ms: 1.01x slower                                           |
| regex_compile  | 129 ms                                                          | 148 ms: 1.14x slower                                            |
| Geometric mean | (ref)                                                           | 1.00x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpickle             | 9.71 us                                                         | 9.23 us: 1.05x faster                                           |
| pickle_list          | 3.37 us                                                         | 3.27 us: 1.03x faster                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 75.6 ms: 1.03x faster                                           |
| json_loads           | 20.4 us                                                         | 20.0 us: 1.02x faster                                           |
| xml_etree_generate   | 72.1 ms                                                         | 71.6 ms: 1.01x faster                                           |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                           |
| xml_etree_parse      | 113 ms                                                          | 114 ms: 1.01x slower                                            |
| pickle               | 7.79 us                                                         | 7.99 us: 1.02x slower                                           |
| xml_etree_process    | 53.2 ms                                                         | 55.0 ms: 1.03x slower                                           |
| tomli_loads          | 2.20 sec                                                        | 2.31 sec: 1.05x slower                                          |
| pickle_pure_python   | 286 us                                                          | 309 us: 1.08x slower                                            |
| unpickle_pure_python | 210 us                                                          | 231 us: 1.10x slower                                            |
| unpickle_list        | 2.95 us                                                         | 3.28 us: 1.11x slower                                           |
| json_dumps           | 7.40 ms                                                         | 9.80 ms: 1.32x slower                                           |
| Geometric mean       | (ref)                                                           | 1.04x slower                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.0 ms: 1.02x faster                                           |
| python_startup_no_site | 19.1 ms                                                         | 18.8 ms: 1.01x faster                                           |
| Geometric mean         | (ref)                                                           | 1.02x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| django_template | 36.9 ms                                                         | 37.4 ms: 1.01x slower                                           |
| mako            | 9.96 ms                                                         | 10.3 ms: 1.03x slower                                           |
| Geometric mean  | (ref)                                                           | 1.02x slower                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_generators           | 313 ms                                                          | 260 ms: 1.21x faster                                            |
| pathlib                    | 91.4 ms                                                         | 79.9 ms: 1.14x faster                                           |
| regex_effbot               | 2.04 ms                                                         | 1.82 ms: 1.12x faster                                           |
| bench_mp_pool              | 75.4 ms                                                         | 70.9 ms: 1.06x faster                                           |
| create_gc_cycles           | 652 us                                                          | 618 us: 1.06x faster                                            |
| unpickle                   | 9.71 us                                                         | 9.23 us: 1.05x faster                                           |
| gc_traversal               | 1.44 ms                                                         | 1.38 ms: 1.05x faster                                           |
| regex_dna                  | 127 ms                                                          | 122 ms: 1.04x faster                                            |
| telco                      | 5.51 ms                                                         | 5.29 ms: 1.04x faster                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.1 sec: 1.04x faster                                          |
| pickle_list                | 3.37 us                                                         | 3.27 us: 1.03x faster                                           |
| xml_etree_iterparse        | 77.6 ms                                                         | 75.6 ms: 1.03x faster                                           |
| python_startup             | 22.4 ms                                                         | 22.0 ms: 1.02x faster                                           |
| json_loads                 | 20.4 us                                                         | 20.0 us: 1.02x faster                                           |
| python_startup_no_site     | 19.1 ms                                                         | 18.8 ms: 1.01x faster                                           |
| float                      | 76.7 ms                                                         | 76.1 ms: 1.01x faster                                           |
| xml_etree_generate         | 72.1 ms                                                         | 71.6 ms: 1.01x faster                                           |
| regex_v8                   | 15.0 ms                                                         | 15.2 ms: 1.01x slower                                           |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                           |
| 2to3                       | 280 ms                                                          | 282 ms: 1.01x slower                                            |
| xml_etree_parse            | 113 ms                                                          | 114 ms: 1.01x slower                                            |
| django_template            | 36.9 ms                                                         | 37.4 ms: 1.01x slower                                           |
| pidigits                   | 199 ms                                                          | 203 ms: 1.02x slower                                            |
| pickle                     | 7.79 us                                                         | 7.99 us: 1.02x slower                                           |
| deepcopy_reduce            | 3.23 us                                                         | 3.32 us: 1.03x slower                                           |
| bench_thread_pool          | 1.10 ms                                                         | 1.14 ms: 1.03x slower                                           |
| mako                       | 9.96 ms                                                         | 10.3 ms: 1.03x slower                                           |
| xml_etree_process          | 53.2 ms                                                         | 55.0 ms: 1.03x slower                                           |
| sqlite_synth               | 2.07 us                                                         | 2.15 us: 1.04x slower                                           |
| scimark_sor                | 130 ms                                                          | 135 ms: 1.04x slower                                            |
| chameleon                  | 7.75 ms                                                         | 8.08 ms: 1.04x slower                                           |
| deepcopy_memo              | 38.4 us                                                         | 40.0 us: 1.04x slower                                           |
| unpack_sequence            | 62.5 ns                                                         | 65.2 ns: 1.04x slower                                           |
| meteor_contest             | 86.9 ms                                                         | 90.9 ms: 1.05x slower                                           |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 590 ms: 1.05x slower                                            |
| tomli_loads                | 2.20 sec                                                        | 2.31 sec: 1.05x slower                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 577 ms: 1.06x slower                                            |
| docutils                   | 1.98 sec                                                        | 2.10 sec: 1.06x slower                                          |
| deepcopy                   | 360 us                                                          | 381 us: 1.06x slower                                            |
| raytrace                   | 308 ms                                                          | 327 ms: 1.06x slower                                            |
| scimark_monte_carlo        | 66.4 ms                                                         | 70.8 ms: 1.07x slower                                           |
| pycparser                  | 978 ms                                                          | 1.04 sec: 1.07x slower                                          |
| sqlglot_optimize           | 48.5 ms                                                         | 51.8 ms: 1.07x slower                                           |
| go                         | 137 ms                                                          | 147 ms: 1.07x slower                                            |
| mypy2                      | 584 ms                                                          | 626 ms: 1.07x slower                                            |
| dulwich_log                | 58.5 ms                                                         | 62.8 ms: 1.07x slower                                           |
| scimark_fft                | 271 ms                                                          | 291 ms: 1.08x slower                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 378 ms: 1.08x slower                                            |
| pickle_pure_python         | 286 us                                                          | 309 us: 1.08x slower                                            |
| mdp                        | 1.91 sec                                                        | 2.07 sec: 1.08x slower                                          |
| async_tree_none_tg         | 278 ms                                                          | 301 ms: 1.08x slower                                            |
| async_tree_io              | 693 ms                                                          | 754 ms: 1.09x slower                                            |
| dask                       | 323 ms                                                          | 355 ms: 1.10x slower                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 4.23 ms: 1.10x slower                                           |
| scimark_lu                 | 93.2 ms                                                         | 102 ms: 1.10x slower                                            |
| logging_format             | 10.4 us                                                         | 11.5 us: 1.10x slower                                           |
| hexiom                     | 6.82 ms                                                         | 7.51 ms: 1.10x slower                                           |
| unpickle_pure_python       | 210 us                                                          | 231 us: 1.10x slower                                            |
| async_tree_io_tg           | 677 ms                                                          | 746 ms: 1.10x slower                                            |
| aiohttp                    | 1.06 ms                                                         | 1.17 ms: 1.11x slower                                           |
| logging_simple             | 9.75 us                                                         | 10.8 us: 1.11x slower                                           |
| pyflate                    | 424 ms                                                          | 471 ms: 1.11x slower                                            |
| unpickle_list              | 2.95 us                                                         | 3.28 us: 1.11x slower                                           |
| sqlalchemy_declarative     | 103 ms                                                          | 115 ms: 1.12x slower                                            |
| async_tree_memoization     | 364 ms                                                          | 408 ms: 1.12x slower                                            |
| tornado_http               | 105 ms                                                          | 118 ms: 1.13x slower                                            |
| sqlglot_normalize          | 100 ms                                                          | 113 ms: 1.13x slower                                            |
| fannkuch                   | 354 ms                                                          | 399 ms: 1.13x slower                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.70 sec: 1.13x slower                                          |
| sympy_integrate            | 17.5 ms                                                         | 19.9 ms: 1.13x slower                                           |
| coroutines                 | 20.9 ms                                                         | 23.7 ms: 1.14x slower                                           |
| pprint_safe_repr           | 721 ms                                                          | 819 ms: 1.14x slower                                            |
| regex_compile              | 129 ms                                                          | 148 ms: 1.14x slower                                            |
| deltablue                  | 3.58 ms                                                         | 4.10 ms: 1.14x slower                                           |
| crypto_pyaes               | 69.2 ms                                                         | 79.4 ms: 1.15x slower                                           |
| comprehensions             | 19.2 us                                                         | 22.1 us: 1.15x slower                                           |
| json                       | 4.15 ms                                                         | 4.78 ms: 1.15x slower                                           |
| async_tree_none            | 298 ms                                                          | 343 ms: 1.15x slower                                            |
| sympy_expand               | 398 ms                                                          | 462 ms: 1.16x slower                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.78 ms: 1.17x slower                                           |
| spectral_norm              | 104 ms                                                          | 122 ms: 1.17x slower                                            |
| logging_silent             | 101 ns                                                          | 119 ns: 1.18x slower                                            |
| richards                   | 41.3 ms                                                         | 48.8 ms: 1.18x slower                                           |
| sympy_str                  | 240 ms                                                          | 283 ms: 1.18x slower                                            |
| asyncio_tcp                | 662 ms                                                          | 787 ms: 1.19x slower                                            |
| nqueens                    | 93.7 ms                                                         | 111 ms: 1.19x slower                                            |
| sqlglot_parse              | 1.25 ms                                                         | 1.49 ms: 1.19x slower                                           |
| coverage                   | 48.4 ms                                                         | 58.0 ms: 1.20x slower                                           |
| sympy_sum                  | 123 ms                                                          | 149 ms: 1.21x slower                                            |
| chaos                      | 69.4 ms                                                         | 84.4 ms: 1.22x slower                                           |
| sqlalchemy_imperative      | 12.3 ms                                                         | 15.4 ms: 1.26x slower                                           |
| richards_super             | 46.5 ms                                                         | 58.7 ms: 1.26x slower                                           |
| json_dumps                 | 7.40 ms                                                         | 9.80 ms: 1.32x slower                                           |
| generators                 | 38.5 ms                                                         | 52.2 ms: 1.36x slower                                           |
| typing_runtime_protocols   | 126 us                                                          | 478 us: 3.79x slower                                            |
| Geometric mean             | (ref)                                                           | 1.09x slower                                                    |

Benchmark hidden because not significant (1): nbody
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: unknown