
# Results vs. 3.12.0

- fork: python
- ref: f428c4dafbfa2425ea05
- machine: windows-x86
- commit hash: f428c4d
- commit date: 2023-12-18
- overall geometric mean: 1.15x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 239 ms: 1.17x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.78 ms: 1.34x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.76 sec: 1.13x faster                                                          |
| tornado_http   | 105 ms                                                          | 99.1 ms: 1.06x faster                                                           |
| Geometric mean | (ref)                                                           | 1.17x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 247 ms: 1.20x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 293 ms: 1.20x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 306 ms: 1.19x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 235 ms: 1.18x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 575 ms: 1.18x faster                                                            |
| async_tree_io              | 693 ms                                                          | 595 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 496 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 488 ms: 1.12x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 84.9 ms: 1.50x faster                                                           |
| float          | 76.7 ms                                                         | 59.4 ms: 1.29x faster                                                           |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 105 ms: 1.22x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.91 ms: 1.06x faster                                                           |
| regex_dna      | 127 ms                                                          | 121 ms: 1.05x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.3 ms: 1.09x slower                                                           |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 153 us: 1.37x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 209 us: 1.37x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.67 sec: 1.31x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 41.6 ms: 1.28x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 60.7 ms: 1.19x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.5 ms: 1.13x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.62 ms: 1.12x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| unpickle             | 9.71 us                                                         | 9.46 us: 1.03x faster                                                           |
| json_loads           | 20.4 us                                                         | 20.0 us: 1.02x faster                                                           |
| pickle               | 7.79 us                                                         | 7.65 us: 1.02x faster                                                           |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (2): unpickle_list, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.7 ms: 1.01x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.2 ms: 1.06x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.04x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 8.06 ms: 1.24x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.0 ms: 1.75x faster                                                           |
| logging_silent             | 101 ns                                                          | 59.7 ns: 1.69x faster                                                           |
| scimark_sor                | 130 ms                                                          | 82.9 ms: 1.57x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 24.7 us: 1.55x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 60.6 ms: 1.54x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 41.1 ns: 1.52x faster                                                           |
| raytrace                   | 308 ms                                                          | 206 ms: 1.50x faster                                                            |
| nbody                      | 127 ms                                                          | 84.9 ms: 1.50x faster                                                           |
| richards                   | 41.3 ms                                                         | 29.2 ms: 1.42x faster                                                           |
| richards_super             | 46.5 ms                                                         | 32.9 ms: 1.41x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.8 ms: 1.41x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 89.7 us: 1.41x faster                                                           |
| comprehensions             | 19.2 us                                                         | 13.7 us: 1.40x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 153 us: 1.37x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 209 us: 1.37x faster                                                            |
| sqlglot_parse              | 1.25 ms                                                         | 919 us: 1.36x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.40 us: 1.35x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 5.78 ms: 1.34x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.15 ms: 1.33x faster                                                           |
| go                         | 137 ms                                                          | 104 ms: 1.32x faster                                                            |
| deepcopy                   | 360 us                                                          | 272 us: 1.32x faster                                                            |
| chaos                      | 69.4 ms                                                         | 52.5 ms: 1.32x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.67 sec: 1.31x faster                                                          |
| float                      | 76.7 ms                                                         | 59.4 ms: 1.29x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 41.6 ms: 1.28x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.83 ms: 1.26x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 5.41 ms: 1.26x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 52.8 ms: 1.26x faster                                                           |
| pyflate                    | 424 ms                                                          | 338 ms: 1.25x faster                                                            |
| mako                       | 9.96 ms                                                         | 8.06 ms: 1.24x faster                                                           |
| logging_simple             | 9.75 us                                                         | 7.95 us: 1.23x faster                                                           |
| regex_compile              | 129 ms                                                          | 105 ms: 1.22x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 56.7 ms: 1.22x faster                                                           |
| logging_format             | 10.4 us                                                         | 8.54 us: 1.22x faster                                                           |
| scimark_fft                | 271 ms                                                          | 223 ms: 1.22x faster                                                            |
| async_tree_none            | 298 ms                                                          | 247 ms: 1.20x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 40.5 ms: 1.20x faster                                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 293 ms: 1.20x faster                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.26 sec: 1.19x faster                                                          |
| pycparser                  | 978 ms                                                          | 821 ms: 1.19x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 306 ms: 1.19x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 60.7 ms: 1.19x faster                                                           |
| async_tree_none_tg         | 278 ms                                                          | 235 ms: 1.18x faster                                                            |
| async_generators           | 313 ms                                                          | 265 ms: 1.18x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 611 ms: 1.18x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 575 ms: 1.18x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 105 ms: 1.17x faster                                                            |
| 2to3                       | 280 ms                                                          | 239 ms: 1.17x faster                                                            |
| async_tree_io              | 693 ms                                                          | 595 ms: 1.16x faster                                                            |
| sympy_str                  | 240 ms                                                          | 206 ms: 1.16x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.33 ms: 1.16x faster                                                           |
| sqlite_synth               | 2.07 us                                                         | 1.79 us: 1.16x faster                                                           |
| sympy_integrate            | 17.5 ms                                                         | 15.2 ms: 1.16x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 81.1 ms: 1.15x faster                                                           |
| fannkuch                   | 354 ms                                                          | 307 ms: 1.15x faster                                                            |
| spectral_norm              | 104 ms                                                          | 90.0 ms: 1.15x faster                                                           |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 496 ms: 1.14x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.5 ms: 1.13x faster                                                           |
| docutils                   | 1.98 sec                                                        | 1.76 sec: 1.13x faster                                                          |
| mdp                        | 1.91 sec                                                        | 1.70 sec: 1.13x faster                                                          |
| sympy_expand               | 398 ms                                                          | 355 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 488 ms: 1.12x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.62 ms: 1.12x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 80.0 ms: 1.09x faster                                                           |
| dask                       | 323 ms                                                          | 300 ms: 1.08x faster                                                            |
| asyncio_tcp                | 662 ms                                                          | 619 ms: 1.07x faster                                                            |
| regex_effbot               | 2.04 ms                                                         | 1.91 ms: 1.06x faster                                                           |
| tornado_http               | 105 ms                                                          | 99.1 ms: 1.06x faster                                                           |
| regex_dna                  | 127 ms                                                          | 121 ms: 1.05x faster                                                            |
| bench_mp_pool              | 75.4 ms                                                         | 71.9 ms: 1.05x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 87.6 ms: 1.04x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| unpickle                   | 9.71 us                                                         | 9.46 us: 1.03x faster                                                           |
| json_loads                 | 20.4 us                                                         | 20.0 us: 1.02x faster                                                           |
| pickle                     | 7.79 us                                                         | 7.65 us: 1.02x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.3 sec: 1.02x faster                                                          |
| gc_traversal               | 1.44 ms                                                         | 1.42 ms: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| python_startup             | 22.4 ms                                                         | 22.7 ms: 1.01x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.2 ms: 1.06x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.98 ms: 1.08x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.3 ms: 1.09x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 206 ms: 2.05x slower                                                            |
| coverage                   | 48.4 ms                                                         | 479 ms: 9.90x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.15x faster                                                                    |

Benchmark hidden because not significant (5): bench_thread_pool, create_gc_cycles, unpickle_list, pickle_dict, json
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown