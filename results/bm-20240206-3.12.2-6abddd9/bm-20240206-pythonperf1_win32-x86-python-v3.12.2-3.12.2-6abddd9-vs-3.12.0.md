
# Results vs. 3.12.0

- fork: python
- ref: v3.12.2
- machine: windows-x86
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.02x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 274 ms: 1.02x faster                                            |
| chameleon      | 7.75 ms                                                         | 7.50 ms: 1.03x faster                                           |
| docutils       | 1.98 sec                                                        | 1.93 sec: 1.03x faster                                          |
| Geometric mean | (ref)                                                           | 1.02x faster                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization_tg  | 350 ms                                                          | 341 ms: 1.03x faster                                            |
| async_tree_io_tg           | 677 ms                                                          | 661 ms: 1.02x faster                                            |
| async_tree_io              | 693 ms                                                          | 678 ms: 1.02x faster                                            |
| async_tree_none_tg         | 278 ms                                                          | 273 ms: 1.02x faster                                            |
| async_tree_memoization     | 364 ms                                                          | 358 ms: 1.02x faster                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 555 ms: 1.02x faster                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 538 ms: 1.01x faster                                            |
| Geometric mean             | (ref)                                                           | 1.02x faster                                                    |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 73.6 ms: 1.04x faster                                           |
| nbody          | 127 ms                                                          | 124 ms: 1.03x faster                                            |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                            |
| Geometric mean | (ref)                                                           | 1.03x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                           |
| regex_dna      | 127 ms                                                          | 120 ms: 1.06x faster                                            |
| regex_compile  | 129 ms                                                          | 126 ms: 1.03x faster                                            |
| regex_v8       | 15.0 ms                                                         | 15.4 ms: 1.02x slower                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_list          | 3.37 us                                                         | 3.26 us: 1.03x faster                                           |
| unpickle             | 9.71 us                                                         | 9.42 us: 1.03x faster                                           |
| unpickle_pure_python | 210 us                                                          | 205 us: 1.03x faster                                            |
| xml_etree_parse      | 113 ms                                                          | 111 ms: 1.02x faster                                            |
| tomli_loads          | 2.20 sec                                                        | 2.17 sec: 1.01x faster                                          |
| xml_etree_iterparse  | 77.6 ms                                                         | 77.1 ms: 1.01x faster                                           |
| json_loads           | 20.4 us                                                         | 20.3 us: 1.00x faster                                           |
| pickle               | 7.79 us                                                         | 7.85 us: 1.01x slower                                           |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                           |
| xml_etree_generate   | 72.1 ms                                                         | 72.8 ms: 1.01x slower                                           |
| json_dumps           | 7.40 ms                                                         | 7.47 ms: 1.01x slower                                           |
| xml_etree_process    | 53.2 ms                                                         | 53.9 ms: 1.01x slower                                           |
| Geometric mean       | (ref)                                                           | 1.01x faster                                                    |

Benchmark hidden because not significant (2): pickle_pure_python, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 19.1 ms                                                         | 18.1 ms: 1.05x faster                                           |
| python_startup         | 22.4 ms                                                         | 21.3 ms: 1.05x faster                                           |
| Geometric mean         | (ref)                                                           | 1.05x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| django_template | 36.9 ms                                                         | 36.1 ms: 1.02x faster                                           |
| mako            | 9.96 ms                                                         | 9.80 ms: 1.02x faster                                           |
| Geometric mean  | (ref)                                                           | 1.02x faster                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 126 us                                                          | 113 us: 1.12x faster                                            |
| mypy2                      | 584 ms                                                          | 529 ms: 1.10x faster                                            |
| pathlib                    | 91.4 ms                                                         | 85.1 ms: 1.07x faster                                           |
| regex_effbot               | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                           |
| telco                      | 5.51 ms                                                         | 5.22 ms: 1.06x faster                                           |
| regex_dna                  | 127 ms                                                          | 120 ms: 1.06x faster                                            |
| bench_mp_pool              | 75.4 ms                                                         | 71.6 ms: 1.05x faster                                           |
| python_startup_no_site     | 19.1 ms                                                         | 18.1 ms: 1.05x faster                                           |
| dulwich_log                | 58.5 ms                                                         | 55.7 ms: 1.05x faster                                           |
| python_startup             | 22.4 ms                                                         | 21.3 ms: 1.05x faster                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.9 sec: 1.05x faster                                          |
| mdp                        | 1.91 sec                                                        | 1.83 sec: 1.04x faster                                          |
| float                      | 76.7 ms                                                         | 73.6 ms: 1.04x faster                                           |
| aiohttp                    | 1.06 ms                                                         | 1.02 ms: 1.04x faster                                           |
| pickle_list                | 3.37 us                                                         | 3.26 us: 1.03x faster                                           |
| chameleon                  | 7.75 ms                                                         | 7.50 ms: 1.03x faster                                           |
| docutils                   | 1.98 sec                                                        | 1.93 sec: 1.03x faster                                          |
| unpickle                   | 9.71 us                                                         | 9.42 us: 1.03x faster                                           |
| sqlalchemy_imperative      | 12.3 ms                                                         | 11.9 ms: 1.03x faster                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 341 ms: 1.03x faster                                            |
| nbody                      | 127 ms                                                          | 124 ms: 1.03x faster                                            |
| regex_compile              | 129 ms                                                          | 126 ms: 1.03x faster                                            |
| logging_simple             | 9.75 us                                                         | 9.50 us: 1.03x faster                                           |
| logging_format             | 10.4 us                                                         | 10.1 us: 1.03x faster                                           |
| gc_traversal               | 1.44 ms                                                         | 1.40 ms: 1.03x faster                                           |
| sympy_sum                  | 123 ms                                                          | 120 ms: 1.03x faster                                            |
| unpickle_pure_python       | 210 us                                                          | 205 us: 1.03x faster                                            |
| raytrace                   | 308 ms                                                          | 301 ms: 1.02x faster                                            |
| go                         | 137 ms                                                          | 134 ms: 1.02x faster                                            |
| async_tree_io_tg           | 677 ms                                                          | 661 ms: 1.02x faster                                            |
| pycparser                  | 978 ms                                                          | 955 ms: 1.02x faster                                            |
| async_tree_io              | 693 ms                                                          | 678 ms: 1.02x faster                                            |
| django_template            | 36.9 ms                                                         | 36.1 ms: 1.02x faster                                           |
| async_generators           | 313 ms                                                          | 307 ms: 1.02x faster                                            |
| sympy_integrate            | 17.5 ms                                                         | 17.2 ms: 1.02x faster                                           |
| 2to3                       | 280 ms                                                          | 274 ms: 1.02x faster                                            |
| sqlalchemy_declarative     | 103 ms                                                          | 101 ms: 1.02x faster                                            |
| chaos                      | 69.4 ms                                                         | 68.0 ms: 1.02x faster                                           |
| xml_etree_parse            | 113 ms                                                          | 111 ms: 1.02x faster                                            |
| deltablue                  | 3.58 ms                                                         | 3.52 ms: 1.02x faster                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 47.6 ms: 1.02x faster                                           |
| create_gc_cycles           | 652 us                                                          | 641 us: 1.02x faster                                            |
| async_tree_none_tg         | 278 ms                                                          | 273 ms: 1.02x faster                                            |
| deepcopy_memo              | 38.4 us                                                         | 37.8 us: 1.02x faster                                           |
| mako                       | 9.96 ms                                                         | 9.80 ms: 1.02x faster                                           |
| pyflate                    | 424 ms                                                          | 417 ms: 1.02x faster                                            |
| async_tree_memoization     | 364 ms                                                          | 358 ms: 1.02x faster                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 555 ms: 1.02x faster                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 538 ms: 1.01x faster                                            |
| spectral_norm              | 104 ms                                                          | 102 ms: 1.01x faster                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.51 ms: 1.01x faster                                           |
| sympy_expand               | 398 ms                                                          | 393 ms: 1.01x faster                                            |
| coroutines                 | 20.9 ms                                                         | 20.7 ms: 1.01x faster                                           |
| crypto_pyaes               | 69.2 ms                                                         | 68.5 ms: 1.01x faster                                           |
| tomli_loads                | 2.20 sec                                                        | 2.17 sec: 1.01x faster                                          |
| generators                 | 38.5 ms                                                         | 38.1 ms: 1.01x faster                                           |
| hexiom                     | 6.82 ms                                                         | 6.75 ms: 1.01x faster                                           |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                            |
| coverage                   | 48.4 ms                                                         | 48.0 ms: 1.01x faster                                           |
| dask                       | 323 ms                                                          | 321 ms: 1.01x faster                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 77.1 ms: 1.01x faster                                           |
| deepcopy                   | 360 us                                                          | 358 us: 1.01x faster                                            |
| sympy_str                  | 240 ms                                                          | 238 ms: 1.01x faster                                            |
| scimark_fft                | 271 ms                                                          | 269 ms: 1.01x faster                                            |
| json_loads                 | 20.4 us                                                         | 20.3 us: 1.00x faster                                           |
| meteor_contest             | 86.9 ms                                                         | 86.5 ms: 1.00x faster                                           |
| pickle                     | 7.79 us                                                         | 7.85 us: 1.01x slower                                           |
| sqlite_synth               | 2.07 us                                                         | 2.09 us: 1.01x slower                                           |
| scimark_lu                 | 93.2 ms                                                         | 94.0 ms: 1.01x slower                                           |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                           |
| xml_etree_generate         | 72.1 ms                                                         | 72.8 ms: 1.01x slower                                           |
| json_dumps                 | 7.40 ms                                                         | 7.47 ms: 1.01x slower                                           |
| richards_super             | 46.5 ms                                                         | 46.9 ms: 1.01x slower                                           |
| pprint_safe_repr           | 721 ms                                                          | 728 ms: 1.01x slower                                            |
| richards                   | 41.3 ms                                                         | 41.8 ms: 1.01x slower                                           |
| xml_etree_process          | 53.2 ms                                                         | 53.9 ms: 1.01x slower                                           |
| nqueens                    | 93.7 ms                                                         | 94.8 ms: 1.01x slower                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 67.3 ms: 1.01x slower                                           |
| sqlglot_normalize          | 100 ms                                                          | 102 ms: 1.01x slower                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.93 ms: 1.02x slower                                           |
| json                       | 4.15 ms                                                         | 4.24 ms: 1.02x slower                                           |
| comprehensions             | 19.2 us                                                         | 19.6 us: 1.02x slower                                           |
| regex_v8                   | 15.0 ms                                                         | 15.4 ms: 1.02x slower                                           |
| fannkuch                   | 354 ms                                                          | 367 ms: 1.04x slower                                            |
| Geometric mean             | (ref)                                                           | 1.02x faster                                                    |

Benchmark hidden because not significant (12): asyncio_tcp, tornado_http, bench_thread_pool, unpack_sequence, logging_silent, sqlglot_parse, pprint_pformat, scimark_sor, pickle_pure_python, deepcopy_reduce, async_tree_none, unpickle_list


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown