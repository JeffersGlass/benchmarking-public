# Results vs. 3.12.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: windows-x86
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 255 ms: 1.10x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.77 ms: 1.34x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.82 sec: 1.09x faster                                                          |
| tornado_http   | 105 ms                                                          | 95.2 ms: 1.10x faster                                                           |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 350 ms                                                          | 302 ms: 1.16x faster                                                            |
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 318 ms: 1.14x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 597 ms: 1.13x faster                                                            |
| async_tree_io              | 693 ms                                                          | 612 ms: 1.13x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 523 ms: 1.08x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 507 ms: 1.08x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 54.7 ms: 1.40x faster                                                           |
| nbody          | 127 ms                                                          | 93.7 ms: 1.36x faster                                                           |
| pidigits       | 199 ms                                                          | 201 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 111 ms: 1.16x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.97 ms: 1.04x faster                                                           |
| regex_dna      | 127 ms                                                          | 130 ms: 1.02x slower                                                            |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 286 us                                                          | 214 us: 1.34x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.66 sec: 1.32x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 41.9 ms: 1.27x faster                                                           |
| unpickle_pure_python | 210 us                                                          | 167 us: 1.26x faster                                                            |
| xml_etree_generate   | 72.1 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 66.6 ms: 1.17x faster                                                           |
| unpickle_list        | 2.95 us                                                         | 2.65 us: 1.11x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.80 ms: 1.09x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 107 ms: 1.06x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| json_loads           | 20.4 us                                                         | 20.5 us: 1.00x slower                                                           |
| unpickle             | 9.71 us                                                         | 9.86 us: 1.02x slower                                                           |
| pickle_dict          | 19.9 us                                                         | 20.3 us: 1.02x slower                                                           |
| pickle               | 7.79 us                                                         | 8.02 us: 1.03x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.12x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 26.2 ms: 1.17x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 23.6 ms: 1.24x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.20x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.22 ms: 1.38x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 21.6 ms: 1.78x faster                                                           |
| logging_silent             | 101 ns                                                          | 60.2 ns: 1.68x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 24.2 us: 1.59x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.1 ms: 1.48x faster                                                           |
| spectral_norm              | 104 ms                                                          | 71.1 ms: 1.46x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.51 ms: 1.43x faster                                                           |
| float                      | 76.7 ms                                                         | 54.7 ms: 1.40x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.22 ms: 1.38x faster                                                           |
| comprehensions             | 19.2 us                                                         | 14.1 us: 1.36x faster                                                           |
| nbody                      | 127 ms                                                          | 93.7 ms: 1.36x faster                                                           |
| deepcopy                   | 360 us                                                          | 268 us: 1.35x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.40 us: 1.35x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 5.77 ms: 1.34x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 94.5 us: 1.34x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 214 us: 1.34x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.66 sec: 1.32x faster                                                          |
| scimark_sor                | 130 ms                                                          | 98.4 ms: 1.32x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 958 us: 1.30x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.20 ms: 1.28x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 41.9 ms: 1.27x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 167 us: 1.26x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.16 ms: 1.22x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| logging_format             | 10.4 us                                                         | 8.76 us: 1.19x faster                                                           |
| chaos                      | 69.4 ms                                                         | 58.6 ms: 1.18x faster                                                           |
| logging_simple             | 9.75 us                                                         | 8.23 us: 1.18x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 58.5 ms: 1.18x faster                                                           |
| raytrace                   | 308 ms                                                          | 261 ms: 1.18x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 66.6 ms: 1.17x faster                                                           |
| regex_compile              | 129 ms                                                          | 111 ms: 1.16x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 302 ms: 1.16x faster                                                            |
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                            |
| richards                   | 41.3 ms                                                         | 35.8 ms: 1.15x faster                                                           |
| go                         | 137 ms                                                          | 119 ms: 1.15x faster                                                            |
| pycparser                  | 978 ms                                                          | 850 ms: 1.15x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 107 ms: 1.15x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| sympy_str                  | 240 ms                                                          | 208 ms: 1.15x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.3 ms: 1.15x faster                                                           |
| scimark_fft                | 271 ms                                                          | 236 ms: 1.15x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 318 ms: 1.14x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 597 ms: 1.13x faster                                                            |
| async_tree_io              | 693 ms                                                          | 612 ms: 1.13x faster                                                            |
| pyflate                    | 424 ms                                                          | 376 ms: 1.13x faster                                                            |
| async_generators           | 313 ms                                                          | 278 ms: 1.13x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.70 sec: 1.13x faster                                                          |
| richards_super             | 46.5 ms                                                         | 41.6 ms: 1.12x faster                                                           |
| unpickle_list              | 2.95 us                                                         | 2.65 us: 1.11x faster                                                           |
| tornado_http               | 105 ms                                                          | 95.2 ms: 1.10x faster                                                           |
| sympy_expand               | 398 ms                                                          | 362 ms: 1.10x faster                                                            |
| 2to3                       | 280 ms                                                          | 255 ms: 1.10x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.82 sec: 1.09x faster                                                          |
| meteor_contest             | 86.9 ms                                                         | 79.7 ms: 1.09x faster                                                           |
| json_dumps                 | 7.40 ms                                                         | 6.80 ms: 1.09x faster                                                           |
| sqlite_synth               | 2.07 us                                                         | 1.90 us: 1.09x faster                                                           |
| fannkuch                   | 354 ms                                                          | 325 ms: 1.09x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 44.6 ms: 1.09x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 84.6 ms: 1.08x faster                                                           |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 523 ms: 1.08x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 507 ms: 1.08x faster                                                            |
| hexiom                     | 6.82 ms                                                         | 6.35 ms: 1.07x faster                                                           |
| bench_thread_pool          | 1.10 ms                                                         | 1.03 ms: 1.07x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 107 ms: 1.06x faster                                                            |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                          |
| nqueens                    | 93.7 ms                                                         | 89.2 ms: 1.05x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 89.2 ms: 1.04x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.97 ms: 1.04x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.39 ms: 1.03x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 61.0 ns: 1.02x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 73.7 ms: 1.02x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 65.4 ms: 1.02x faster                                                           |
| json_loads                 | 20.4 us                                                         | 20.5 us: 1.00x slower                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.51 sec: 1.01x slower                                                          |
| pidigits                   | 199 ms                                                          | 201 ms: 1.01x slower                                                            |
| unpickle                   | 9.71 us                                                         | 9.86 us: 1.02x slower                                                           |
| pickle_dict                | 19.9 us                                                         | 20.3 us: 1.02x slower                                                           |
| pprint_safe_repr           | 721 ms                                                          | 735 ms: 1.02x slower                                                            |
| json                       | 4.15 ms                                                         | 4.25 ms: 1.02x slower                                                           |
| regex_dna                  | 127 ms                                                          | 130 ms: 1.02x slower                                                            |
| pickle                     | 7.79 us                                                         | 8.02 us: 1.03x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.26 ms: 1.14x slower                                                           |
| python_startup             | 22.4 ms                                                         | 26.2 ms: 1.17x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 23.6 ms: 1.24x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 218 ms: 2.17x slower                                                            |
| coverage                   | 48.4 ms                                                         | 301 ms: 6.22x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (2): asyncio_tcp, create_gc_cycles
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown