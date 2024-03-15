# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_arena
- machine: windows-x86
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 260 ms: 1.08x faster                                                          |
| chameleon      | 8.08 ms                                                         | 5.71 ms: 1.41x faster                                                         |
| docutils       | 2.10 sec                                                        | 1.80 sec: 1.17x faster                                                        |
| html5lib       | 54.3 ms                                                         | 45.3 ms: 1.20x faster                                                         |
| tornado_http   | 118 ms                                                          | 95.9 ms: 1.23x faster                                                         |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 257 ms: 1.34x faster                                                          |
| async_tree_memoization     | 408 ms                                                          | 320 ms: 1.28x faster                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 303 ms: 1.25x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 242 ms: 1.24x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 605 ms: 1.23x faster                                                          |
| async_tree_io              | 754 ms                                                          | 621 ms: 1.21x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 518 ms: 1.14x faster                                                          |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 509 ms: 1.13x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 55.1 ms: 1.38x faster                                                         |
| nbody          | 126 ms                                                          | 96.5 ms: 1.30x faster                                                         |
| pidigits       | 203 ms                                                          | 198 ms: 1.03x faster                                                          |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 107 ms: 1.38x faster                                                          |
| regex_dna      | 122 ms                                                          | 116 ms: 1.05x faster                                                          |
| regex_effbot   | 1.82 ms                                                         | 1.88 ms: 1.03x slower                                                         |
| regex_v8       | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_pure_python   | 309 us                                                          | 209 us: 1.48x faster                                                          |
| json_dumps           | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                         |
| tomli_loads          | 2.31 sec                                                        | 1.70 sec: 1.36x faster                                                        |
| unpickle_pure_python | 231 us                                                          | 171 us: 1.35x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                                         |
| unpickle_list        | 3.28 us                                                         | 2.82 us: 1.16x faster                                                         |
| xml_etree_generate   | 71.6 ms                                                         | 62.5 ms: 1.15x faster                                                         |
| xml_etree_iterparse  | 75.6 ms                                                         | 66.5 ms: 1.14x faster                                                         |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                          |
| pickle               | 7.99 us                                                         | 7.89 us: 1.01x faster                                                         |
| pickle_list          | 3.27 us                                                         | 3.23 us: 1.01x faster                                                         |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                                         |
| json_loads           | 20.0 us                                                         | 19.8 us: 1.01x faster                                                         |
| unpickle             | 9.23 us                                                         | 10.0 us: 1.08x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.16x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 25.7 ms: 1.17x slower                                                         |
| python_startup_no_site | 18.8 ms                                                         | 23.6 ms: 1.25x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.21x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako            | 10.3 ms                                                         | 7.12 ms: 1.44x faster                                                         |
| django_template | 37.4 ms                                                         | 29.9 ms: 1.25x faster                                                         |
| genshi_xml      | 61.2 ms                                                         | 50.1 ms: 1.22x faster                                                         |
| genshi_text     | 26.8 ms                                                         | 22.5 ms: 1.19x faster                                                         |
| Geometric mean  | (ref)                                                           | 1.27x faster                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 97.7 us: 4.89x faster                                                         |
| generators                 | 52.2 ms                                                         | 22.1 ms: 2.37x faster                                                         |
| logging_silent             | 119 ns                                                          | 59.6 ns: 2.00x faster                                                         |
| pylint                     | 418 ms                                                          | 226 ms: 1.85x faster                                                          |
| coroutines                 | 23.7 ms                                                         | 14.4 ms: 1.65x faster                                                         |
| spectral_norm              | 122 ms                                                          | 74.0 ms: 1.64x faster                                                         |
| deepcopy_memo              | 40.0 us                                                         | 24.4 us: 1.64x faster                                                         |
| deltablue                  | 4.10 ms                                                         | 2.52 ms: 1.63x faster                                                         |
| unpack_sequence            | 65.2 ns                                                         | 41.7 ns: 1.56x faster                                                         |
| richards_super             | 58.7 ms                                                         | 37.7 ms: 1.56x faster                                                         |
| sqlglot_parse              | 1.49 ms                                                         | 965 us: 1.55x faster                                                          |
| pickle_pure_python         | 309 us                                                          | 209 us: 1.48x faster                                                          |
| comprehensions             | 22.1 us                                                         | 14.9 us: 1.48x faster                                                         |
| sqlglot_transpile          | 1.78 ms                                                         | 1.21 ms: 1.47x faster                                                         |
| richards                   | 48.8 ms                                                         | 33.6 ms: 1.45x faster                                                         |
| mako                       | 10.3 ms                                                         | 7.12 ms: 1.44x faster                                                         |
| json_dumps                 | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                         |
| chaos                      | 84.4 ms                                                         | 59.5 ms: 1.42x faster                                                         |
| chameleon                  | 8.08 ms                                                         | 5.71 ms: 1.41x faster                                                         |
| deepcopy_reduce            | 3.32 us                                                         | 2.36 us: 1.40x faster                                                         |
| sympy_sum                  | 149 ms                                                          | 107 ms: 1.40x faster                                                          |
| regex_compile              | 148 ms                                                          | 107 ms: 1.38x faster                                                          |
| float                      | 76.1 ms                                                         | 55.1 ms: 1.38x faster                                                         |
| deepcopy                   | 381 us                                                          | 276 us: 1.38x faster                                                          |
| scimark_sor                | 135 ms                                                          | 98.4 ms: 1.37x faster                                                         |
| tomli_loads                | 2.31 sec                                                        | 1.70 sec: 1.36x faster                                                        |
| sympy_str                  | 283 ms                                                          | 209 ms: 1.36x faster                                                          |
| unpickle_pure_python       | 231 us                                                          | 171 us: 1.35x faster                                                          |
| async_tree_none            | 343 ms                                                          | 257 ms: 1.34x faster                                                          |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.18 ms: 1.33x faster                                                         |
| crypto_pyaes               | 79.4 ms                                                         | 60.3 ms: 1.32x faster                                                         |
| logging_simple             | 10.8 us                                                         | 8.26 us: 1.31x faster                                                         |
| nbody                      | 126 ms                                                          | 96.5 ms: 1.30x faster                                                         |
| sympy_integrate            | 19.9 ms                                                         | 15.4 ms: 1.29x faster                                                         |
| logging_format             | 11.5 us                                                         | 8.87 us: 1.29x faster                                                         |
| xml_etree_process          | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                                         |
| async_tree_memoization     | 408 ms                                                          | 320 ms: 1.28x faster                                                          |
| sympy_expand               | 462 ms                                                          | 366 ms: 1.26x faster                                                          |
| go                         | 147 ms                                                          | 118 ms: 1.25x faster                                                          |
| django_template            | 37.4 ms                                                         | 29.9 ms: 1.25x faster                                                         |
| async_tree_memoization_tg  | 378 ms                                                          | 303 ms: 1.25x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 242 ms: 1.24x faster                                                          |
| pyflate                    | 471 ms                                                          | 380 ms: 1.24x faster                                                          |
| pycparser                  | 1.04 sec                                                        | 842 ms: 1.24x faster                                                          |
| tornado_http               | 118 ms                                                          | 95.9 ms: 1.23x faster                                                         |
| async_tree_io_tg           | 746 ms                                                          | 605 ms: 1.23x faster                                                          |
| genshi_xml                 | 61.2 ms                                                         | 50.1 ms: 1.22x faster                                                         |
| scimark_fft                | 291 ms                                                          | 240 ms: 1.22x faster                                                          |
| async_tree_io              | 754 ms                                                          | 621 ms: 1.21x faster                                                          |
| asyncio_tcp                | 787 ms                                                          | 649 ms: 1.21x faster                                                          |
| raytrace                   | 327 ms                                                          | 273 ms: 1.20x faster                                                          |
| html5lib                   | 54.3 ms                                                         | 45.3 ms: 1.20x faster                                                         |
| hexiom                     | 7.51 ms                                                         | 6.29 ms: 1.19x faster                                                         |
| genshi_text                | 26.8 ms                                                         | 22.5 ms: 1.19x faster                                                         |
| nqueens                    | 111 ms                                                          | 94.5 ms: 1.18x faster                                                         |
| mdp                        | 2.07 sec                                                        | 1.75 sec: 1.18x faster                                                        |
| scimark_lu                 | 102 ms                                                          | 87.3 ms: 1.17x faster                                                         |
| docutils                   | 2.10 sec                                                        | 1.80 sec: 1.17x faster                                                        |
| unpickle_list              | 3.28 us                                                         | 2.82 us: 1.16x faster                                                         |
| fannkuch                   | 399 ms                                                          | 345 ms: 1.16x faster                                                          |
| xml_etree_generate         | 71.6 ms                                                         | 62.5 ms: 1.15x faster                                                         |
| sqlglot_optimize           | 51.8 ms                                                         | 45.3 ms: 1.15x faster                                                         |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 518 ms: 1.14x faster                                                          |
| xml_etree_iterparse        | 75.6 ms                                                         | 66.5 ms: 1.14x faster                                                         |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 509 ms: 1.13x faster                                                          |
| json                       | 4.78 ms                                                         | 4.24 ms: 1.13x faster                                                         |
| pprint_pformat             | 1.70 sec                                                        | 1.51 sec: 1.12x faster                                                        |
| sqlite_synth               | 2.15 us                                                         | 1.92 us: 1.12x faster                                                         |
| pprint_safe_repr           | 819 ms                                                          | 744 ms: 1.10x faster                                                          |
| scimark_monte_carlo        | 70.8 ms                                                         | 65.1 ms: 1.09x faster                                                         |
| bench_thread_pool          | 1.14 ms                                                         | 1.05 ms: 1.09x faster                                                         |
| 2to3                       | 282 ms                                                          | 260 ms: 1.08x faster                                                          |
| meteor_contest             | 90.9 ms                                                         | 85.9 ms: 1.06x faster                                                         |
| regex_dna                  | 122 ms                                                          | 116 ms: 1.05x faster                                                          |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                          |
| pidigits                   | 203 ms                                                          | 198 ms: 1.03x faster                                                          |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.01x faster                                                        |
| pickle                     | 7.99 us                                                         | 7.89 us: 1.01x faster                                                         |
| pickle_list                | 3.27 us                                                         | 3.23 us: 1.01x faster                                                         |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                                         |
| json_loads                 | 20.0 us                                                         | 19.8 us: 1.01x faster                                                         |
| gc_traversal               | 1.38 ms                                                         | 1.41 ms: 1.03x slower                                                         |
| regex_effbot               | 1.82 ms                                                         | 1.88 ms: 1.03x slower                                                         |
| bench_mp_pool              | 70.9 ms                                                         | 73.1 ms: 1.03x slower                                                         |
| pathlib                    | 79.9 ms                                                         | 84.5 ms: 1.06x slower                                                         |
| regex_v8                   | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                         |
| create_gc_cycles           | 618 us                                                          | 658 us: 1.07x slower                                                          |
| unpickle                   | 9.23 us                                                         | 10.0 us: 1.08x slower                                                         |
| async_generators           | 260 ms                                                          | 302 ms: 1.16x slower                                                          |
| python_startup             | 22.0 ms                                                         | 25.7 ms: 1.17x slower                                                         |
| dask                       | 355 ms                                                          | 419 ms: 1.18x slower                                                          |
| telco                      | 5.29 ms                                                         | 6.35 ms: 1.20x slower                                                         |
| python_startup_no_site     | 18.8 ms                                                         | 23.6 ms: 1.25x slower                                                         |
| sqlglot_normalize          | 113 ms                                                          | 221 ms: 1.95x slower                                                          |
| coverage                   | 58.0 ms                                                         | 484 ms: 8.34x slower                                                          |
| thrift                     | 801 us                                                          | 10.7 ms: 13.36x slower                                                        |
| Geometric mean             | (ref)                                                           | 1.16x faster                                                                  |
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown