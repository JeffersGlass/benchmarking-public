
# Results vs. 3.12.0

- fork: python
- ref: ae460d450ab854ca66d5
- machine: windows-x86
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 252 ms: 1.11x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.96 ms: 1.30x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                          |
| tornado_http   | 105 ms                                                          | 97.8 ms: 1.07x faster                                                           |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 256 ms: 1.16x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 305 ms: 1.15x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 243 ms: 1.14x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 320 ms: 1.14x faster                                                            |
| async_tree_io              | 693 ms                                                          | 611 ms: 1.14x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 601 ms: 1.13x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 511 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 498 ms: 1.10x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 54.5 ms: 1.41x faster                                                           |
| nbody          | 127 ms                                                          | 92.6 ms: 1.37x faster                                                           |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 108 ms: 1.20x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| regex_dna      | 127 ms                                                          | 122 ms: 1.04x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                        | 1.61 sec: 1.37x faster                                                          |
| unpickle_pure_python | 210 us                                                          | 161 us: 1.31x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 224 us: 1.27x faster                                                            |
| xml_etree_process    | 53.2 ms                                                         | 43.3 ms: 1.23x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.0 ms: 1.14x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.91 ms: 1.07x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.26 us: 1.03x faster                                                           |
| json_loads           | 20.4 us                                                         | 20.0 us: 1.02x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 20.0 us: 1.00x slower                                                           |
| pickle               | 7.79 us                                                         | 8.08 us: 1.04x slower                                                           |
| unpickle_list        | 2.95 us                                                         | 3.08 us: 1.05x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.3 us: 1.06x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 19.1 ms                                                         | 20.4 ms: 1.07x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.04x slower                                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.31 ms: 1.36x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 24.7 ms: 1.56x faster                                                           |
| logging_silent             | 101 ns                                                          | 66.7 ns: 1.52x faster                                                           |
| spectral_norm              | 104 ms                                                          | 70.6 ms: 1.47x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 26.4 us: 1.45x faster                                                           |
| float                      | 76.7 ms                                                         | 54.5 ms: 1.41x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.57 ms: 1.40x faster                                                           |
| scimark_sor                | 130 ms                                                          | 94.1 ms: 1.38x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 15.2 ms: 1.37x faster                                                           |
| nbody                      | 127 ms                                                          | 92.6 ms: 1.37x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.61 sec: 1.37x faster                                                          |
| mako                       | 9.96 ms                                                         | 7.31 ms: 1.36x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 69.1 ms: 1.35x faster                                                           |
| comprehensions             | 19.2 us                                                         | 14.3 us: 1.34x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 46.9 ns: 1.33x faster                                                           |
| richards                   | 41.3 ms                                                         | 31.2 ms: 1.33x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.45 us: 1.32x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 161 us: 1.31x faster                                                            |
| richards_super             | 46.5 ms                                                         | 35.6 ms: 1.31x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 960 us: 1.30x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.96 ms: 1.30x faster                                                           |
| raytrace                   | 308 ms                                                          | 237 ms: 1.30x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 98.1 us: 1.29x faster                                                           |
| deepcopy                   | 360 us                                                          | 280 us: 1.28x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 224 us: 1.27x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.21 ms: 1.26x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 43.3 ms: 1.23x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.20 ms: 1.20x faster                                                           |
| regex_compile              | 129 ms                                                          | 108 ms: 1.20x faster                                                            |
| logging_simple             | 9.75 us                                                         | 8.25 us: 1.18x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| async_tree_none            | 298 ms                                                          | 256 ms: 1.16x faster                                                            |
| logging_format             | 10.4 us                                                         | 8.95 us: 1.16x faster                                                           |
| chaos                      | 69.4 ms                                                         | 60.0 ms: 1.16x faster                                                           |
| fannkuch                   | 354 ms                                                          | 306 ms: 1.16x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 305 ms: 1.15x faster                                                            |
| pyflate                    | 424 ms                                                          | 370 ms: 1.14x faster                                                            |
| go                         | 137 ms                                                          | 120 ms: 1.14x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.0 ms: 1.14x faster                                                           |
| async_tree_none_tg         | 278 ms                                                          | 243 ms: 1.14x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 320 ms: 1.14x faster                                                            |
| pycparser                  | 978 ms                                                          | 861 ms: 1.14x faster                                                            |
| async_tree_io              | 693 ms                                                          | 611 ms: 1.14x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 109 ms: 1.13x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 601 ms: 1.13x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 61.5 ms: 1.12x faster                                                           |
| sympy_str                  | 240 ms                                                          | 214 ms: 1.12x faster                                                            |
| scimark_fft                | 271 ms                                                          | 242 ms: 1.12x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.7 ms: 1.12x faster                                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 43.5 ms: 1.12x faster                                                           |
| 2to3                       | 280 ms                                                          | 252 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 511 ms: 1.10x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 498 ms: 1.10x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.89 us: 1.09x faster                                                           |
| bench_thread_pool          | 1.10 ms                                                         | 1.01 ms: 1.09x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 84.3 ms: 1.08x faster                                                           |
| async_generators           | 313 ms                                                          | 290 ms: 1.08x faster                                                            |
| nqueens                    | 93.7 ms                                                         | 87.0 ms: 1.08x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| dask                       | 323 ms                                                          | 301 ms: 1.07x faster                                                            |
| asyncio_tcp                | 662 ms                                                          | 617 ms: 1.07x faster                                                            |
| tornado_http               | 105 ms                                                          | 97.8 ms: 1.07x faster                                                           |
| json_dumps                 | 7.40 ms                                                         | 6.91 ms: 1.07x faster                                                           |
| sympy_expand               | 398 ms                                                          | 374 ms: 1.06x faster                                                            |
| bench_mp_pool              | 75.4 ms                                                         | 71.2 ms: 1.06x faster                                                           |
| mdp                        | 1.91 sec                                                        | 1.82 sec: 1.05x faster                                                          |
| gc_traversal               | 1.44 ms                                                         | 1.37 ms: 1.05x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                          |
| hexiom                     | 6.82 ms                                                         | 6.50 ms: 1.05x faster                                                           |
| regex_dna                  | 127 ms                                                          | 122 ms: 1.04x faster                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.45 sec: 1.03x faster                                                          |
| pickle_list                | 3.37 us                                                         | 3.26 us: 1.03x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 84.2 ms: 1.03x faster                                                           |
| pprint_safe_repr           | 721 ms                                                          | 703 ms: 1.03x faster                                                            |
| json_loads                 | 20.4 us                                                         | 20.0 us: 1.02x faster                                                           |
| pickle_dict                | 19.9 us                                                         | 20.0 us: 1.00x slower                                                           |
| json                       | 4.15 ms                                                         | 4.19 ms: 1.01x slower                                                           |
| pickle                     | 7.79 us                                                         | 8.08 us: 1.04x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 3.08 us: 1.05x slower                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 70.2 ms: 1.06x slower                                                           |
| unpickle                   | 9.71 us                                                         | 10.3 us: 1.06x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.4 ms: 1.07x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.11 ms: 1.11x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 224 ms: 2.23x slower                                                            |
| coverage                   | 48.4 ms                                                         | 483 ms: 9.98x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (4): create_gc_cycles, xml_etree_parse, pidigits, python_startup
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown