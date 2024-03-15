# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-x86
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.17x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 264 ms: 1.07x faster                                                          |
| chameleon      | 8.08 ms                                                         | 5.90 ms: 1.37x faster                                                         |
| docutils       | 2.10 sec                                                        | 1.89 sec: 1.11x faster                                                        |
| tornado_http   | 118 ms                                                          | 99.4 ms: 1.19x faster                                                         |
| Geometric mean | (ref)                                                           | 1.18x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 268 ms: 1.28x faster                                                          |
| async_tree_memoization     | 408 ms                                                          | 332 ms: 1.23x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 618 ms: 1.21x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 251 ms: 1.20x faster                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 315 ms: 1.20x faster                                                          |
| async_tree_io              | 754 ms                                                          | 637 ms: 1.18x faster                                                          |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 541 ms: 1.07x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 556 ms: 1.06x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.18x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 55.2 ms: 1.38x faster                                                         |
| nbody          | 126 ms                                                          | 97.7 ms: 1.29x faster                                                         |
| pidigits       | 203 ms                                                          | 200 ms: 1.01x faster                                                          |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 114 ms: 1.30x faster                                                          |
| regex_dna      | 122 ms                                                          | 119 ms: 1.02x faster                                                          |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.03x slower                                                         |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 7.16 ms: 1.37x faster                                                         |
| pickle_pure_python   | 309 us                                                          | 227 us: 1.36x faster                                                          |
| unpickle_pure_python | 231 us                                                          | 174 us: 1.33x faster                                                          |
| tomli_loads          | 2.31 sec                                                        | 1.75 sec: 1.33x faster                                                        |
| xml_etree_process    | 55.0 ms                                                         | 44.3 ms: 1.24x faster                                                         |
| unpickle_list        | 3.28 us                                                         | 2.79 us: 1.17x faster                                                         |
| xml_etree_iterparse  | 75.6 ms                                                         | 66.9 ms: 1.13x faster                                                         |
| xml_etree_generate   | 71.6 ms                                                         | 63.8 ms: 1.12x faster                                                         |
| xml_etree_parse      | 114 ms                                                          | 108 ms: 1.06x faster                                                          |
| pickle               | 7.99 us                                                         | 7.91 us: 1.01x faster                                                         |
| pickle_list          | 3.27 us                                                         | 3.29 us: 1.01x slower                                                         |
| json_loads           | 20.0 us                                                         | 20.4 us: 1.02x slower                                                         |
| unpickle             | 9.23 us                                                         | 10.0 us: 1.08x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                  |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 26.0 ms: 1.18x slower                                                         |
| python_startup_no_site | 18.8 ms                                                         | 23.7 ms: 1.26x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.22x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.24 ms: 1.42x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 97.1 us: 4.92x faster                                                         |
| generators                 | 52.2 ms                                                         | 25.0 ms: 2.09x faster                                                         |
| logging_silent             | 119 ns                                                          | 70.3 ns: 1.69x faster                                                         |
| spectral_norm              | 122 ms                                                          | 73.3 ms: 1.66x faster                                                         |
| coroutines                 | 23.7 ms                                                         | 15.1 ms: 1.57x faster                                                         |
| deltablue                  | 4.10 ms                                                         | 2.74 ms: 1.49x faster                                                         |
| unpack_sequence            | 65.2 ns                                                         | 43.7 ns: 1.49x faster                                                         |
| comprehensions             | 22.1 us                                                         | 15.3 us: 1.44x faster                                                         |
| deepcopy_memo              | 40.0 us                                                         | 27.9 us: 1.43x faster                                                         |
| chaos                      | 84.4 ms                                                         | 58.9 ms: 1.43x faster                                                         |
| sqlglot_parse              | 1.49 ms                                                         | 1.04 ms: 1.43x faster                                                         |
| mako                       | 10.3 ms                                                         | 7.24 ms: 1.42x faster                                                         |
| richards_super             | 58.7 ms                                                         | 41.7 ms: 1.41x faster                                                         |
| float                      | 76.1 ms                                                         | 55.2 ms: 1.38x faster                                                         |
| sympy_sum                  | 149 ms                                                          | 109 ms: 1.37x faster                                                          |
| json_dumps                 | 9.80 ms                                                         | 7.16 ms: 1.37x faster                                                         |
| chameleon                  | 8.08 ms                                                         | 5.90 ms: 1.37x faster                                                         |
| sqlglot_transpile          | 1.78 ms                                                         | 1.31 ms: 1.37x faster                                                         |
| pickle_pure_python         | 309 us                                                          | 227 us: 1.36x faster                                                          |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.11 ms: 1.36x faster                                                         |
| sympy_str                  | 283 ms                                                          | 213 ms: 1.33x faster                                                          |
| unpickle_pure_python       | 231 us                                                          | 174 us: 1.33x faster                                                          |
| tomli_loads                | 2.31 sec                                                        | 1.75 sec: 1.33x faster                                                        |
| richards                   | 48.8 ms                                                         | 37.1 ms: 1.32x faster                                                         |
| crypto_pyaes               | 79.4 ms                                                         | 61.1 ms: 1.30x faster                                                         |
| regex_compile              | 148 ms                                                          | 114 ms: 1.30x faster                                                          |
| deepcopy                   | 381 us                                                          | 294 us: 1.30x faster                                                          |
| logging_simple             | 10.8 us                                                         | 8.33 us: 1.30x faster                                                         |
| logging_format             | 11.5 us                                                         | 8.87 us: 1.29x faster                                                         |
| nbody                      | 126 ms                                                          | 97.7 ms: 1.29x faster                                                         |
| async_tree_none            | 343 ms                                                          | 268 ms: 1.28x faster                                                          |
| deepcopy_reduce            | 3.32 us                                                         | 2.61 us: 1.27x faster                                                         |
| scimark_sor                | 135 ms                                                          | 108 ms: 1.25x faster                                                          |
| sympy_integrate            | 19.9 ms                                                         | 15.9 ms: 1.25x faster                                                         |
| asyncio_tcp                | 787 ms                                                          | 632 ms: 1.24x faster                                                          |
| sympy_expand               | 462 ms                                                          | 372 ms: 1.24x faster                                                          |
| xml_etree_process          | 55.0 ms                                                         | 44.3 ms: 1.24x faster                                                         |
| async_tree_memoization     | 408 ms                                                          | 332 ms: 1.23x faster                                                          |
| scimark_fft                | 291 ms                                                          | 239 ms: 1.22x faster                                                          |
| nqueens                    | 111 ms                                                          | 91.7 ms: 1.22x faster                                                         |
| pyflate                    | 471 ms                                                          | 388 ms: 1.21x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 618 ms: 1.21x faster                                                          |
| fannkuch                   | 399 ms                                                          | 332 ms: 1.20x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 251 ms: 1.20x faster                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 315 ms: 1.20x faster                                                          |
| tornado_http               | 118 ms                                                          | 99.4 ms: 1.19x faster                                                         |
| hexiom                     | 7.51 ms                                                         | 6.32 ms: 1.19x faster                                                         |
| pycparser                  | 1.04 sec                                                        | 878 ms: 1.19x faster                                                          |
| async_tree_io              | 754 ms                                                          | 637 ms: 1.18x faster                                                          |
| raytrace                   | 327 ms                                                          | 277 ms: 1.18x faster                                                          |
| scimark_lu                 | 102 ms                                                          | 87.2 ms: 1.17x faster                                                         |
| unpickle_list              | 3.28 us                                                         | 2.79 us: 1.17x faster                                                         |
| json                       | 4.78 ms                                                         | 4.13 ms: 1.16x faster                                                         |
| sqlite_synth               | 2.15 us                                                         | 1.86 us: 1.15x faster                                                         |
| mdp                        | 2.07 sec                                                        | 1.80 sec: 1.15x faster                                                        |
| go                         | 147 ms                                                          | 128 ms: 1.15x faster                                                          |
| xml_etree_iterparse        | 75.6 ms                                                         | 66.9 ms: 1.13x faster                                                         |
| pprint_pformat             | 1.70 sec                                                        | 1.50 sec: 1.13x faster                                                        |
| xml_etree_generate         | 71.6 ms                                                         | 63.8 ms: 1.12x faster                                                         |
| pprint_safe_repr           | 819 ms                                                          | 735 ms: 1.11x faster                                                          |
| docutils                   | 2.10 sec                                                        | 1.89 sec: 1.11x faster                                                        |
| sqlglot_optimize           | 51.8 ms                                                         | 47.4 ms: 1.09x faster                                                         |
| meteor_contest             | 90.9 ms                                                         | 83.5 ms: 1.09x faster                                                         |
| scimark_monte_carlo        | 70.8 ms                                                         | 65.7 ms: 1.08x faster                                                         |
| bench_thread_pool          | 1.14 ms                                                         | 1.06 ms: 1.07x faster                                                         |
| 2to3                       | 282 ms                                                          | 264 ms: 1.07x faster                                                          |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 541 ms: 1.07x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 556 ms: 1.06x faster                                                          |
| xml_etree_parse            | 114 ms                                                          | 108 ms: 1.06x faster                                                          |
| regex_dna                  | 122 ms                                                          | 119 ms: 1.02x faster                                                          |
| pidigits                   | 203 ms                                                          | 200 ms: 1.01x faster                                                          |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.01x faster                                                        |
| pickle                     | 7.99 us                                                         | 7.91 us: 1.01x faster                                                         |
| pickle_list                | 3.27 us                                                         | 3.29 us: 1.01x slower                                                         |
| gc_traversal               | 1.38 ms                                                         | 1.40 ms: 1.02x slower                                                         |
| json_loads                 | 20.0 us                                                         | 20.4 us: 1.02x slower                                                         |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.03x slower                                                         |
| bench_mp_pool              | 70.9 ms                                                         | 74.5 ms: 1.05x slower                                                         |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                         |
| create_gc_cycles           | 618 us                                                          | 653 us: 1.06x slower                                                          |
| pathlib                    | 79.9 ms                                                         | 84.6 ms: 1.06x slower                                                         |
| unpickle                   | 9.23 us                                                         | 10.0 us: 1.08x slower                                                         |
| telco                      | 5.29 ms                                                         | 6.18 ms: 1.17x slower                                                         |
| python_startup             | 22.0 ms                                                         | 26.0 ms: 1.18x slower                                                         |
| async_generators           | 260 ms                                                          | 316 ms: 1.21x slower                                                          |
| python_startup_no_site     | 18.8 ms                                                         | 23.7 ms: 1.26x slower                                                         |
| sqlglot_normalize          | 113 ms                                                          | 235 ms: 2.08x slower                                                          |
| coverage                   | 58.0 ms                                                         | 330 ms: 5.68x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                  |

Benchmark hidden because not significant (1): pickle_dict
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown