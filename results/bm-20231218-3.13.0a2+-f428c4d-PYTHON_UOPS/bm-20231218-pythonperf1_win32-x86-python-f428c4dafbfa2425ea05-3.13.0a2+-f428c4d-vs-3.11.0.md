
# Results vs. 3.11.0

- fork: python
- ref: f428c4dafbfa2425ea05
- machine: windows-x86
- commit hash: f428c4d
- commit date: 2023-12-18
- overall geometric mean: 1.25x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 239 ms: 1.18x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.78 ms: 1.40x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.76 sec: 1.19x faster                                                          |
| tornado_http   | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 247 ms: 1.39x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 306 ms: 1.34x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 575 ms: 1.30x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 293 ms: 1.29x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 235 ms: 1.28x faster                                                            |
| async_tree_io              | 754 ms                                                          | 595 ms: 1.27x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 496 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 488 ms: 1.18x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.28x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 84.9 ms: 1.48x faster                                                           |
| float          | 76.1 ms                                                         | 59.4 ms: 1.28x faster                                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 105 ms: 1.40x faster                                                            |
| regex_dna      | 122 ms                                                          | 121 ms: 1.01x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 153 us: 1.51x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.62 ms: 1.48x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 209 us: 1.48x faster                                                            |
| tomli_loads          | 2.31 sec                                                        | 1.67 sec: 1.38x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 41.6 ms: 1.32x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 60.7 ms: 1.18x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.94 us: 1.12x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.5 ms: 1.10x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pickle               | 7.99 us                                                         | 7.65 us: 1.04x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.25 us: 1.01x faster                                                           |
| unpickle             | 9.23 us                                                         | 9.46 us: 1.03x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.17x faster                                                                    |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.7 ms: 1.03x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.2 ms: 1.07x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 8.06 ms: 1.28x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 89.7 us: 5.33x faster                                                           |
| generators                 | 52.2 ms                                                         | 22.0 ms: 2.37x faster                                                           |
| logging_silent             | 119 ns                                                          | 59.7 ns: 2.00x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.9 ms: 1.78x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 60.6 ms: 1.69x faster                                                           |
| richards                   | 48.8 ms                                                         | 29.2 ms: 1.67x faster                                                           |
| scimark_sor                | 135 ms                                                          | 82.9 ms: 1.63x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 919 us: 1.62x faster                                                            |
| deepcopy_memo              | 40.0 us                                                         | 24.7 us: 1.62x faster                                                           |
| comprehensions             | 22.1 us                                                         | 13.7 us: 1.61x faster                                                           |
| chaos                      | 84.4 ms                                                         | 52.5 ms: 1.61x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.8 ms: 1.60x faster                                                           |
| raytrace                   | 327 ms                                                          | 206 ms: 1.59x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 41.1 ns: 1.59x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.15 ms: 1.55x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 153 us: 1.51x faster                                                            |
| nbody                      | 126 ms                                                          | 84.9 ms: 1.48x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.62 ms: 1.48x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 209 us: 1.48x faster                                                            |
| deltablue                  | 4.10 ms                                                         | 2.83 ms: 1.45x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 105 ms: 1.42x faster                                                            |
| go                         | 147 ms                                                          | 104 ms: 1.42x faster                                                            |
| deepcopy                   | 381 us                                                          | 272 us: 1.40x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 56.7 ms: 1.40x faster                                                           |
| regex_compile              | 148 ms                                                          | 105 ms: 1.40x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.78 ms: 1.40x faster                                                           |
| pyflate                    | 471 ms                                                          | 338 ms: 1.39x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 5.41 ms: 1.39x faster                                                           |
| async_tree_none            | 343 ms                                                          | 247 ms: 1.39x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.67 sec: 1.38x faster                                                          |
| deepcopy_reduce            | 3.32 us                                                         | 2.40 us: 1.38x faster                                                           |
| sympy_str                  | 283 ms                                                          | 206 ms: 1.38x faster                                                            |
| nqueens                    | 111 ms                                                          | 81.1 ms: 1.37x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.95 us: 1.36x faster                                                           |
| spectral_norm              | 122 ms                                                          | 90.0 ms: 1.35x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.26 sec: 1.35x faster                                                          |
| scimark_monte_carlo        | 70.8 ms                                                         | 52.8 ms: 1.34x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.54 us: 1.34x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 611 ms: 1.34x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 306 ms: 1.34x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 41.6 ms: 1.32x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 15.2 ms: 1.31x faster                                                           |
| scimark_fft                | 291 ms                                                          | 223 ms: 1.31x faster                                                            |
| sympy_expand               | 462 ms                                                          | 355 ms: 1.30x faster                                                            |
| fannkuch                   | 399 ms                                                          | 307 ms: 1.30x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 575 ms: 1.30x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 293 ms: 1.29x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 235 ms: 1.28x faster                                                            |
| float                      | 76.1 ms                                                         | 59.4 ms: 1.28x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 40.5 ms: 1.28x faster                                                           |
| mako                       | 10.3 ms                                                         | 8.06 ms: 1.28x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 619 ms: 1.27x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.33 ms: 1.27x faster                                                           |
| pycparser                  | 1.04 sec                                                        | 821 ms: 1.27x faster                                                            |
| async_tree_io              | 754 ms                                                          | 595 ms: 1.27x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.70 sec: 1.22x faster                                                          |
| sqlite_synth               | 2.15 us                                                         | 1.79 us: 1.20x faster                                                           |
| tornado_http               | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.76 sec: 1.19x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 496 ms: 1.19x faster                                                            |
| dask                       | 355 ms                                                          | 300 ms: 1.18x faster                                                            |
| 2to3                       | 282 ms                                                          | 239 ms: 1.18x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 488 ms: 1.18x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 60.7 ms: 1.18x faster                                                           |
| json                       | 4.78 ms                                                         | 4.17 ms: 1.15x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 80.0 ms: 1.14x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.94 us: 1.12x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.5 ms: 1.10x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.07 ms: 1.07x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.65 us: 1.04x faster                                                           |
| pidigits                   | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| pickle_list                | 3.27 us                                                         | 3.25 us: 1.01x faster                                                           |
| regex_dna                  | 122 ms                                                          | 121 ms: 1.01x faster                                                            |
| bench_mp_pool              | 70.9 ms                                                         | 71.9 ms: 1.01x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.3 sec: 1.02x slower                                                          |
| async_generators           | 260 ms                                                          | 265 ms: 1.02x slower                                                            |
| unpickle                   | 9.23 us                                                         | 9.46 us: 1.03x slower                                                           |
| python_startup             | 22.0 ms                                                         | 22.7 ms: 1.03x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.42 ms: 1.03x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 646 us: 1.05x slower                                                            |
| regex_effbot               | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.2 ms: 1.07x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 87.6 ms: 1.10x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.98 ms: 1.13x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 206 ms: 1.82x slower                                                            |
| coverage                   | 58.0 ms                                                         | 479 ms: 8.26x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.25x faster                                                                    |

Benchmark hidden because not significant (1): json_loads
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: unknown