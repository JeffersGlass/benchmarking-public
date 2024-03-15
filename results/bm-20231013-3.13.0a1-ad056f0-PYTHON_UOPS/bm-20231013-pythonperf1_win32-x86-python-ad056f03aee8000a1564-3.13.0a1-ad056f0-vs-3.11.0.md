
# Results vs. 3.11.0

- fork: python
- ref: ad056f03aee8000a1564
- machine: windows-x86
- commit hash: ad056f0
- commit date: 2023-10-13
- overall geometric mean: 1.08x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 309 ms: 1.09x slower                                                           |
| chameleon      | 8.08 ms                                                         | 9.20 ms: 1.14x slower                                                          |
| docutils       | 2.10 sec                                                        | 2.17 sec: 1.04x slower                                                         |
| tornado_http   | 118 ms                                                          | 116 ms: 1.02x faster                                                           |
| Geometric mean | (ref)                                                           | 1.06x slower                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 317 ms: 1.08x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 396 ms: 1.03x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 579 ms: 1.02x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 569 ms: 1.01x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 743 ms: 1.00x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 304 ms: 1.01x slower                                                           |
| async_tree_memoization_tg  | 378 ms                                                          | 386 ms: 1.02x slower                                                           |
| Geometric mean             | (ref)                                                           | 1.01x faster                                                                   |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 203 ms                                                          | 198 ms: 1.02x faster                                                           |
| float          | 76.1 ms                                                         | 92.7 ms: 1.22x slower                                                          |
| nbody          | 126 ms                                                          | 167 ms: 1.33x slower                                                           |
| Geometric mean | (ref)                                                           | 1.17x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_dna      | 122 ms                                                          | 119 ms: 1.02x faster                                                           |
| regex_effbot   | 1.82 ms                                                         | 1.93 ms: 1.06x slower                                                          |
| regex_compile  | 148 ms                                                          | 159 ms: 1.08x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.8 ms: 1.11x slower                                                          |
| Geometric mean | (ref)                                                           | 1.05x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|----------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 8.05 ms: 1.22x faster                                                          |
| unpickle_list        | 3.28 us                                                         | 3.00 us: 1.09x faster                                                          |
| pickle               | 7.99 us                                                         | 7.73 us: 1.03x faster                                                          |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                                          |
| pickle_list          | 3.27 us                                                         | 3.28 us: 1.01x slower                                                          |
| json_loads           | 20.0 us                                                         | 20.4 us: 1.02x slower                                                          |
| unpickle             | 9.23 us                                                         | 9.47 us: 1.03x slower                                                          |
| pickle_pure_python   | 309 us                                                          | 348 us: 1.12x slower                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 86.1 ms: 1.14x slower                                                          |
| xml_etree_process    | 55.0 ms                                                         | 64.0 ms: 1.16x slower                                                          |
| xml_etree_generate   | 71.6 ms                                                         | 84.7 ms: 1.18x slower                                                          |
| tomli_loads          | 2.31 sec                                                        | 2.79 sec: 1.20x slower                                                         |
| unpickle_pure_python | 231 us                                                          | 279 us: 1.21x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.05x slower                                                                   |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.3 ms: 1.02x slower                                                          |
| python_startup_no_site | 18.8 ms                                                         | 19.6 ms: 1.04x slower                                                          |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|-----------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 12.4 ms: 1.21x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1_win32-x86-python-ad056f03aee8000a1564-3.13.0a1-ad056f0 |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 143 us: 3.36x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 8.05 ms: 1.22x faster                                                          |
| asyncio_tcp                | 787 ms                                                          | 674 ms: 1.17x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 3.00 us: 1.09x faster                                                          |
| json                       | 4.78 ms                                                         | 4.41 ms: 1.08x faster                                                          |
| async_tree_none            | 343 ms                                                          | 317 ms: 1.08x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 139 ms: 1.07x faster                                                           |
| chaos                      | 84.4 ms                                                         | 80.1 ms: 1.05x faster                                                          |
| crypto_pyaes               | 79.4 ms                                                         | 76.0 ms: 1.04x faster                                                          |
| pickle                     | 7.99 us                                                         | 7.73 us: 1.03x faster                                                          |
| async_tree_memoization     | 408 ms                                                          | 396 ms: 1.03x faster                                                           |
| generators                 | 52.2 ms                                                         | 50.6 ms: 1.03x faster                                                          |
| sympy_str                  | 283 ms                                                          | 276 ms: 1.03x faster                                                           |
| nqueens                    | 111 ms                                                          | 109 ms: 1.03x faster                                                           |
| regex_dna                  | 122 ms                                                          | 119 ms: 1.02x faster                                                           |
| pidigits                   | 203 ms                                                          | 198 ms: 1.02x faster                                                           |
| tornado_http               | 118 ms                                                          | 116 ms: 1.02x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 579 ms: 1.02x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 569 ms: 1.01x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 2.12 us: 1.01x faster                                                          |
| sympy_expand               | 462 ms                                                          | 457 ms: 1.01x faster                                                           |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 743 ms: 1.00x faster                                                           |
| pickle_list                | 3.27 us                                                         | 3.28 us: 1.01x slower                                                          |
| sympy_integrate            | 19.9 ms                                                         | 20.1 ms: 1.01x slower                                                          |
| logging_format             | 11.5 us                                                         | 11.6 us: 1.01x slower                                                          |
| logging_simple             | 10.8 us                                                         | 10.9 us: 1.01x slower                                                          |
| async_tree_none_tg         | 301 ms                                                          | 304 ms: 1.01x slower                                                           |
| raytrace                   | 327 ms                                                          | 331 ms: 1.01x slower                                                           |
| python_startup             | 22.0 ms                                                         | 22.3 ms: 1.02x slower                                                          |
| json_loads                 | 20.0 us                                                         | 20.4 us: 1.02x slower                                                          |
| sqlglot_transpile          | 1.78 ms                                                         | 1.82 ms: 1.02x slower                                                          |
| sqlglot_parse              | 1.49 ms                                                         | 1.52 ms: 1.02x slower                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 386 ms: 1.02x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.5 sec: 1.02x slower                                                         |
| unpickle                   | 9.23 us                                                         | 9.47 us: 1.03x slower                                                          |
| docutils                   | 2.10 sec                                                        | 2.17 sec: 1.04x slower                                                         |
| bench_thread_pool          | 1.14 ms                                                         | 1.18 ms: 1.04x slower                                                          |
| bench_mp_pool              | 70.9 ms                                                         | 73.9 ms: 1.04x slower                                                          |
| sqlglot_normalize          | 113 ms                                                          | 118 ms: 1.04x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 645 us: 1.04x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 19.6 ms: 1.04x slower                                                          |
| comprehensions             | 22.1 us                                                         | 23.3 us: 1.05x slower                                                          |
| regex_effbot               | 1.82 ms                                                         | 1.93 ms: 1.06x slower                                                          |
| meteor_contest             | 90.9 ms                                                         | 96.7 ms: 1.06x slower                                                          |
| sqlglot_optimize           | 51.8 ms                                                         | 55.9 ms: 1.08x slower                                                          |
| regex_compile              | 148 ms                                                          | 159 ms: 1.08x slower                                                           |
| pycparser                  | 1.04 sec                                                        | 1.13 sec: 1.08x slower                                                         |
| deltablue                  | 4.10 ms                                                         | 4.47 ms: 1.09x slower                                                          |
| pprint_pformat             | 1.70 sec                                                        | 1.85 sec: 1.09x slower                                                         |
| richards_super             | 58.7 ms                                                         | 64.1 ms: 1.09x slower                                                          |
| 2to3                       | 282 ms                                                          | 309 ms: 1.09x slower                                                           |
| pprint_safe_repr           | 819 ms                                                          | 901 ms: 1.10x slower                                                           |
| deepcopy                   | 381 us                                                          | 420 us: 1.10x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.8 ms: 1.11x slower                                                          |
| spectral_norm              | 122 ms                                                          | 135 ms: 1.11x slower                                                           |
| pickle_pure_python         | 309 us                                                          | 348 us: 1.12x slower                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 3.73 us: 1.13x slower                                                          |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 4.77 ms: 1.13x slower                                                          |
| pathlib                    | 79.9 ms                                                         | 90.9 ms: 1.14x slower                                                          |
| xml_etree_iterparse        | 75.6 ms                                                         | 86.1 ms: 1.14x slower                                                          |
| chameleon                  | 8.08 ms                                                         | 9.20 ms: 1.14x slower                                                          |
| pyflate                    | 471 ms                                                          | 539 ms: 1.14x slower                                                           |
| scimark_fft                | 291 ms                                                          | 335 ms: 1.15x slower                                                           |
| logging_silent             | 119 ns                                                          | 138 ns: 1.16x slower                                                           |
| xml_etree_process          | 55.0 ms                                                         | 64.0 ms: 1.16x slower                                                          |
| unpack_sequence            | 65.2 ns                                                         | 76.1 ns: 1.17x slower                                                          |
| hexiom                     | 7.51 ms                                                         | 8.81 ms: 1.17x slower                                                          |
| scimark_monte_carlo        | 70.8 ms                                                         | 83.1 ms: 1.17x slower                                                          |
| xml_etree_generate         | 71.6 ms                                                         | 84.7 ms: 1.18x slower                                                          |
| coroutines                 | 23.7 ms                                                         | 28.2 ms: 1.19x slower                                                          |
| fannkuch                   | 399 ms                                                          | 475 ms: 1.19x slower                                                           |
| go                         | 147 ms                                                          | 175 ms: 1.19x slower                                                           |
| scimark_lu                 | 102 ms                                                          | 123 ms: 1.20x slower                                                           |
| tomli_loads                | 2.31 sec                                                        | 2.79 sec: 1.20x slower                                                         |
| mako                       | 10.3 ms                                                         | 12.4 ms: 1.21x slower                                                          |
| unpickle_pure_python       | 231 us                                                          | 279 us: 1.21x slower                                                           |
| richards                   | 48.8 ms                                                         | 59.1 ms: 1.21x slower                                                          |
| float                      | 76.1 ms                                                         | 92.7 ms: 1.22x slower                                                          |
| deepcopy_memo              | 40.0 us                                                         | 49.5 us: 1.24x slower                                                          |
| scimark_sor                | 135 ms                                                          | 168 ms: 1.24x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.92 ms: 1.31x slower                                                          |
| nbody                      | 126 ms                                                          | 167 ms: 1.33x slower                                                           |
| async_generators           | 260 ms                                                          | 365 ms: 1.41x slower                                                           |
| coverage                   | 58.0 ms                                                         | 690 ms: 11.89x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.08x slower                                                                   |

Benchmark hidden because not significant (4): xml_etree_parse, mdp, async_tree_io, gc_traversal
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown