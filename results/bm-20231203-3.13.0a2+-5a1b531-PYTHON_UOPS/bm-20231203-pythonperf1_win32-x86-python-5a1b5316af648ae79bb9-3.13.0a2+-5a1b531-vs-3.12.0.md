
# Results vs. 3.12.0

- fork: python
- ref: 5a1b5316af648ae79bb9
- machine: windows-x86
- commit hash: 5a1b531
- commit date: 2023-12-03
- overall geometric mean: 1.14x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 312 ms: 1.11x slower                                                            |
| chameleon      | 7.75 ms                                                         | 9.94 ms: 1.28x slower                                                           |
| docutils       | 1.98 sec                                                        | 2.15 sec: 1.08x slower                                                          |
| tornado_http   | 105 ms                                                          | 113 ms: 1.07x slower                                                            |
| Geometric mean | (ref)                                                           | 1.13x slower                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 564 ms                                                          | 592 ms: 1.05x slower                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 578 ms: 1.06x slower                                                            |
| async_tree_none            | 298 ms                                                          | 330 ms: 1.11x slower                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 395 ms: 1.13x slower                                                            |
| async_tree_io              | 693 ms                                                          | 782 ms: 1.13x slower                                                            |
| async_tree_memoization     | 364 ms                                                          | 412 ms: 1.13x slower                                                            |
| async_tree_io_tg           | 677 ms                                                          | 769 ms: 1.14x slower                                                            |
| async_tree_none_tg         | 278 ms                                                          | 317 ms: 1.14x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.11x slower                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 98.2 ms: 1.29x faster                                                           |
| float          | 76.7 ms                                                         | 68.7 ms: 1.12x faster                                                           |
| pidigits       | 199 ms                                                          | 200 ms: 1.00x slower                                                            |
| Geometric mean | (ref)                                                           | 1.13x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_effbot   | 2.04 ms                                                         | 1.94 ms: 1.05x faster                                                           |
| regex_dna      | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 17.2 ms: 1.14x slower                                                           |
| regex_compile  | 129 ms                                                          | 149 ms: 1.15x slower                                                            |
| Geometric mean | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_list        | 2.95 us                                                         | 2.71 us: 1.09x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.17 us: 1.06x faster                                                           |
| pickle               | 7.79 us                                                         | 7.54 us: 1.03x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 111 ms: 1.02x faster                                                            |
| pickle_dict          | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 78.3 ms: 1.01x slower                                                           |
| json_loads           | 20.4 us                                                         | 21.0 us: 1.03x slower                                                           |
| json_dumps           | 7.40 ms                                                         | 8.30 ms: 1.12x slower                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 83.0 ms: 1.15x slower                                                           |
| xml_etree_process    | 53.2 ms                                                         | 64.6 ms: 1.21x slower                                                           |
| pickle_pure_python   | 286 us                                                          | 385 us: 1.35x slower                                                            |
| unpickle_pure_python | 210 us                                                          | 304 us: 1.45x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.07x slower                                                                    |

Benchmark hidden because not significant (2): unpickle, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.9 ms: 1.02x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.5 ms: 1.07x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 8.09 ms: 1.23x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody                      | 127 ms                                                          | 98.2 ms: 1.29x faster                                                           |
| mako                       | 9.96 ms                                                         | 8.09 ms: 1.23x faster                                                           |
| spectral_norm              | 104 ms                                                          | 89.8 ms: 1.16x faster                                                           |
| scimark_fft                | 271 ms                                                          | 236 ms: 1.15x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.45 ms: 1.12x faster                                                           |
| float                      | 76.7 ms                                                         | 68.7 ms: 1.12x faster                                                           |
| sqlite_synth               | 2.07 us                                                         | 1.89 us: 1.10x faster                                                           |
| unpickle_list              | 2.95 us                                                         | 2.71 us: 1.09x faster                                                           |
| comprehensions             | 19.2 us                                                         | 17.8 us: 1.08x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.17 us: 1.06x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.94 ms: 1.05x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 66.0 ms: 1.05x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 72.4 ms: 1.04x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.39 ms: 1.04x faster                                                           |
| pickle                     | 7.79 us                                                         | 7.54 us: 1.03x faster                                                           |
| regex_dna                  | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 89.6 ms: 1.02x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.3 sec: 1.02x faster                                                          |
| xml_etree_parse            | 113 ms                                                          | 111 ms: 1.02x faster                                                            |
| create_gc_cycles           | 652 us                                                          | 642 us: 1.02x faster                                                            |
| pickle_dict                | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 200 ms: 1.00x slower                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 78.3 ms: 1.01x slower                                                           |
| python_startup             | 22.4 ms                                                         | 22.9 ms: 1.02x slower                                                           |
| json_loads                 | 20.4 us                                                         | 21.0 us: 1.03x slower                                                           |
| sympy_sum                  | 123 ms                                                          | 127 ms: 1.03x slower                                                            |
| typing_runtime_protocols   | 126 us                                                          | 132 us: 1.04x slower                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 592 ms: 1.05x slower                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 578 ms: 1.06x slower                                                            |
| json                       | 4.15 ms                                                         | 4.41 ms: 1.06x slower                                                           |
| nqueens                    | 93.7 ms                                                         | 99.7 ms: 1.06x slower                                                           |
| bench_thread_pool          | 1.10 ms                                                         | 1.18 ms: 1.07x slower                                                           |
| tornado_http               | 105 ms                                                          | 113 ms: 1.07x slower                                                            |
| chaos                      | 69.4 ms                                                         | 74.5 ms: 1.07x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.5 ms: 1.07x slower                                                           |
| meteor_contest             | 86.9 ms                                                         | 93.7 ms: 1.08x slower                                                           |
| docutils                   | 1.98 sec                                                        | 2.15 sec: 1.08x slower                                                          |
| mdp                        | 1.91 sec                                                        | 2.08 sec: 1.09x slower                                                          |
| dask                       | 323 ms                                                          | 353 ms: 1.09x slower                                                            |
| hexiom                     | 6.82 ms                                                         | 7.45 ms: 1.09x slower                                                           |
| sympy_str                  | 240 ms                                                          | 264 ms: 1.10x slower                                                            |
| sympy_integrate            | 17.5 ms                                                         | 19.4 ms: 1.10x slower                                                           |
| logging_format             | 10.4 us                                                         | 11.5 us: 1.11x slower                                                           |
| async_tree_none            | 298 ms                                                          | 330 ms: 1.11x slower                                                            |
| logging_simple             | 9.75 us                                                         | 10.8 us: 1.11x slower                                                           |
| 2to3                       | 280 ms                                                          | 312 ms: 1.11x slower                                                            |
| deltablue                  | 3.58 ms                                                         | 4.01 ms: 1.12x slower                                                           |
| json_dumps                 | 7.40 ms                                                         | 8.30 ms: 1.12x slower                                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 395 ms: 1.13x slower                                                            |
| fannkuch                   | 354 ms                                                          | 399 ms: 1.13x slower                                                            |
| async_tree_io              | 693 ms                                                          | 782 ms: 1.13x slower                                                            |
| async_tree_memoization     | 364 ms                                                          | 412 ms: 1.13x slower                                                            |
| async_tree_io_tg           | 677 ms                                                          | 769 ms: 1.14x slower                                                            |
| async_tree_none_tg         | 278 ms                                                          | 317 ms: 1.14x slower                                                            |
| async_generators           | 313 ms                                                          | 357 ms: 1.14x slower                                                            |
| regex_v8                   | 15.0 ms                                                         | 17.2 ms: 1.14x slower                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 83.0 ms: 1.15x slower                                                           |
| pyflate                    | 424 ms                                                          | 488 ms: 1.15x slower                                                            |
| raytrace                   | 308 ms                                                          | 354 ms: 1.15x slower                                                            |
| regex_compile              | 129 ms                                                          | 149 ms: 1.15x slower                                                            |
| sympy_expand               | 398 ms                                                          | 463 ms: 1.16x slower                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 56.6 ms: 1.17x slower                                                           |
| pycparser                  | 978 ms                                                          | 1.15 sec: 1.18x slower                                                          |
| scimark_monte_carlo        | 66.4 ms                                                         | 79.6 ms: 1.20x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 120 ms: 1.20x slower                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 3.89 us: 1.21x slower                                                           |
| xml_etree_process          | 53.2 ms                                                         | 64.6 ms: 1.21x slower                                                           |
| deepcopy                   | 360 us                                                          | 443 us: 1.23x slower                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.93 ms: 1.26x slower                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.90 sec: 1.27x slower                                                          |
| chameleon                  | 7.75 ms                                                         | 9.94 ms: 1.28x slower                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 1.60 ms: 1.28x slower                                                           |
| telco                      | 5.51 ms                                                         | 7.09 ms: 1.29x slower                                                           |
| pprint_safe_repr           | 721 ms                                                          | 936 ms: 1.30x slower                                                            |
| deepcopy_memo              | 38.4 us                                                         | 50.7 us: 1.32x slower                                                           |
| go                         | 137 ms                                                          | 185 ms: 1.34x slower                                                            |
| pickle_pure_python         | 286 us                                                          | 385 us: 1.35x slower                                                            |
| scimark_lu                 | 93.2 ms                                                         | 133 ms: 1.43x slower                                                            |
| scimark_sor                | 130 ms                                                          | 186 ms: 1.43x slower                                                            |
| unpickle_pure_python       | 210 us                                                          | 304 us: 1.45x slower                                                            |
| richards_super             | 46.5 ms                                                         | 67.7 ms: 1.46x slower                                                           |
| generators                 | 38.5 ms                                                         | 56.9 ms: 1.48x slower                                                           |
| richards                   | 41.3 ms                                                         | 61.5 ms: 1.49x slower                                                           |
| coroutines                 | 20.9 ms                                                         | 31.9 ms: 1.53x slower                                                           |
| logging_silent             | 101 ns                                                          | 156 ns: 1.54x slower                                                            |
| unpack_sequence            | 62.5 ns                                                         | 97.7 ns: 1.56x slower                                                           |
| coverage                   | 48.4 ms                                                         | 774 ms: 15.98x slower                                                           |
| Geometric mean             | (ref)                                                           | 1.14x slower                                                                    |

Benchmark hidden because not significant (3): unpickle, tomli_loads, asyncio_tcp
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.08x
- 95% likely to have a slowdown of 1.08x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: unknown