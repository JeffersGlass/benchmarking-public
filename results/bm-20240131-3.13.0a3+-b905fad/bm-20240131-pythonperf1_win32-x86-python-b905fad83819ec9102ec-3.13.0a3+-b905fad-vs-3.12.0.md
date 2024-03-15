
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 233 ms: 1.20x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.65 ms: 1.37x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.73 sec: 1.15x faster                                                          |
| tornado_http   | 105 ms                                                          | 93.7 ms: 1.12x faster                                                           |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 301 ms: 1.16x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 239 ms: 1.16x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 314 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 587 ms: 1.15x faster                                                            |
| async_tree_io              | 693 ms                                                          | 613 ms: 1.13x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 488 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 505 ms: 1.12x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 72.6 ms: 1.75x faster                                                           |
| float          | 76.7 ms                                                         | 52.4 ms: 1.46x faster                                                           |
| pidigits       | 199 ms                                                          | 197 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.37x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 95.4 ms: 1.35x faster                                                           |
| regex_effbot   | 2.04 ms                                                         | 1.98 ms: 1.03x faster                                                           |
| regex_v8       | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                           |
| regex_dna      | 127 ms                                                          | 138 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 139 us: 1.50x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 205 us: 1.39x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.62 sec: 1.35x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 40.8 ms: 1.30x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 58.5 ms: 1.23x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 66.6 ms: 1.17x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.65 ms: 1.11x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.24 us: 1.04x faster                                                           |
| json_loads           | 20.4 us                                                         | 19.9 us: 1.02x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 111 ms: 1.02x faster                                                            |
| pickle_dict          | 19.9 us                                                         | 20.2 us: 1.01x slower                                                           |
| unpickle_list        | 2.95 us                                                         | 2.98 us: 1.01x slower                                                           |
| pickle               | 7.79 us                                                         | 7.92 us: 1.02x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.0 us: 1.03x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.1 ms: 1.03x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.4 ms: 1.07x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.01 ms: 1.42x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpack_sequence            | 62.5 ns                                                         | 31.1 ns: 2.01x faster                                                           |
| logging_silent             | 101 ns                                                          | 57.6 ns: 1.75x faster                                                           |
| nbody                      | 127 ms                                                          | 72.6 ms: 1.75x faster                                                           |
| comprehensions             | 19.2 us                                                         | 11.1 us: 1.72x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 22.4 us: 1.71x faster                                                           |
| generators                 | 38.5 ms                                                         | 23.1 ms: 1.66x faster                                                           |
| spectral_norm              | 104 ms                                                          | 64.3 ms: 1.61x faster                                                           |
| raytrace                   | 308 ms                                                          | 191 ms: 1.61x faster                                                            |
| hexiom                     | 6.82 ms                                                         | 4.24 ms: 1.61x faster                                                           |
| scimark_sor                | 130 ms                                                          | 80.8 ms: 1.61x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.23 ms: 1.61x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 59.8 ms: 1.56x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 139 us: 1.50x faster                                                            |
| chaos                      | 69.4 ms                                                         | 46.7 ms: 1.48x faster                                                           |
| float                      | 76.7 ms                                                         | 52.4 ms: 1.46x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 866 us: 1.44x faster                                                            |
| go                         | 137 ms                                                          | 95.3 ms: 1.44x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 46.2 ms: 1.44x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.5 ms: 1.44x faster                                                           |
| richards                   | 41.3 ms                                                         | 28.8 ms: 1.44x faster                                                           |
| richards_super             | 46.5 ms                                                         | 32.4 ms: 1.43x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.01 ms: 1.42x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.09 ms: 1.40x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 205 us: 1.39x faster                                                            |
| pyflate                    | 424 ms                                                          | 307 ms: 1.38x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.65 ms: 1.37x faster                                                           |
| scimark_fft                | 271 ms                                                          | 199 ms: 1.36x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.38 us: 1.36x faster                                                           |
| regex_compile              | 129 ms                                                          | 95.4 ms: 1.35x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.62 sec: 1.35x faster                                                          |
| typing_runtime_protocols   | 126 us                                                          | 93.8 us: 1.35x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 2.88 ms: 1.34x faster                                                           |
| deepcopy                   | 360 us                                                          | 270 us: 1.33x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 52.3 ms: 1.32x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 71.4 ms: 1.31x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 40.8 ms: 1.30x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.16 sec: 1.29x faster                                                          |
| pprint_safe_repr           | 721 ms                                                          | 570 ms: 1.27x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 14.1 ms: 1.25x faster                                                           |
| logging_format             | 10.4 us                                                         | 8.34 us: 1.25x faster                                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 38.9 ms: 1.25x faster                                                           |
| logging_simple             | 9.75 us                                                         | 7.85 us: 1.24x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 58.5 ms: 1.23x faster                                                           |
| sympy_sum                  | 123 ms                                                          | 101 ms: 1.21x faster                                                            |
| fannkuch                   | 354 ms                                                          | 292 ms: 1.21x faster                                                            |
| sympy_str                  | 240 ms                                                          | 198 ms: 1.21x faster                                                            |
| pycparser                  | 978 ms                                                          | 812 ms: 1.20x faster                                                            |
| 2to3                       | 280 ms                                                          | 233 ms: 1.20x faster                                                            |
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.61 sec: 1.19x faster                                                          |
| async_generators           | 313 ms                                                          | 265 ms: 1.18x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 66.6 ms: 1.17x faster                                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 301 ms: 1.16x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 239 ms: 1.16x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 314 ms: 1.16x faster                                                            |
| sympy_expand               | 398 ms                                                          | 344 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 587 ms: 1.15x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.73 sec: 1.15x faster                                                          |
| meteor_contest             | 86.9 ms                                                         | 75.9 ms: 1.14x faster                                                           |
| sqlite_synth               | 2.07 us                                                         | 1.83 us: 1.13x faster                                                           |
| async_tree_io              | 693 ms                                                          | 613 ms: 1.13x faster                                                            |
| tornado_http               | 105 ms                                                          | 93.7 ms: 1.12x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 488 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 505 ms: 1.12x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.65 ms: 1.11x faster                                                           |
| dask                       | 323 ms                                                          | 302 ms: 1.07x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.04 ms: 1.06x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 71.9 ms: 1.05x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.24 us: 1.04x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.98 ms: 1.03x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.41 ms: 1.02x faster                                                           |
| json_loads                 | 20.4 us                                                         | 19.9 us: 1.02x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 89.5 ms: 1.02x faster                                                           |
| json                       | 4.15 ms                                                         | 4.09 ms: 1.02x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 111 ms: 1.02x faster                                                            |
| pidigits                   | 199 ms                                                          | 197 ms: 1.01x faster                                                            |
| pickle_dict                | 19.9 us                                                         | 20.2 us: 1.01x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 2.98 us: 1.01x slower                                                           |
| pickle                     | 7.79 us                                                         | 7.92 us: 1.02x slower                                                           |
| create_gc_cycles           | 652 us                                                          | 664 us: 1.02x slower                                                            |
| python_startup             | 22.4 ms                                                         | 23.1 ms: 1.03x slower                                                           |
| unpickle                   | 9.71 us                                                         | 10.0 us: 1.03x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.4 ms: 1.07x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.99 ms: 1.09x slower                                                           |
| regex_dna                  | 127 ms                                                          | 138 ms: 1.09x slower                                                            |
| sqlglot_normalize          | 100 ms                                                          | 202 ms: 2.01x slower                                                            |
| coverage                   | 48.4 ms                                                         | 473 ms: 9.77x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.19x faster                                                                    |

Benchmark hidden because not significant (2): asyncio_tcp, asyncio_tcp_ssl
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown