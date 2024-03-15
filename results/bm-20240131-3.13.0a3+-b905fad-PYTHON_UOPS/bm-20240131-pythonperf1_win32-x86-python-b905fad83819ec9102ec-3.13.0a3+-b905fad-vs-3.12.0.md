
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 247 ms: 1.13x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.94 ms: 1.30x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                          |
| tornado_http   | 105 ms                                                          | 97.4 ms: 1.08x faster                                                           |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 252 ms: 1.18x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 302 ms: 1.16x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 243 ms: 1.14x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 318 ms: 1.14x faster                                                            |
| async_tree_io              | 693 ms                                                          | 611 ms: 1.13x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 606 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 516 ms: 1.09x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 506 ms: 1.08x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 87.6 ms: 1.45x faster                                                           |
| float          | 76.7 ms                                                         | 61.4 ms: 1.25x faster                                                           |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 107 ms: 1.20x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| regex_dna      | 127 ms                                                          | 122 ms: 1.04x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 152 us: 1.38x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 213 us: 1.34x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.67 sec: 1.32x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 42.0 ms: 1.27x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 59.6 ms: 1.21x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 69.7 ms: 1.11x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.94 ms: 1.07x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 111 ms: 1.02x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.35 us: 1.01x faster                                                           |
| json_loads           | 20.4 us                                                         | 20.5 us: 1.01x slower                                                           |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| unpickle             | 9.71 us                                                         | 9.92 us: 1.02x slower                                                           |
| unpickle_list        | 2.95 us                                                         | 3.13 us: 1.06x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.3 ms: 1.04x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.9 ms: 1.10x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 8.19 ms: 1.22x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 60.2 ns: 1.68x faster                                                           |
| generators                 | 38.5 ms                                                         | 23.2 ms: 1.66x faster                                                           |
| scimark_sor                | 130 ms                                                          | 82.6 ms: 1.57x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 24.4 us: 1.57x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 40.4 ns: 1.55x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 62.8 ms: 1.48x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.3 ms: 1.46x faster                                                           |
| raytrace                   | 308 ms                                                          | 211 ms: 1.46x faster                                                            |
| nbody                      | 127 ms                                                          | 87.6 ms: 1.45x faster                                                           |
| comprehensions             | 19.2 us                                                         | 13.8 us: 1.39x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 152 us: 1.38x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 91.3 us: 1.38x faster                                                           |
| richards_super             | 46.5 ms                                                         | 33.6 ms: 1.38x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.36 us: 1.37x faster                                                           |
| richards                   | 41.3 ms                                                         | 30.4 ms: 1.36x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 921 us: 1.35x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 213 us: 1.34x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.16 ms: 1.32x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.67 sec: 1.32x faster                                                          |
| deepcopy                   | 360 us                                                          | 274 us: 1.32x faster                                                            |
| go                         | 137 ms                                                          | 105 ms: 1.31x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.94 ms: 1.30x faster                                                           |
| chaos                      | 69.4 ms                                                         | 54.5 ms: 1.27x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 52.3 ms: 1.27x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 42.0 ms: 1.27x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 5.39 ms: 1.27x faster                                                           |
| float                      | 76.7 ms                                                         | 61.4 ms: 1.25x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.88 ms: 1.25x faster                                                           |
| pyflate                    | 424 ms                                                          | 340 ms: 1.25x faster                                                            |
| mako                       | 9.96 ms                                                         | 8.19 ms: 1.22x faster                                                           |
| scimark_fft                | 271 ms                                                          | 224 ms: 1.21x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 59.6 ms: 1.21x faster                                                           |
| logging_simple             | 9.75 us                                                         | 8.06 us: 1.21x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.24 sec: 1.21x faster                                                          |
| regex_compile              | 129 ms                                                          | 107 ms: 1.20x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 57.5 ms: 1.20x faster                                                           |
| fannkuch                   | 354 ms                                                          | 295 ms: 1.20x faster                                                            |
| nqueens                    | 93.7 ms                                                         | 78.2 ms: 1.20x faster                                                           |
| spectral_norm              | 104 ms                                                          | 87.2 ms: 1.19x faster                                                           |
| async_generators           | 313 ms                                                          | 264 ms: 1.19x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 607 ms: 1.19x faster                                                            |
| async_tree_none            | 298 ms                                                          | 252 ms: 1.18x faster                                                            |
| logging_format             | 10.4 us                                                         | 8.84 us: 1.18x faster                                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 41.3 ms: 1.17x faster                                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 302 ms: 1.16x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 243 ms: 1.14x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 318 ms: 1.14x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.4 ms: 1.14x faster                                                           |
| async_tree_io              | 693 ms                                                          | 611 ms: 1.13x faster                                                            |
| 2to3                       | 280 ms                                                          | 247 ms: 1.13x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 109 ms: 1.13x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.41 ms: 1.13x faster                                                           |
| pycparser                  | 978 ms                                                          | 871 ms: 1.12x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 606 ms: 1.12x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.71 sec: 1.12x faster                                                          |
| xml_etree_iterparse        | 77.6 ms                                                         | 69.7 ms: 1.11x faster                                                           |
| sqlite_synth               | 2.07 us                                                         | 1.87 us: 1.11x faster                                                           |
| sympy_str                  | 240 ms                                                          | 216 ms: 1.11x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                          |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 516 ms: 1.09x faster                                                            |
| meteor_contest             | 86.9 ms                                                         | 80.5 ms: 1.08x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 506 ms: 1.08x faster                                                            |
| tornado_http               | 105 ms                                                          | 97.4 ms: 1.08x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| json_dumps                 | 7.40 ms                                                         | 6.94 ms: 1.07x faster                                                           |
| sympy_expand               | 398 ms                                                          | 378 ms: 1.05x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.05 ms: 1.05x faster                                                           |
| regex_dna                  | 127 ms                                                          | 122 ms: 1.04x faster                                                            |
| dask                       | 323 ms                                                          | 311 ms: 1.04x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 88.7 ms: 1.03x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 73.4 ms: 1.03x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 111 ms: 1.02x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.42 ms: 1.02x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.35 us: 1.01x faster                                                           |
| json_loads                 | 20.4 us                                                         | 20.5 us: 1.01x slower                                                           |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| json                       | 4.15 ms                                                         | 4.20 ms: 1.01x slower                                                           |
| create_gc_cycles           | 652 us                                                          | 664 us: 1.02x slower                                                            |
| unpickle                   | 9.71 us                                                         | 9.92 us: 1.02x slower                                                           |
| python_startup             | 22.4 ms                                                         | 23.3 ms: 1.04x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 3.13 us: 1.06x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.9 ms: 1.10x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.18 ms: 1.12x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 213 ms: 2.13x slower                                                            |
| coverage                   | 48.4 ms                                                         | 481 ms: 9.93x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (4): asyncio_tcp, pidigits, asyncio_tcp_ssl, pickle
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown