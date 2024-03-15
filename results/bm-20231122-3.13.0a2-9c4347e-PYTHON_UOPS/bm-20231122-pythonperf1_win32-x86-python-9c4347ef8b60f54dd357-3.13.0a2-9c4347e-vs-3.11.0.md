
# Results vs. 3.11.0

- fork: python
- ref: 9c4347ef8b60f54dd357
- machine: windows-x86
- commit hash: 9c4347e
- commit date: 2023-11-22
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 268 ms: 1.05x faster                                                           |
| chameleon      | 8.08 ms                                                         | 6.15 ms: 1.31x faster                                                          |
| docutils       | 2.10 sec                                                        | 1.94 sec: 1.08x faster                                                         |
| tornado_http   | 118 ms                                                          | 112 ms: 1.06x faster                                                           |
| Geometric mean | (ref)                                                           | 1.12x faster                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 270 ms: 1.27x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 329 ms: 1.24x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 634 ms: 1.18x faster                                                           |
| async_tree_io              | 754 ms                                                          | 651 ms: 1.16x faster                                                           |
| async_tree_memoization_tg  | 378 ms                                                          | 327 ms: 1.16x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 264 ms: 1.14x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 523 ms: 1.13x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 518 ms: 1.11x faster                                                           |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 91.9 ms: 1.37x faster                                                          |
| float          | 76.1 ms                                                         | 62.3 ms: 1.22x faster                                                          |
| pidigits       | 203 ms                                                          | 198 ms: 1.02x faster                                                           |
| Geometric mean | (ref)                                                           | 1.20x faster                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 131 ms: 1.12x faster                                                           |
| regex_v8       | 15.2 ms                                                         | 16.3 ms: 1.08x slower                                                          |
| regex_dna      | 122 ms                                                          | 132 ms: 1.08x slower                                                           |
| regex_effbot   | 1.82 ms                                                         | 2.01 ms: 1.10x slower                                                          |
| Geometric mean | (ref)                                                           | 1.03x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|----------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 7.11 ms: 1.38x faster                                                          |
| unpickle_pure_python | 231 us                                                          | 173 us: 1.33x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 235 us: 1.31x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.79 sec: 1.29x faster                                                         |
| unpickle_list        | 3.28 us                                                         | 2.69 us: 1.22x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 47.9 ms: 1.15x faster                                                          |
| xml_etree_generate   | 71.6 ms                                                         | 67.3 ms: 1.06x faster                                                          |
| xml_etree_iterparse  | 75.6 ms                                                         | 71.7 ms: 1.05x faster                                                          |
| pickle               | 7.99 us                                                         | 7.66 us: 1.04x faster                                                          |
| xml_etree_parse      | 114 ms                                                          | 111 ms: 1.03x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.7 us: 1.02x faster                                                          |
| pickle_list          | 3.27 us                                                         | 3.20 us: 1.02x faster                                                          |
| json_loads           | 20.0 us                                                         | 19.9 us: 1.00x faster                                                          |
| unpickle             | 9.23 us                                                         | 9.65 us: 1.05x slower                                                          |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                          |
| python_startup_no_site | 18.8 ms                                                         | 21.2 ms: 1.13x slower                                                          |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|-----------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 8.20 ms: 1.25x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1_win32-x86-python-9c4347ef8b60f54dd357-3.13.0a2-9c4347e |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 105 us: 4.56x faster                                                           |
| generators                 | 52.2 ms                                                         | 29.6 ms: 1.77x faster                                                          |
| logging_silent             | 119 ns                                                          | 76.8 ns: 1.55x faster                                                          |
| unpack_sequence            | 65.2 ns                                                         | 42.6 ns: 1.53x faster                                                          |
| chaos                      | 84.4 ms                                                         | 57.2 ms: 1.48x faster                                                          |
| richards_super             | 58.7 ms                                                         | 40.6 ms: 1.45x faster                                                          |
| deepcopy_memo              | 40.0 us                                                         | 27.8 us: 1.44x faster                                                          |
| comprehensions             | 22.1 us                                                         | 15.7 us: 1.41x faster                                                          |
| sqlglot_parse              | 1.49 ms                                                         | 1.06 ms: 1.40x faster                                                          |
| json_dumps                 | 9.80 ms                                                         | 7.11 ms: 1.38x faster                                                          |
| nbody                      | 126 ms                                                          | 91.9 ms: 1.37x faster                                                          |
| richards                   | 48.8 ms                                                         | 35.6 ms: 1.37x faster                                                          |
| crypto_pyaes               | 79.4 ms                                                         | 58.8 ms: 1.35x faster                                                          |
| sqlglot_transpile          | 1.78 ms                                                         | 1.33 ms: 1.34x faster                                                          |
| unpickle_pure_python       | 231 us                                                          | 173 us: 1.33x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 3.08 ms: 1.33x faster                                                          |
| scimark_sor                | 135 ms                                                          | 102 ms: 1.33x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 235 us: 1.31x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 6.15 ms: 1.31x faster                                                          |
| coroutines                 | 23.7 ms                                                         | 18.3 ms: 1.29x faster                                                          |
| scimark_lu                 | 102 ms                                                          | 79.2 ms: 1.29x faster                                                          |
| tomli_loads                | 2.31 sec                                                        | 1.79 sec: 1.29x faster                                                         |
| pyflate                    | 471 ms                                                          | 367 ms: 1.28x faster                                                           |
| raytrace                   | 327 ms                                                          | 257 ms: 1.27x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.33 sec: 1.27x faster                                                         |
| async_tree_none            | 343 ms                                                          | 270 ms: 1.27x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 649 ms: 1.26x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.58 us: 1.26x faster                                                          |
| deepcopy_reduce            | 3.32 us                                                         | 2.64 us: 1.26x faster                                                          |
| spectral_norm              | 122 ms                                                          | 96.9 ms: 1.26x faster                                                          |
| mako                       | 10.3 ms                                                         | 8.20 ms: 1.25x faster                                                          |
| logging_format             | 11.5 us                                                         | 9.15 us: 1.25x faster                                                          |
| fannkuch                   | 399 ms                                                          | 321 ms: 1.25x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 329 ms: 1.24x faster                                                           |
| deepcopy                   | 381 us                                                          | 310 us: 1.23x faster                                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 57.8 ms: 1.22x faster                                                          |
| nqueens                    | 111 ms                                                          | 91.2 ms: 1.22x faster                                                          |
| float                      | 76.1 ms                                                         | 62.3 ms: 1.22x faster                                                          |
| unpickle_list              | 3.28 us                                                         | 2.69 us: 1.22x faster                                                          |
| go                         | 147 ms                                                          | 121 ms: 1.22x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 123 ms: 1.21x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 6.24 ms: 1.20x faster                                                          |
| scimark_fft                | 291 ms                                                          | 243 ms: 1.20x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 658 ms: 1.20x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 634 ms: 1.18x faster                                                           |
| sympy_str                  | 283 ms                                                          | 241 ms: 1.17x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.63 ms: 1.17x faster                                                          |
| json                       | 4.78 ms                                                         | 4.12 ms: 1.16x faster                                                          |
| async_tree_io              | 754 ms                                                          | 651 ms: 1.16x faster                                                           |
| async_tree_memoization_tg  | 378 ms                                                          | 327 ms: 1.16x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.87 us: 1.15x faster                                                          |
| xml_etree_process          | 55.0 ms                                                         | 47.9 ms: 1.15x faster                                                          |
| sympy_integrate            | 19.9 ms                                                         | 17.4 ms: 1.14x faster                                                          |
| mdp                        | 2.07 sec                                                        | 1.81 sec: 1.14x faster                                                         |
| async_tree_none_tg         | 301 ms                                                          | 264 ms: 1.14x faster                                                           |
| sympy_expand               | 462 ms                                                          | 408 ms: 1.13x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 523 ms: 1.13x faster                                                           |
| regex_compile              | 148 ms                                                          | 131 ms: 1.12x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 518 ms: 1.11x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 46.8 ms: 1.11x faster                                                          |
| pycparser                  | 1.04 sec                                                        | 955 ms: 1.09x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 83.2 ms: 1.09x faster                                                          |
| dask                       | 355 ms                                                          | 328 ms: 1.08x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.94 sec: 1.08x faster                                                         |
| xml_etree_generate         | 71.6 ms                                                         | 67.3 ms: 1.06x faster                                                          |
| tornado_http               | 118 ms                                                          | 112 ms: 1.06x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 71.7 ms: 1.05x faster                                                          |
| 2to3                       | 282 ms                                                          | 268 ms: 1.05x faster                                                           |
| pickle                     | 7.99 us                                                         | 7.66 us: 1.04x faster                                                          |
| bench_thread_pool          | 1.14 ms                                                         | 1.09 ms: 1.04x faster                                                          |
| xml_etree_parse            | 114 ms                                                          | 111 ms: 1.03x faster                                                           |
| pidigits                   | 203 ms                                                          | 198 ms: 1.02x faster                                                           |
| pickle_dict                | 20.1 us                                                         | 19.7 us: 1.02x faster                                                          |
| pickle_list                | 3.27 us                                                         | 3.20 us: 1.02x faster                                                          |
| json_loads                 | 20.0 us                                                         | 19.9 us: 1.00x faster                                                          |
| gc_traversal               | 1.38 ms                                                         | 1.40 ms: 1.02x slower                                                          |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.4 sec: 1.02x slower                                                         |
| unpickle                   | 9.23 us                                                         | 9.65 us: 1.05x slower                                                          |
| create_gc_cycles           | 618 us                                                          | 648 us: 1.05x slower                                                           |
| python_startup             | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                          |
| bench_mp_pool              | 70.9 ms                                                         | 75.2 ms: 1.06x slower                                                          |
| regex_v8                   | 15.2 ms                                                         | 16.3 ms: 1.08x slower                                                          |
| regex_dna                  | 122 ms                                                          | 132 ms: 1.08x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 2.01 ms: 1.10x slower                                                          |
| pathlib                    | 79.9 ms                                                         | 89.1 ms: 1.11x slower                                                          |
| python_startup_no_site     | 18.8 ms                                                         | 21.2 ms: 1.13x slower                                                          |
| async_generators           | 260 ms                                                          | 304 ms: 1.17x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.40 ms: 1.21x slower                                                          |
| sqlglot_normalize          | 113 ms                                                          | 237 ms: 2.09x slower                                                           |
| coverage                   | 58.0 ms                                                         | 510 ms: 8.79x slower                                                           |
| Geometric mean             | (ref)                                                           | 1.14x faster                                                                   |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown