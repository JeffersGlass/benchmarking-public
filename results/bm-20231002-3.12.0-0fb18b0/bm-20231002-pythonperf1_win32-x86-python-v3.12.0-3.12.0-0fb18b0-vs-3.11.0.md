
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0
- machine: windows-x86
- commit hash: 0fb18b0
- commit date: 2023-10-02
- overall geometric mean: 1.09x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 280 ms: 1.01x faster                                            |
| chameleon      | 8.08 ms                                                         | 7.75 ms: 1.04x faster                                           |
| docutils       | 2.10 sec                                                        | 1.98 sec: 1.06x faster                                          |
| tornado_http   | 118 ms                                                          | 105 ms: 1.13x faster                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 298 ms: 1.15x faster                                            |
| async_tree_memoization     | 408 ms                                                          | 364 ms: 1.12x faster                                            |
| async_tree_io_tg           | 746 ms                                                          | 677 ms: 1.10x faster                                            |
| async_tree_io              | 754 ms                                                          | 693 ms: 1.09x faster                                            |
| async_tree_none_tg         | 301 ms                                                          | 278 ms: 1.08x faster                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 350 ms: 1.08x faster                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 546 ms: 1.06x faster                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 564 ms: 1.05x faster                                            |
| Geometric mean             | (ref)                                                           | 1.09x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 203 ms                                                          | 199 ms: 1.02x faster                                            |
| float          | 76.1 ms                                                         | 76.7 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                           | 1.00x faster                                                    |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 129 ms: 1.14x faster                                            |
| regex_v8       | 15.2 ms                                                         | 15.0 ms: 1.01x faster                                           |
| regex_dna      | 122 ms                                                          | 127 ms: 1.04x slower                                            |
| regex_effbot   | 1.82 ms                                                         | 2.04 ms: 1.12x slower                                           |
| Geometric mean | (ref)                                                           | 1.00x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 7.40 ms: 1.32x faster                                           |
| unpickle_list        | 3.28 us                                                         | 2.95 us: 1.11x faster                                           |
| unpickle_pure_python | 231 us                                                          | 210 us: 1.10x faster                                            |
| pickle_pure_python   | 309 us                                                          | 286 us: 1.08x faster                                            |
| tomli_loads          | 2.31 sec                                                        | 2.20 sec: 1.05x faster                                          |
| xml_etree_process    | 55.0 ms                                                         | 53.2 ms: 1.03x faster                                           |
| pickle               | 7.99 us                                                         | 7.79 us: 1.02x faster                                           |
| xml_etree_parse      | 114 ms                                                          | 113 ms: 1.01x faster                                            |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                           |
| xml_etree_generate   | 71.6 ms                                                         | 72.1 ms: 1.01x slower                                           |
| json_loads           | 20.0 us                                                         | 20.4 us: 1.02x slower                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 77.6 ms: 1.03x slower                                           |
| pickle_list          | 3.27 us                                                         | 3.37 us: 1.03x slower                                           |
| unpickle             | 9.23 us                                                         | 9.71 us: 1.05x slower                                           |
| Geometric mean       | (ref)                                                           | 1.04x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 18.8 ms                                                         | 19.1 ms: 1.01x slower                                           |
| python_startup         | 22.0 ms                                                         | 22.4 ms: 1.02x slower                                           |
| Geometric mean         | (ref)                                                           | 1.02x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 10.3 ms                                                         | 9.96 ms: 1.03x faster                                           |
| django_template | 37.4 ms                                                         | 36.9 ms: 1.01x faster                                           |
| Geometric mean  | (ref)                                                           | 1.02x faster                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 126 us: 3.79x faster                                            |
| generators                 | 52.2 ms                                                         | 38.5 ms: 1.36x faster                                           |
| json_dumps                 | 9.80 ms                                                         | 7.40 ms: 1.32x faster                                           |
| richards_super             | 58.7 ms                                                         | 46.5 ms: 1.26x faster                                           |
| sqlalchemy_imperative      | 15.4 ms                                                         | 12.3 ms: 1.26x faster                                           |
| chaos                      | 84.4 ms                                                         | 69.4 ms: 1.22x faster                                           |
| sympy_sum                  | 149 ms                                                          | 123 ms: 1.21x faster                                            |
| coverage                   | 58.0 ms                                                         | 48.4 ms: 1.20x faster                                           |
| sqlglot_parse              | 1.49 ms                                                         | 1.25 ms: 1.19x faster                                           |
| nqueens                    | 111 ms                                                          | 93.7 ms: 1.19x faster                                           |
| asyncio_tcp                | 787 ms                                                          | 662 ms: 1.19x faster                                            |
| sympy_str                  | 283 ms                                                          | 240 ms: 1.18x faster                                            |
| richards                   | 48.8 ms                                                         | 41.3 ms: 1.18x faster                                           |
| logging_silent             | 119 ns                                                          | 101 ns: 1.18x faster                                            |
| spectral_norm              | 122 ms                                                          | 104 ms: 1.17x faster                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.53 ms: 1.17x faster                                           |
| sympy_expand               | 462 ms                                                          | 398 ms: 1.16x faster                                            |
| async_tree_none            | 343 ms                                                          | 298 ms: 1.15x faster                                            |
| json                       | 4.78 ms                                                         | 4.15 ms: 1.15x faster                                           |
| comprehensions             | 22.1 us                                                         | 19.2 us: 1.15x faster                                           |
| crypto_pyaes               | 79.4 ms                                                         | 69.2 ms: 1.15x faster                                           |
| deltablue                  | 4.10 ms                                                         | 3.58 ms: 1.14x faster                                           |
| regex_compile              | 148 ms                                                          | 129 ms: 1.14x faster                                            |
| pprint_safe_repr           | 819 ms                                                          | 721 ms: 1.14x faster                                            |
| coroutines                 | 23.7 ms                                                         | 20.9 ms: 1.14x faster                                           |
| sympy_integrate            | 19.9 ms                                                         | 17.5 ms: 1.13x faster                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.50 sec: 1.13x faster                                          |
| fannkuch                   | 399 ms                                                          | 354 ms: 1.13x faster                                            |
| sqlglot_normalize          | 113 ms                                                          | 100 ms: 1.13x faster                                            |
| tornado_http               | 118 ms                                                          | 105 ms: 1.13x faster                                            |
| async_tree_memoization     | 408 ms                                                          | 364 ms: 1.12x faster                                            |
| sqlalchemy_declarative     | 115 ms                                                          | 103 ms: 1.12x faster                                            |
| unpickle_list              | 3.28 us                                                         | 2.95 us: 1.11x faster                                           |
| pyflate                    | 471 ms                                                          | 424 ms: 1.11x faster                                            |
| logging_simple             | 10.8 us                                                         | 9.75 us: 1.11x faster                                           |
| aiohttp                    | 1.17 ms                                                         | 1.06 ms: 1.11x faster                                           |
| async_tree_io_tg           | 746 ms                                                          | 677 ms: 1.10x faster                                            |
| unpickle_pure_python       | 231 us                                                          | 210 us: 1.10x faster                                            |
| hexiom                     | 7.51 ms                                                         | 6.82 ms: 1.10x faster                                           |
| logging_format             | 11.5 us                                                         | 10.4 us: 1.10x faster                                           |
| scimark_lu                 | 102 ms                                                          | 93.2 ms: 1.10x faster                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.86 ms: 1.10x faster                                           |
| dask                       | 355 ms                                                          | 323 ms: 1.10x faster                                            |
| async_tree_io              | 754 ms                                                          | 693 ms: 1.09x faster                                            |
| async_tree_none_tg         | 301 ms                                                          | 278 ms: 1.08x faster                                            |
| mdp                        | 2.07 sec                                                        | 1.91 sec: 1.08x faster                                          |
| pickle_pure_python         | 309 us                                                          | 286 us: 1.08x faster                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 350 ms: 1.08x faster                                            |
| scimark_fft                | 291 ms                                                          | 271 ms: 1.08x faster                                            |
| dulwich_log                | 62.8 ms                                                         | 58.5 ms: 1.07x faster                                           |
| mypy2                      | 626 ms                                                          | 584 ms: 1.07x faster                                            |
| go                         | 147 ms                                                          | 137 ms: 1.07x faster                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 48.5 ms: 1.07x faster                                           |
| pycparser                  | 1.04 sec                                                        | 978 ms: 1.07x faster                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 66.4 ms: 1.07x faster                                           |
| raytrace                   | 327 ms                                                          | 308 ms: 1.06x faster                                            |
| deepcopy                   | 381 us                                                          | 360 us: 1.06x faster                                            |
| docutils                   | 2.10 sec                                                        | 1.98 sec: 1.06x faster                                          |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 546 ms: 1.06x faster                                            |
| tomli_loads                | 2.31 sec                                                        | 2.20 sec: 1.05x faster                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 564 ms: 1.05x faster                                            |
| meteor_contest             | 90.9 ms                                                         | 86.9 ms: 1.05x faster                                           |
| unpack_sequence            | 65.2 ns                                                         | 62.5 ns: 1.04x faster                                           |
| deepcopy_memo              | 40.0 us                                                         | 38.4 us: 1.04x faster                                           |
| chameleon                  | 8.08 ms                                                         | 7.75 ms: 1.04x faster                                           |
| scimark_sor                | 135 ms                                                          | 130 ms: 1.04x faster                                            |
| sqlite_synth               | 2.15 us                                                         | 2.07 us: 1.04x faster                                           |
| xml_etree_process          | 55.0 ms                                                         | 53.2 ms: 1.03x faster                                           |
| mako                       | 10.3 ms                                                         | 9.96 ms: 1.03x faster                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.10 ms: 1.03x faster                                           |
| deepcopy_reduce            | 3.32 us                                                         | 3.23 us: 1.03x faster                                           |
| pickle                     | 7.99 us                                                         | 7.79 us: 1.02x faster                                           |
| pidigits                   | 203 ms                                                          | 199 ms: 1.02x faster                                            |
| django_template            | 37.4 ms                                                         | 36.9 ms: 1.01x faster                                           |
| xml_etree_parse            | 114 ms                                                          | 113 ms: 1.01x faster                                            |
| 2to3                       | 282 ms                                                          | 280 ms: 1.01x faster                                            |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                           |
| regex_v8                   | 15.2 ms                                                         | 15.0 ms: 1.01x faster                                           |
| xml_etree_generate         | 71.6 ms                                                         | 72.1 ms: 1.01x slower                                           |
| float                      | 76.1 ms                                                         | 76.7 ms: 1.01x slower                                           |
| python_startup_no_site     | 18.8 ms                                                         | 19.1 ms: 1.01x slower                                           |
| json_loads                 | 20.0 us                                                         | 20.4 us: 1.02x slower                                           |
| python_startup             | 22.0 ms                                                         | 22.4 ms: 1.02x slower                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 77.6 ms: 1.03x slower                                           |
| pickle_list                | 3.27 us                                                         | 3.37 us: 1.03x slower                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                          |
| telco                      | 5.29 ms                                                         | 5.51 ms: 1.04x slower                                           |
| regex_dna                  | 122 ms                                                          | 127 ms: 1.04x slower                                            |
| gc_traversal               | 1.38 ms                                                         | 1.44 ms: 1.05x slower                                           |
| unpickle                   | 9.23 us                                                         | 9.71 us: 1.05x slower                                           |
| create_gc_cycles           | 618 us                                                          | 652 us: 1.06x slower                                            |
| bench_mp_pool              | 70.9 ms                                                         | 75.4 ms: 1.06x slower                                           |
| regex_effbot               | 1.82 ms                                                         | 2.04 ms: 1.12x slower                                           |
| pathlib                    | 79.9 ms                                                         | 91.4 ms: 1.14x slower                                           |
| async_generators           | 260 ms                                                          | 313 ms: 1.21x slower                                            |
| Geometric mean             | (ref)                                                           | 1.09x faster                                                    |

Benchmark hidden because not significant (1): nbody
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown