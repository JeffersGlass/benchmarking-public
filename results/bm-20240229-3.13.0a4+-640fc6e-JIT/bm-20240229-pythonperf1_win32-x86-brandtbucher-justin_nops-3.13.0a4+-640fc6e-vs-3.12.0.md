# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_nops
- machine: windows-x86
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 259 ms: 1.08x faster                                                         |
| chameleon      | 7.75 ms                                                         | 5.58 ms: 1.39x faster                                                        |
| docutils       | 1.98 sec                                                        | 1.79 sec: 1.11x faster                                                       |
| tornado_http   | 105 ms                                                          | 96.1 ms: 1.09x faster                                                        |
| Geometric mean | (ref)                                                           | 1.16x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 350 ms                                                          | 306 ms: 1.15x faster                                                         |
| async_tree_none            | 298 ms                                                          | 261 ms: 1.14x faster                                                         |
| async_tree_memoization     | 364 ms                                                          | 324 ms: 1.12x faster                                                         |
| async_tree_none_tg         | 278 ms                                                          | 249 ms: 1.11x faster                                                         |
| async_tree_io_tg           | 677 ms                                                          | 611 ms: 1.11x faster                                                         |
| async_tree_io              | 693 ms                                                          | 630 ms: 1.10x faster                                                         |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 525 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 509 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 55.0 ms: 1.39x faster                                                        |
| nbody          | 127 ms                                                          | 92.6 ms: 1.37x faster                                                        |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 107 ms: 1.20x faster                                                         |
| regex_effbot   | 2.04 ms                                                         | 1.87 ms: 1.09x faster                                                        |
| regex_dna      | 127 ms                                                          | 118 ms: 1.08x faster                                                         |
| regex_v8       | 15.0 ms                                                         | 15.9 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 286 us                                                          | 208 us: 1.37x faster                                                         |
| tomli_loads          | 2.20 sec                                                        | 1.68 sec: 1.31x faster                                                       |
| xml_etree_process    | 53.2 ms                                                         | 42.5 ms: 1.25x faster                                                        |
| unpickle_pure_python | 210 us                                                          | 168 us: 1.25x faster                                                         |
| xml_etree_generate   | 72.1 ms                                                         | 61.8 ms: 1.17x faster                                                        |
| xml_etree_iterparse  | 77.6 ms                                                         | 67.2 ms: 1.16x faster                                                        |
| json_dumps           | 7.40 ms                                                         | 7.05 ms: 1.05x faster                                                        |
| pickle_list          | 3.37 us                                                         | 3.23 us: 1.04x faster                                                        |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                         |
| json_loads           | 20.4 us                                                         | 19.9 us: 1.02x faster                                                        |
| unpickle_list        | 2.95 us                                                         | 2.91 us: 1.01x faster                                                        |
| pickle               | 7.79 us                                                         | 7.91 us: 1.02x slower                                                        |
| pickle_dict          | 19.9 us                                                         | 20.4 us: 1.02x slower                                                        |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 26.9 ms: 1.20x slower                                                        |
| python_startup_no_site | 19.1 ms                                                         | 24.4 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                           | 1.24x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 9.96 ms                                                         | 7.19 ms: 1.39x faster                                                        |
| django_template | 36.9 ms                                                         | 30.2 ms: 1.22x faster                                                        |
| Geometric mean  | (ref)                                                           | 1.30x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.2 ms: 1.73x faster                                                        |
| logging_silent             | 101 ns                                                          | 59.6 ns: 1.69x faster                                                        |
| deepcopy_memo              | 38.4 us                                                         | 23.8 us: 1.61x faster                                                        |
| coroutines                 | 20.9 ms                                                         | 14.2 ms: 1.47x faster                                                        |
| unpack_sequence            | 62.5 ns                                                         | 43.7 ns: 1.43x faster                                                        |
| deltablue                  | 3.58 ms                                                         | 2.55 ms: 1.41x faster                                                        |
| float                      | 76.7 ms                                                         | 55.0 ms: 1.39x faster                                                        |
| chameleon                  | 7.75 ms                                                         | 5.58 ms: 1.39x faster                                                        |
| mako                       | 9.96 ms                                                         | 7.19 ms: 1.39x faster                                                        |
| pickle_pure_python         | 286 us                                                          | 208 us: 1.37x faster                                                         |
| nbody                      | 127 ms                                                          | 92.6 ms: 1.37x faster                                                        |
| comprehensions             | 19.2 us                                                         | 14.1 us: 1.36x faster                                                        |
| deepcopy_reduce            | 3.23 us                                                         | 2.38 us: 1.36x faster                                                        |
| spectral_norm              | 104 ms                                                          | 77.2 ms: 1.35x faster                                                        |
| typing_runtime_protocols   | 126 us                                                          | 94.0 us: 1.34x faster                                                        |
| tomli_loads                | 2.20 sec                                                        | 1.68 sec: 1.31x faster                                                       |
| deepcopy                   | 360 us                                                          | 277 us: 1.30x faster                                                         |
| scimark_sor                | 130 ms                                                          | 100 ms: 1.30x faster                                                         |
| sqlglot_parse              | 1.25 ms                                                         | 976 us: 1.28x faster                                                         |
| sqlglot_transpile          | 1.53 ms                                                         | 1.21 ms: 1.26x faster                                                        |
| xml_etree_process          | 53.2 ms                                                         | 42.5 ms: 1.25x faster                                                        |
| unpickle_pure_python       | 210 us                                                          | 168 us: 1.25x faster                                                         |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.14 ms: 1.23x faster                                                        |
| django_template            | 36.9 ms                                                         | 30.2 ms: 1.22x faster                                                        |
| logging_simple             | 9.75 us                                                         | 8.07 us: 1.21x faster                                                        |
| logging_format             | 10.4 us                                                         | 8.63 us: 1.21x faster                                                        |
| regex_compile              | 129 ms                                                          | 107 ms: 1.20x faster                                                         |
| crypto_pyaes               | 69.2 ms                                                         | 58.6 ms: 1.18x faster                                                        |
| chaos                      | 69.4 ms                                                         | 58.8 ms: 1.18x faster                                                        |
| raytrace                   | 308 ms                                                          | 263 ms: 1.17x faster                                                         |
| xml_etree_generate         | 72.1 ms                                                         | 61.8 ms: 1.17x faster                                                        |
| xml_etree_iterparse        | 77.6 ms                                                         | 67.2 ms: 1.16x faster                                                        |
| scimark_fft                | 271 ms                                                          | 235 ms: 1.15x faster                                                         |
| richards                   | 41.3 ms                                                         | 35.8 ms: 1.15x faster                                                        |
| richards_super             | 46.5 ms                                                         | 40.3 ms: 1.15x faster                                                        |
| sympy_sum                  | 123 ms                                                          | 107 ms: 1.15x faster                                                         |
| sympy_str                  | 240 ms                                                          | 209 ms: 1.15x faster                                                         |
| async_tree_memoization_tg  | 350 ms                                                          | 306 ms: 1.15x faster                                                         |
| go                         | 137 ms                                                          | 120 ms: 1.14x faster                                                         |
| async_tree_none            | 298 ms                                                          | 261 ms: 1.14x faster                                                         |
| pycparser                  | 978 ms                                                          | 857 ms: 1.14x faster                                                         |
| sympy_integrate            | 17.5 ms                                                         | 15.4 ms: 1.14x faster                                                        |
| scimark_lu                 | 93.2 ms                                                         | 82.3 ms: 1.13x faster                                                        |
| async_tree_memoization     | 364 ms                                                          | 324 ms: 1.12x faster                                                         |
| async_tree_none_tg         | 278 ms                                                          | 249 ms: 1.11x faster                                                         |
| async_tree_io_tg           | 677 ms                                                          | 611 ms: 1.11x faster                                                         |
| pyflate                    | 424 ms                                                          | 383 ms: 1.11x faster                                                         |
| docutils                   | 1.98 sec                                                        | 1.79 sec: 1.11x faster                                                       |
| async_generators           | 313 ms                                                          | 283 ms: 1.11x faster                                                         |
| async_tree_io              | 693 ms                                                          | 630 ms: 1.10x faster                                                         |
| hexiom                     | 6.82 ms                                                         | 6.20 ms: 1.10x faster                                                        |
| mdp                        | 1.91 sec                                                        | 1.74 sec: 1.10x faster                                                       |
| tornado_http               | 105 ms                                                          | 96.1 ms: 1.09x faster                                                        |
| sympy_expand               | 398 ms                                                          | 364 ms: 1.09x faster                                                         |
| regex_effbot               | 2.04 ms                                                         | 1.87 ms: 1.09x faster                                                        |
| pathlib                    | 91.4 ms                                                         | 84.2 ms: 1.09x faster                                                        |
| 2to3                       | 280 ms                                                          | 259 ms: 1.08x faster                                                         |
| regex_dna                  | 127 ms                                                          | 118 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 525 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 509 ms: 1.07x faster                                                         |
| bench_thread_pool          | 1.10 ms                                                         | 1.03 ms: 1.07x faster                                                        |
| sqlglot_optimize           | 48.5 ms                                                         | 45.5 ms: 1.07x faster                                                        |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                       |
| sqlite_synth               | 2.07 us                                                         | 1.97 us: 1.05x faster                                                        |
| json_dumps                 | 7.40 ms                                                         | 7.05 ms: 1.05x faster                                                        |
| fannkuch                   | 354 ms                                                          | 339 ms: 1.04x faster                                                         |
| pickle_list                | 3.37 us                                                         | 3.23 us: 1.04x faster                                                        |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                         |
| meteor_contest             | 86.9 ms                                                         | 84.5 ms: 1.03x faster                                                        |
| gc_traversal               | 1.44 ms                                                         | 1.41 ms: 1.02x faster                                                        |
| json_loads                 | 20.4 us                                                         | 19.9 us: 1.02x faster                                                        |
| scimark_monte_carlo        | 66.4 ms                                                         | 65.1 ms: 1.02x faster                                                        |
| nqueens                    | 93.7 ms                                                         | 91.9 ms: 1.02x faster                                                        |
| unpickle_list              | 2.95 us                                                         | 2.91 us: 1.01x faster                                                        |
| pprint_pformat             | 1.50 sec                                                        | 1.49 sec: 1.01x faster                                                       |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                         |
| json                       | 4.15 ms                                                         | 4.19 ms: 1.01x slower                                                        |
| pickle                     | 7.79 us                                                         | 7.91 us: 1.02x slower                                                        |
| create_gc_cycles           | 652 us                                                          | 663 us: 1.02x slower                                                         |
| pprint_safe_repr           | 721 ms                                                          | 733 ms: 1.02x slower                                                         |
| pickle_dict                | 19.9 us                                                         | 20.4 us: 1.02x slower                                                        |
| bench_mp_pool              | 75.4 ms                                                         | 77.5 ms: 1.03x slower                                                        |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                                        |
| regex_v8                   | 15.0 ms                                                         | 15.9 ms: 1.06x slower                                                        |
| telco                      | 5.51 ms                                                         | 6.34 ms: 1.15x slower                                                        |
| python_startup             | 22.4 ms                                                         | 26.9 ms: 1.20x slower                                                        |
| python_startup_no_site     | 19.1 ms                                                         | 24.4 ms: 1.28x slower                                                        |
| dask                       | 323 ms                                                          | 418 ms: 1.29x slower                                                         |
| sqlglot_normalize          | 100 ms                                                          | 223 ms: 2.22x slower                                                         |
| coverage                   | 48.4 ms                                                         | 490 ms: 10.11x slower                                                        |
| Geometric mean             | (ref)                                                           | 1.10x faster                                                                 |

Benchmark hidden because not significant (1): asyncio_tcp
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown