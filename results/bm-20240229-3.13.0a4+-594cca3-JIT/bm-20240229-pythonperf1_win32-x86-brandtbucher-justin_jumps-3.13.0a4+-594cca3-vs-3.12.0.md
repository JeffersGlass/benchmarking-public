# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-x86
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 264 ms: 1.06x faster                                                          |
| chameleon      | 7.75 ms                                                         | 5.90 ms: 1.31x faster                                                         |
| docutils       | 1.98 sec                                                        | 1.89 sec: 1.05x faster                                                        |
| tornado_http   | 105 ms                                                          | 99.4 ms: 1.06x faster                                                         |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 350 ms                                                          | 315 ms: 1.11x faster                                                          |
| async_tree_none            | 298 ms                                                          | 268 ms: 1.11x faster                                                          |
| async_tree_none_tg         | 278 ms                                                          | 251 ms: 1.10x faster                                                          |
| async_tree_io_tg           | 677 ms                                                          | 618 ms: 1.10x faster                                                          |
| async_tree_memoization     | 364 ms                                                          | 332 ms: 1.09x faster                                                          |
| async_tree_io              | 693 ms                                                          | 637 ms: 1.09x faster                                                          |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 556 ms: 1.01x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 541 ms: 1.01x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.08x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 55.2 ms: 1.39x faster                                                         |
| nbody          | 127 ms                                                          | 97.7 ms: 1.30x faster                                                         |
| pidigits       | 199 ms                                                          | 200 ms: 1.00x slower                                                          |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 114 ms: 1.14x faster                                                          |
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                         |
| regex_dna      | 127 ms                                                          | 119 ms: 1.07x faster                                                          |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_pure_python   | 286 us                                                          | 227 us: 1.26x faster                                                          |
| tomli_loads          | 2.20 sec                                                        | 1.75 sec: 1.26x faster                                                        |
| unpickle_pure_python | 210 us                                                          | 174 us: 1.20x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 44.3 ms: 1.20x faster                                                         |
| xml_etree_iterparse  | 77.6 ms                                                         | 66.9 ms: 1.16x faster                                                         |
| xml_etree_generate   | 72.1 ms                                                         | 63.8 ms: 1.13x faster                                                         |
| unpickle_list        | 2.95 us                                                         | 2.79 us: 1.05x faster                                                         |
| xml_etree_parse      | 113 ms                                                          | 108 ms: 1.04x faster                                                          |
| json_dumps           | 7.40 ms                                                         | 7.16 ms: 1.03x faster                                                         |
| pickle_list          | 3.37 us                                                         | 3.29 us: 1.02x faster                                                         |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                                         |
| pickle               | 7.79 us                                                         | 7.91 us: 1.02x slower                                                         |
| unpickle             | 9.71 us                                                         | 10.0 us: 1.03x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                  |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 26.0 ms: 1.16x slower                                                         |
| python_startup_no_site | 19.1 ms                                                         | 23.7 ms: 1.24x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.20x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.24 ms: 1.37x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 25.0 ms: 1.54x faster                                                         |
| logging_silent             | 101 ns                                                          | 70.3 ns: 1.44x faster                                                         |
| unpack_sequence            | 62.5 ns                                                         | 43.7 ns: 1.43x faster                                                         |
| spectral_norm              | 104 ms                                                          | 73.3 ms: 1.42x faster                                                         |
| float                      | 76.7 ms                                                         | 55.2 ms: 1.39x faster                                                         |
| coroutines                 | 20.9 ms                                                         | 15.1 ms: 1.38x faster                                                         |
| deepcopy_memo              | 38.4 us                                                         | 27.9 us: 1.38x faster                                                         |
| mako                       | 9.96 ms                                                         | 7.24 ms: 1.37x faster                                                         |
| chameleon                  | 7.75 ms                                                         | 5.90 ms: 1.31x faster                                                         |
| deltablue                  | 3.58 ms                                                         | 2.74 ms: 1.31x faster                                                         |
| typing_runtime_protocols   | 126 us                                                          | 97.1 us: 1.30x faster                                                         |
| nbody                      | 127 ms                                                          | 97.7 ms: 1.30x faster                                                         |
| pickle_pure_python         | 286 us                                                          | 227 us: 1.26x faster                                                          |
| tomli_loads                | 2.20 sec                                                        | 1.75 sec: 1.26x faster                                                        |
| comprehensions             | 19.2 us                                                         | 15.3 us: 1.26x faster                                                         |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.11 ms: 1.24x faster                                                         |
| deepcopy_reduce            | 3.23 us                                                         | 2.61 us: 1.24x faster                                                         |
| deepcopy                   | 360 us                                                          | 294 us: 1.23x faster                                                          |
| unpickle_pure_python       | 210 us                                                          | 174 us: 1.20x faster                                                          |
| scimark_sor                | 130 ms                                                          | 108 ms: 1.20x faster                                                          |
| xml_etree_process          | 53.2 ms                                                         | 44.3 ms: 1.20x faster                                                         |
| sqlglot_parse              | 1.25 ms                                                         | 1.04 ms: 1.20x faster                                                         |
| chaos                      | 69.4 ms                                                         | 58.9 ms: 1.18x faster                                                         |
| logging_format             | 10.4 us                                                         | 8.87 us: 1.17x faster                                                         |
| sqlglot_transpile          | 1.53 ms                                                         | 1.31 ms: 1.17x faster                                                         |
| logging_simple             | 9.75 us                                                         | 8.33 us: 1.17x faster                                                         |
| xml_etree_iterparse        | 77.6 ms                                                         | 66.9 ms: 1.16x faster                                                         |
| regex_compile              | 129 ms                                                          | 114 ms: 1.14x faster                                                          |
| scimark_fft                | 271 ms                                                          | 239 ms: 1.13x faster                                                          |
| crypto_pyaes               | 69.2 ms                                                         | 61.1 ms: 1.13x faster                                                         |
| sympy_sum                  | 123 ms                                                          | 109 ms: 1.13x faster                                                          |
| xml_etree_generate         | 72.1 ms                                                         | 63.8 ms: 1.13x faster                                                         |
| sympy_str                  | 240 ms                                                          | 213 ms: 1.12x faster                                                          |
| richards_super             | 46.5 ms                                                         | 41.7 ms: 1.11x faster                                                         |
| richards                   | 41.3 ms                                                         | 37.1 ms: 1.11x faster                                                         |
| sqlite_synth               | 2.07 us                                                         | 1.86 us: 1.11x faster                                                         |
| pycparser                  | 978 ms                                                          | 878 ms: 1.11x faster                                                          |
| async_tree_memoization_tg  | 350 ms                                                          | 315 ms: 1.11x faster                                                          |
| async_tree_none            | 298 ms                                                          | 268 ms: 1.11x faster                                                          |
| raytrace                   | 308 ms                                                          | 277 ms: 1.11x faster                                                          |
| async_tree_none_tg         | 278 ms                                                          | 251 ms: 1.10x faster                                                          |
| sympy_integrate            | 17.5 ms                                                         | 15.9 ms: 1.10x faster                                                         |
| async_tree_io_tg           | 677 ms                                                          | 618 ms: 1.10x faster                                                          |
| async_tree_memoization     | 364 ms                                                          | 332 ms: 1.09x faster                                                          |
| pyflate                    | 424 ms                                                          | 388 ms: 1.09x faster                                                          |
| async_tree_io              | 693 ms                                                          | 637 ms: 1.09x faster                                                          |
| pathlib                    | 91.4 ms                                                         | 84.6 ms: 1.08x faster                                                         |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                         |
| hexiom                     | 6.82 ms                                                         | 6.32 ms: 1.08x faster                                                         |
| sympy_expand               | 398 ms                                                          | 372 ms: 1.07x faster                                                          |
| go                         | 137 ms                                                          | 128 ms: 1.07x faster                                                          |
| scimark_lu                 | 93.2 ms                                                         | 87.2 ms: 1.07x faster                                                         |
| regex_dna                  | 127 ms                                                          | 119 ms: 1.07x faster                                                          |
| fannkuch                   | 354 ms                                                          | 332 ms: 1.07x faster                                                          |
| mdp                        | 1.91 sec                                                        | 1.80 sec: 1.06x faster                                                        |
| 2to3                       | 280 ms                                                          | 264 ms: 1.06x faster                                                          |
| tornado_http               | 105 ms                                                          | 99.4 ms: 1.06x faster                                                         |
| unpickle_list              | 2.95 us                                                         | 2.79 us: 1.05x faster                                                         |
| docutils                   | 1.98 sec                                                        | 1.89 sec: 1.05x faster                                                        |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                        |
| asyncio_tcp                | 662 ms                                                          | 632 ms: 1.05x faster                                                          |
| xml_etree_parse            | 113 ms                                                          | 108 ms: 1.04x faster                                                          |
| meteor_contest             | 86.9 ms                                                         | 83.5 ms: 1.04x faster                                                         |
| bench_thread_pool          | 1.10 ms                                                         | 1.06 ms: 1.04x faster                                                         |
| json_dumps                 | 7.40 ms                                                         | 7.16 ms: 1.03x faster                                                         |
| gc_traversal               | 1.44 ms                                                         | 1.40 ms: 1.03x faster                                                         |
| pickle_list                | 3.37 us                                                         | 3.29 us: 1.02x faster                                                         |
| sqlglot_optimize           | 48.5 ms                                                         | 47.4 ms: 1.02x faster                                                         |
| nqueens                    | 93.7 ms                                                         | 91.7 ms: 1.02x faster                                                         |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 556 ms: 1.01x faster                                                          |
| bench_mp_pool              | 75.4 ms                                                         | 74.5 ms: 1.01x faster                                                         |
| scimark_monte_carlo        | 66.4 ms                                                         | 65.7 ms: 1.01x faster                                                         |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 541 ms: 1.01x faster                                                          |
| pidigits                   | 199 ms                                                          | 200 ms: 1.00x slower                                                          |
| async_generators           | 313 ms                                                          | 316 ms: 1.01x slower                                                          |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                                         |
| pickle                     | 7.79 us                                                         | 7.91 us: 1.02x slower                                                         |
| pprint_safe_repr           | 721 ms                                                          | 735 ms: 1.02x slower                                                          |
| unpickle                   | 9.71 us                                                         | 10.0 us: 1.03x slower                                                         |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                         |
| telco                      | 5.51 ms                                                         | 6.18 ms: 1.12x slower                                                         |
| python_startup             | 22.4 ms                                                         | 26.0 ms: 1.16x slower                                                         |
| python_startup_no_site     | 19.1 ms                                                         | 23.7 ms: 1.24x slower                                                         |
| sqlglot_normalize          | 100 ms                                                          | 235 ms: 2.34x slower                                                          |
| coverage                   | 48.4 ms                                                         | 330 ms: 6.80x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.08x faster                                                                  |

Benchmark hidden because not significant (4): json, create_gc_cycles, pprint_pformat, json_loads
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown