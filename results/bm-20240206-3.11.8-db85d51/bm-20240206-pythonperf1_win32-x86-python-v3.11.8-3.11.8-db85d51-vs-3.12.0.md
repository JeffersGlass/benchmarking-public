
# Results vs. 3.12.0

- fork: python
- ref: v3.11.8
- machine: windows-x86
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 277 ms: 1.01x faster                                            |
| chameleon      | 7.75 ms                                                         | 8.27 ms: 1.07x slower                                           |
| docutils       | 1.98 sec                                                        | 2.00 sec: 1.01x slower                                          |
| tornado_http   | 105 ms                                                          | 114 ms: 1.09x slower                                            |
| Geometric mean | (ref)                                                           | 1.04x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io_tg           | 677 ms                                                          | 699 ms: 1.03x slower                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 565 ms: 1.03x slower                                            |
| async_tree_none_tg         | 278 ms                                                          | 291 ms: 1.05x slower                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 372 ms: 1.06x slower                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 600 ms: 1.06x slower                                            |
| async_tree_io              | 693 ms                                                          | 740 ms: 1.07x slower                                            |
| async_tree_memoization     | 364 ms                                                          | 392 ms: 1.08x slower                                            |
| async_tree_none            | 298 ms                                                          | 329 ms: 1.11x slower                                            |
| Geometric mean             | (ref)                                                           | 1.06x slower                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 117 ms: 1.09x faster                                            |
| float          | 76.7 ms                                                         | 71.6 ms: 1.07x faster                                           |
| pidigits       | 199 ms                                                          | 197 ms: 1.01x faster                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 2.04 ms                                                         | 1.85 ms: 1.10x faster                                           |
| regex_dna      | 127 ms                                                          | 117 ms: 1.09x faster                                            |
| regex_v8       | 15.0 ms                                                         | 15.3 ms: 1.02x slower                                           |
| regex_compile  | 129 ms                                                          | 140 ms: 1.09x slower                                            |
| Geometric mean | (ref)                                                           | 1.02x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpickle_list        | 2.95 us                                                         | 2.57 us: 1.15x faster                                           |
| unpickle             | 9.71 us                                                         | 9.04 us: 1.07x faster                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 73.4 ms: 1.06x faster                                           |
| xml_etree_generate   | 72.1 ms                                                         | 68.5 ms: 1.05x faster                                           |
| pickle_list          | 3.37 us                                                         | 3.20 us: 1.05x faster                                           |
| pickle               | 7.79 us                                                         | 7.53 us: 1.03x faster                                           |
| xml_etree_process    | 53.2 ms                                                         | 52.1 ms: 1.02x faster                                           |
| json_loads           | 20.4 us                                                         | 20.1 us: 1.01x faster                                           |
| pickle_dict          | 19.9 us                                                         | 20.0 us: 1.00x slower                                           |
| tomli_loads          | 2.20 sec                                                        | 2.24 sec: 1.02x slower                                          |
| pickle_pure_python   | 286 us                                                          | 299 us: 1.05x slower                                            |
| unpickle_pure_python | 210 us                                                          | 230 us: 1.10x slower                                            |
| json_dumps           | 7.40 ms                                                         | 9.80 ms: 1.32x slower                                           |
| Geometric mean       | (ref)                                                           | 1.00x slower                                                    |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 19.1 ms                                                         | 17.9 ms: 1.07x faster                                           |
| python_startup         | 22.4 ms                                                         | 21.4 ms: 1.05x faster                                           |
| Geometric mean         | (ref)                                                           | 1.06x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 9.96 ms                                                         | 9.58 ms: 1.04x faster                                           |
| django_template | 36.9 ms                                                         | 37.6 ms: 1.02x slower                                           |
| Geometric mean  | (ref)                                                           | 1.01x faster                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_generators           | 313 ms                                                          | 238 ms: 1.31x faster                                            |
| pathlib                    | 91.4 ms                                                         | 74.7 ms: 1.22x faster                                           |
| unpickle_list              | 2.95 us                                                         | 2.57 us: 1.15x faster                                           |
| regex_effbot               | 2.04 ms                                                         | 1.85 ms: 1.10x faster                                           |
| telco                      | 5.51 ms                                                         | 5.06 ms: 1.09x faster                                           |
| regex_dna                  | 127 ms                                                          | 117 ms: 1.09x faster                                            |
| nbody                      | 127 ms                                                          | 117 ms: 1.09x faster                                            |
| create_gc_cycles           | 652 us                                                          | 605 us: 1.08x faster                                            |
| unpickle                   | 9.71 us                                                         | 9.04 us: 1.07x faster                                           |
| float                      | 76.7 ms                                                         | 71.6 ms: 1.07x faster                                           |
| unpack_sequence            | 62.5 ns                                                         | 58.6 ns: 1.07x faster                                           |
| python_startup_no_site     | 19.1 ms                                                         | 17.9 ms: 1.07x faster                                           |
| gc_traversal               | 1.44 ms                                                         | 1.35 ms: 1.07x faster                                           |
| xml_etree_iterparse        | 77.6 ms                                                         | 73.4 ms: 1.06x faster                                           |
| xml_etree_generate         | 72.1 ms                                                         | 68.5 ms: 1.05x faster                                           |
| pickle_list                | 3.37 us                                                         | 3.20 us: 1.05x faster                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                          |
| python_startup             | 22.4 ms                                                         | 21.4 ms: 1.05x faster                                           |
| mako                       | 9.96 ms                                                         | 9.58 ms: 1.04x faster                                           |
| bench_mp_pool              | 75.4 ms                                                         | 72.8 ms: 1.04x faster                                           |
| pickle                     | 7.79 us                                                         | 7.53 us: 1.03x faster                                           |
| scimark_sor                | 130 ms                                                          | 127 ms: 1.02x faster                                            |
| xml_etree_process          | 53.2 ms                                                         | 52.1 ms: 1.02x faster                                           |
| json_loads                 | 20.4 us                                                         | 20.1 us: 1.01x faster                                           |
| pidigits                   | 199 ms                                                          | 197 ms: 1.01x faster                                            |
| 2to3                       | 280 ms                                                          | 277 ms: 1.01x faster                                            |
| sqlite_synth               | 2.07 us                                                         | 2.06 us: 1.01x faster                                           |
| pickle_dict                | 19.9 us                                                         | 20.0 us: 1.00x slower                                           |
| docutils                   | 1.98 sec                                                        | 2.00 sec: 1.01x slower                                          |
| deepcopy_reduce            | 3.23 us                                                         | 3.27 us: 1.01x slower                                           |
| regex_v8                   | 15.0 ms                                                         | 15.3 ms: 1.02x slower                                           |
| tomli_loads                | 2.20 sec                                                        | 2.24 sec: 1.02x slower                                          |
| django_template            | 36.9 ms                                                         | 37.6 ms: 1.02x slower                                           |
| bench_thread_pool          | 1.10 ms                                                         | 1.13 ms: 1.02x slower                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 49.9 ms: 1.03x slower                                           |
| async_tree_io_tg           | 677 ms                                                          | 699 ms: 1.03x slower                                            |
| raytrace                   | 308 ms                                                          | 318 ms: 1.03x slower                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 565 ms: 1.03x slower                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 4.01 ms: 1.04x slower                                           |
| dulwich_log                | 58.5 ms                                                         | 60.7 ms: 1.04x slower                                           |
| deepcopy                   | 360 us                                                          | 375 us: 1.04x slower                                            |
| aiohttp                    | 1.06 ms                                                         | 1.10 ms: 1.04x slower                                           |
| pickle_pure_python         | 286 us                                                          | 299 us: 1.05x slower                                            |
| scimark_lu                 | 93.2 ms                                                         | 97.6 ms: 1.05x slower                                           |
| async_tree_none_tg         | 278 ms                                                          | 291 ms: 1.05x slower                                            |
| scimark_monte_carlo        | 66.4 ms                                                         | 70.1 ms: 1.05x slower                                           |
| mypy2                      | 584 ms                                                          | 616 ms: 1.05x slower                                            |
| pycparser                  | 978 ms                                                          | 1.03 sec: 1.06x slower                                          |
| hexiom                     | 6.82 ms                                                         | 7.22 ms: 1.06x slower                                           |
| meteor_contest             | 86.9 ms                                                         | 92.1 ms: 1.06x slower                                           |
| crypto_pyaes               | 69.2 ms                                                         | 73.4 ms: 1.06x slower                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 372 ms: 1.06x slower                                            |
| scimark_fft                | 271 ms                                                          | 288 ms: 1.06x slower                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 600 ms: 1.06x slower                                            |
| dask                       | 323 ms                                                          | 345 ms: 1.07x slower                                            |
| logging_format             | 10.4 us                                                         | 11.1 us: 1.07x slower                                           |
| async_tree_io              | 693 ms                                                          | 740 ms: 1.07x slower                                            |
| chameleon                  | 7.75 ms                                                         | 8.27 ms: 1.07x slower                                           |
| sqlglot_normalize          | 100 ms                                                          | 107 ms: 1.07x slower                                            |
| logging_simple             | 9.75 us                                                         | 10.5 us: 1.07x slower                                           |
| async_tree_memoization     | 364 ms                                                          | 392 ms: 1.08x slower                                            |
| sqlalchemy_declarative     | 103 ms                                                          | 111 ms: 1.08x slower                                            |
| regex_compile              | 129 ms                                                          | 140 ms: 1.09x slower                                            |
| tornado_http               | 105 ms                                                          | 114 ms: 1.09x slower                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.63 sec: 1.09x slower                                          |
| pprint_safe_repr           | 721 ms                                                          | 787 ms: 1.09x slower                                            |
| go                         | 137 ms                                                          | 150 ms: 1.09x slower                                            |
| deltablue                  | 3.58 ms                                                         | 3.93 ms: 1.10x slower                                           |
| unpickle_pure_python       | 210 us                                                          | 230 us: 1.10x slower                                            |
| coroutines                 | 20.9 ms                                                         | 22.9 ms: 1.10x slower                                           |
| richards                   | 41.3 ms                                                         | 45.5 ms: 1.10x slower                                           |
| async_tree_none            | 298 ms                                                          | 329 ms: 1.11x slower                                            |
| sympy_integrate            | 17.5 ms                                                         | 19.4 ms: 1.11x slower                                           |
| comprehensions             | 19.2 us                                                         | 21.3 us: 1.11x slower                                           |
| asyncio_tcp                | 662 ms                                                          | 738 ms: 1.11x slower                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.71 ms: 1.11x slower                                           |
| logging_silent             | 101 ns                                                          | 114 ns: 1.13x slower                                            |
| spectral_norm              | 104 ms                                                          | 118 ms: 1.14x slower                                            |
| mdp                        | 1.91 sec                                                        | 2.18 sec: 1.14x slower                                          |
| sympy_expand               | 398 ms                                                          | 455 ms: 1.14x slower                                            |
| sympy_str                  | 240 ms                                                          | 274 ms: 1.15x slower                                            |
| sqlglot_parse              | 1.25 ms                                                         | 1.44 ms: 1.15x slower                                           |
| nqueens                    | 93.7 ms                                                         | 108 ms: 1.16x slower                                            |
| fannkuch                   | 354 ms                                                          | 413 ms: 1.17x slower                                            |
| sympy_sum                  | 123 ms                                                          | 146 ms: 1.19x slower                                            |
| richards_super             | 46.5 ms                                                         | 56.2 ms: 1.21x slower                                           |
| sqlalchemy_imperative      | 12.3 ms                                                         | 14.9 ms: 1.21x slower                                           |
| chaos                      | 69.4 ms                                                         | 84.1 ms: 1.21x slower                                           |
| coverage                   | 48.4 ms                                                         | 59.0 ms: 1.22x slower                                           |
| generators                 | 38.5 ms                                                         | 49.4 ms: 1.28x slower                                           |
| json_dumps                 | 7.40 ms                                                         | 9.80 ms: 1.32x slower                                           |
| typing_runtime_protocols   | 126 us                                                          | 469 us: 3.71x slower                                            |
| Geometric mean             | (ref)                                                           | 1.05x slower                                                    |

Benchmark hidden because not significant (4): xml_etree_parse, pyflate, deepcopy_memo, json
Ignored benchmarks (6) of results/bm-20240206-3.11.8-db85d51/bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: unknown