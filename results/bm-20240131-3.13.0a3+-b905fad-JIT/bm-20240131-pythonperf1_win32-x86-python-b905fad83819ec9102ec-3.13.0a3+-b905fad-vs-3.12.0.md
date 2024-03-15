
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 263 ms: 1.06x faster                                                            |
| chameleon      | 7.75 ms                                                         | 6.44 ms: 1.20x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.87 sec: 1.06x faster                                                          |
| tornado_http   | 105 ms                                                          | 101 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.09x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 265 ms: 1.12x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 319 ms: 1.10x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 253 ms: 1.10x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 333 ms: 1.09x faster                                                            |
| async_tree_io              | 693 ms                                                          | 640 ms: 1.08x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 630 ms: 1.07x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 529 ms: 1.07x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 516 ms: 1.06x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.09x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 56.2 ms: 1.37x faster                                                           |
| nbody          | 127 ms                                                          | 93.7 ms: 1.36x faster                                                           |
| pidigits       | 199 ms                                                          | 202 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 114 ms: 1.14x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                           |
| regex_dna      | 127 ms                                                          | 124 ms: 1.02x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 159 us: 1.32x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.69 sec: 1.30x faster                                                          |
| pickle_pure_python   | 286 us                                                          | 224 us: 1.28x faster                                                            |
| xml_etree_process    | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 69.4 ms: 1.12x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 7.06 ms: 1.05x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.26 us: 1.03x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 110 ms: 1.03x faster                                                            |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                                           |
| pickle               | 7.79 us                                                         | 8.16 us: 1.05x slower                                                           |
| unpickle_list        | 2.95 us                                                         | 3.12 us: 1.06x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                    |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.3 ms: 1.04x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 21.0 ms: 1.10x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.84 ms: 1.27x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 24.2 ms: 1.59x faster                                                           |
| logging_silent             | 101 ns                                                          | 67.1 ns: 1.51x faster                                                           |
| scimark_sor                | 130 ms                                                          | 88.3 ms: 1.47x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 26.3 us: 1.46x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.58 ms: 1.39x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 67.6 ms: 1.38x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 15.1 ms: 1.38x faster                                                           |
| float                      | 76.7 ms                                                         | 56.2 ms: 1.37x faster                                                           |
| nbody                      | 127 ms                                                          | 93.7 ms: 1.36x faster                                                           |
| spectral_norm              | 104 ms                                                          | 77.0 ms: 1.35x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 47.1 ns: 1.32x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 159 us: 1.32x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.69 sec: 1.30x faster                                                          |
| raytrace                   | 308 ms                                                          | 237 ms: 1.30x faster                                                            |
| richards                   | 41.3 ms                                                         | 32.1 ms: 1.29x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.52 us: 1.28x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 224 us: 1.28x faster                                                            |
| sqlglot_parse              | 1.25 ms                                                         | 980 us: 1.27x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 99.3 us: 1.27x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.84 ms: 1.27x faster                                                           |
| comprehensions             | 19.2 us                                                         | 15.2 us: 1.26x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                           |
| richards_super             | 46.5 ms                                                         | 37.5 ms: 1.24x faster                                                           |
| deepcopy                   | 360 us                                                          | 292 us: 1.24x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.25 ms: 1.23x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.17 ms: 1.22x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 6.44 ms: 1.20x faster                                                           |
| logging_simple             | 9.75 us                                                         | 8.29 us: 1.18x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| chaos                      | 69.4 ms                                                         | 59.4 ms: 1.17x faster                                                           |
| logging_format             | 10.4 us                                                         | 9.01 us: 1.16x faster                                                           |
| regex_compile              | 129 ms                                                          | 114 ms: 1.14x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.84 us: 1.13x faster                                                           |
| pycparser                  | 978 ms                                                          | 869 ms: 1.13x faster                                                            |
| async_tree_none            | 298 ms                                                          | 265 ms: 1.12x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 69.4 ms: 1.12x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 61.9 ms: 1.12x faster                                                           |
| go                         | 137 ms                                                          | 124 ms: 1.11x faster                                                            |
| pyflate                    | 424 ms                                                          | 384 ms: 1.10x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 319 ms: 1.10x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 253 ms: 1.10x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 333 ms: 1.09x faster                                                            |
| fannkuch                   | 354 ms                                                          | 325 ms: 1.09x faster                                                            |
| sympy_str                  | 240 ms                                                          | 221 ms: 1.09x faster                                                            |
| async_tree_io              | 693 ms                                                          | 640 ms: 1.08x faster                                                            |
| scimark_fft                | 271 ms                                                          | 250 ms: 1.08x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 114 ms: 1.08x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 630 ms: 1.07x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 45.4 ms: 1.07x faster                                                           |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 529 ms: 1.07x faster                                                            |
| 2to3                       | 280 ms                                                          | 263 ms: 1.06x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.87 sec: 1.06x faster                                                          |
| regex_effbot               | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 516 ms: 1.06x faster                                                            |
| nqueens                    | 93.7 ms                                                         | 89.0 ms: 1.05x faster                                                           |
| sympy_integrate            | 17.5 ms                                                         | 16.7 ms: 1.05x faster                                                           |
| sympy_expand               | 398 ms                                                          | 380 ms: 1.05x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 7.06 ms: 1.05x faster                                                           |
| async_generators           | 313 ms                                                          | 299 ms: 1.05x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.06 ms: 1.04x faster                                                           |
| tornado_http               | 105 ms                                                          | 101 ms: 1.03x faster                                                            |
| pickle_list                | 3.37 us                                                         | 3.26 us: 1.03x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 110 ms: 1.03x faster                                                            |
| dask                       | 323 ms                                                          | 315 ms: 1.03x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.41 ms: 1.02x faster                                                           |
| mdp                        | 1.91 sec                                                        | 1.87 sec: 1.02x faster                                                          |
| regex_dna                  | 127 ms                                                          | 124 ms: 1.02x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 89.6 ms: 1.02x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 6.71 ms: 1.02x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 85.6 ms: 1.02x faster                                                           |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| pidigits                   | 199 ms                                                          | 202 ms: 1.01x slower                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.52 sec: 1.01x slower                                                          |
| json                       | 4.15 ms                                                         | 4.22 ms: 1.02x slower                                                           |
| create_gc_cycles           | 652 us                                                          | 667 us: 1.02x slower                                                            |
| pprint_safe_repr           | 721 ms                                                          | 743 ms: 1.03x slower                                                            |
| python_startup             | 22.4 ms                                                         | 23.3 ms: 1.04x slower                                                           |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                                           |
| pickle                     | 7.79 us                                                         | 8.16 us: 1.05x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 3.12 us: 1.06x slower                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 71.6 ms: 1.08x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 21.0 ms: 1.10x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.51 ms: 1.18x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 232 ms: 2.31x slower                                                            |
| coverage                   | 48.4 ms                                                         | 483 ms: 9.97x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.08x faster                                                                    |

Benchmark hidden because not significant (4): bench_mp_pool, json_loads, asyncio_tcp_ssl, asyncio_tcp
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown