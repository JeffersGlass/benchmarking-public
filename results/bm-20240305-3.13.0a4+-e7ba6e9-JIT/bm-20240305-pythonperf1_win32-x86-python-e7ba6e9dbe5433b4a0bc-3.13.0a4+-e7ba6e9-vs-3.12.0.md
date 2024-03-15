# Results vs. 3.12.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: windows-x86
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.06x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 266 ms: 1.05x faster                                                            |
| chameleon      | 7.75 ms                                                         | 6.00 ms: 1.29x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.87 sec: 1.06x faster                                                          |
| tornado_http   | 105 ms                                                          | 99.9 ms: 1.05x faster                                                           |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 271 ms: 1.10x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 325 ms: 1.08x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 258 ms: 1.08x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 339 ms: 1.07x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 634 ms: 1.07x faster                                                            |
| async_tree_io              | 693 ms                                                          | 649 ms: 1.07x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 529 ms: 1.07x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 515 ms: 1.06x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 56.4 ms: 1.36x faster                                                           |
| nbody          | 127 ms                                                          | 96.7 ms: 1.31x faster                                                           |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 113 ms: 1.14x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.96 ms: 1.04x faster                                                           |
| regex_dna      | 127 ms                                                          | 130 ms: 1.02x slower                                                            |
| regex_v8       | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.02x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 286 us                                                          | 228 us: 1.25x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.77 sec: 1.24x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                           |
| unpickle_pure_python | 210 us                                                          | 170 us: 1.23x faster                                                            |
| xml_etree_generate   | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.3 ms: 1.14x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 7.10 ms: 1.04x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.03x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.28 us: 1.03x faster                                                           |
| json_loads           | 20.4 us                                                         | 20.3 us: 1.00x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 20.0 us: 1.01x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                                           |
| pickle               | 7.79 us                                                         | 8.16 us: 1.05x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                    |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 26.0 ms: 1.16x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 24.0 ms: 1.26x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.21x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako            | 9.96 ms                                                         | 7.19 ms: 1.38x faster                                                           |
| django_template | 36.9 ms                                                         | 31.9 ms: 1.16x faster                                                           |
| Geometric mean  | (ref)                                                           | 1.27x faster                                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 25.0 ms: 1.54x faster                                                           |
| logging_silent             | 101 ns                                                          | 68.8 ns: 1.47x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 44.3 ns: 1.41x faster                                                           |
| spectral_norm              | 104 ms                                                          | 73.7 ms: 1.41x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.19 ms: 1.38x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 15.2 ms: 1.38x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 28.0 us: 1.37x faster                                                           |
| float                      | 76.7 ms                                                         | 56.4 ms: 1.36x faster                                                           |
| comprehensions             | 19.2 us                                                         | 14.6 us: 1.31x faster                                                           |
| nbody                      | 127 ms                                                          | 96.7 ms: 1.31x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.75 ms: 1.30x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 6.00 ms: 1.29x faster                                                           |
| scimark_sor                | 130 ms                                                          | 102 ms: 1.27x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 101 us: 1.26x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 228 us: 1.25x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.59 us: 1.25x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.77 sec: 1.24x faster                                                          |
| xml_etree_process          | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 170 us: 1.23x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.14 ms: 1.23x faster                                                           |
| deepcopy                   | 360 us                                                          | 296 us: 1.22x faster                                                            |
| sqlglot_parse              | 1.25 ms                                                         | 1.03 ms: 1.21x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.30 ms: 1.18x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| logging_simple             | 9.75 us                                                         | 8.37 us: 1.17x faster                                                           |
| django_template            | 36.9 ms                                                         | 31.9 ms: 1.16x faster                                                           |
| logging_format             | 10.4 us                                                         | 9.07 us: 1.15x faster                                                           |
| regex_compile              | 129 ms                                                          | 113 ms: 1.14x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 60.8 ms: 1.14x faster                                                           |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.3 ms: 1.14x faster                                                           |
| scimark_fft                | 271 ms                                                          | 242 ms: 1.12x faster                                                            |
| chaos                      | 69.4 ms                                                         | 62.4 ms: 1.11x faster                                                           |
| pyflate                    | 424 ms                                                          | 385 ms: 1.10x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 112 ms: 1.10x faster                                                            |
| richards_super             | 46.5 ms                                                         | 42.3 ms: 1.10x faster                                                           |
| async_tree_none            | 298 ms                                                          | 271 ms: 1.10x faster                                                            |
| sympy_str                  | 240 ms                                                          | 219 ms: 1.09x faster                                                            |
| richards                   | 41.3 ms                                                         | 37.9 ms: 1.09x faster                                                           |
| sqlite_synth               | 2.07 us                                                         | 1.91 us: 1.09x faster                                                           |
| raytrace                   | 308 ms                                                          | 284 ms: 1.08x faster                                                            |
| pycparser                  | 978 ms                                                          | 902 ms: 1.08x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.77 sec: 1.08x faster                                                          |
| async_tree_memoization_tg  | 350 ms                                                          | 325 ms: 1.08x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 84.7 ms: 1.08x faster                                                           |
| sympy_integrate            | 17.5 ms                                                         | 16.3 ms: 1.08x faster                                                           |
| async_tree_none_tg         | 278 ms                                                          | 258 ms: 1.08x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 339 ms: 1.07x faster                                                            |
| scimark_lu                 | 93.2 ms                                                         | 86.9 ms: 1.07x faster                                                           |
| async_tree_io_tg           | 677 ms                                                          | 634 ms: 1.07x faster                                                            |
| async_tree_io              | 693 ms                                                          | 649 ms: 1.07x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 529 ms: 1.07x faster                                                            |
| hexiom                     | 6.82 ms                                                         | 6.40 ms: 1.07x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 515 ms: 1.06x faster                                                            |
| go                         | 137 ms                                                          | 130 ms: 1.06x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.87 sec: 1.06x faster                                                          |
| 2to3                       | 280 ms                                                          | 266 ms: 1.05x faster                                                            |
| tornado_http               | 105 ms                                                          | 99.9 ms: 1.05x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                          |
| json_dumps                 | 7.40 ms                                                         | 7.10 ms: 1.04x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.96 ms: 1.04x faster                                                           |
| sympy_expand               | 398 ms                                                          | 383 ms: 1.04x faster                                                            |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.03x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.40 ms: 1.03x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.28 us: 1.03x faster                                                           |
| async_generators           | 313 ms                                                          | 307 ms: 1.02x faster                                                            |
| fannkuch                   | 354 ms                                                          | 347 ms: 1.02x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 47.8 ms: 1.01x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 74.5 ms: 1.01x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 85.9 ms: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| json_loads                 | 20.4 us                                                         | 20.3 us: 1.00x faster                                                           |
| pickle_dict                | 19.9 us                                                         | 20.0 us: 1.01x slower                                                           |
| nqueens                    | 93.7 ms                                                         | 94.7 ms: 1.01x slower                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.52 sec: 1.01x slower                                                          |
| regex_dna                  | 127 ms                                                          | 130 ms: 1.02x slower                                                            |
| create_gc_cycles           | 652 us                                                          | 668 us: 1.03x slower                                                            |
| json                       | 4.15 ms                                                         | 4.28 ms: 1.03x slower                                                           |
| pprint_safe_repr           | 721 ms                                                          | 745 ms: 1.03x slower                                                            |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                                           |
| pickle                     | 7.79 us                                                         | 8.16 us: 1.05x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.16 ms: 1.12x slower                                                           |
| python_startup             | 22.4 ms                                                         | 26.0 ms: 1.16x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 24.0 ms: 1.26x slower                                                           |
| dask                       | 323 ms                                                          | 439 ms: 1.36x slower                                                            |
| sqlglot_normalize          | 100 ms                                                          | 241 ms: 2.40x slower                                                            |
| coverage                   | 48.4 ms                                                         | 497 ms: 10.26x slower                                                           |
| Geometric mean             | (ref)                                                           | 1.06x faster                                                                    |

Benchmark hidden because not significant (4): bench_thread_pool, unpickle_list, asyncio_tcp, scimark_monte_carlo
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown