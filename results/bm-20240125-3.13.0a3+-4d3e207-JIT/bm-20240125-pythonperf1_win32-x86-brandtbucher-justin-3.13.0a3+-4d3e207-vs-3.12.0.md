
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: windows-x86
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.12x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 255 ms: 1.10x faster                                                    |
| chameleon      | 7.75 ms                                                         | 6.09 ms: 1.27x faster                                                   |
| docutils       | 1.98 sec                                                        | 1.82 sec: 1.09x faster                                                  |
| tornado_http   | 105 ms                                                          | 98.2 ms: 1.07x faster                                                   |
| Geometric mean | (ref)                                                           | 1.13x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                    |
| async_tree_memoization_tg  | 350 ms                                                          | 307 ms: 1.14x faster                                                    |
| async_tree_none_tg         | 278 ms                                                          | 247 ms: 1.13x faster                                                    |
| async_tree_memoization     | 364 ms                                                          | 324 ms: 1.12x faster                                                    |
| async_tree_io              | 693 ms                                                          | 617 ms: 1.12x faster                                                    |
| async_tree_io_tg           | 677 ms                                                          | 609 ms: 1.11x faster                                                    |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 520 ms: 1.08x faster                                                    |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 511 ms: 1.07x faster                                                    |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 55.9 ms: 1.37x faster                                                   |
| nbody          | 127 ms                                                          | 93.0 ms: 1.37x faster                                                   |
| pidigits       | 199 ms                                                          | 204 ms: 1.02x slower                                                    |
| Geometric mean | (ref)                                                           | 1.22x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 106 ms: 1.21x faster                                                    |
| regex_effbot   | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                   |
| regex_dna      | 127 ms                                                          | 120 ms: 1.06x faster                                                    |
| regex_v8       | 15.0 ms                                                         | 16.4 ms: 1.09x slower                                                   |
| Geometric mean | (ref)                                                           | 1.06x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 150 us: 1.40x faster                                                    |
| pickle_pure_python   | 286 us                                                          | 205 us: 1.39x faster                                                    |
| tomli_loads          | 2.20 sec                                                        | 1.64 sec: 1.34x faster                                                  |
| xml_etree_process    | 53.2 ms                                                         | 41.2 ms: 1.29x faster                                                   |
| xml_etree_generate   | 72.1 ms                                                         | 59.2 ms: 1.22x faster                                                   |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.5 ms: 1.13x faster                                                   |
| json_dumps           | 7.40 ms                                                         | 6.78 ms: 1.09x faster                                                   |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                    |
| pickle_list          | 3.37 us                                                         | 3.26 us: 1.03x faster                                                   |
| json_loads           | 20.4 us                                                         | 20.1 us: 1.02x faster                                                   |
| unpickle             | 9.71 us                                                         | 10.2 us: 1.05x slower                                                   |
| pickle               | 7.79 us                                                         | 8.23 us: 1.06x slower                                                   |
| unpickle_list        | 2.95 us                                                         | 3.23 us: 1.10x slower                                                   |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                            |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.9 ms: 1.03x slower                                                   |
| python_startup_no_site | 19.1 ms                                                         | 20.7 ms: 1.08x slower                                                   |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.75 ms: 1.28x faster                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 60.0 ns: 1.68x faster                                                   |
| deepcopy_memo              | 38.4 us                                                         | 22.9 us: 1.68x faster                                                   |
| generators                 | 38.5 ms                                                         | 23.2 ms: 1.66x faster                                                   |
| scimark_sor                | 130 ms                                                          | 82.3 ms: 1.58x faster                                                   |
| unpack_sequence            | 62.5 ns                                                         | 40.1 ns: 1.56x faster                                                   |
| scimark_lu                 | 93.2 ms                                                         | 61.4 ms: 1.52x faster                                                   |
| richards                   | 41.3 ms                                                         | 28.1 ms: 1.47x faster                                                   |
| richards_super             | 46.5 ms                                                         | 31.7 ms: 1.47x faster                                                   |
| deltablue                  | 3.58 ms                                                         | 2.47 ms: 1.45x faster                                                   |
| coroutines                 | 20.9 ms                                                         | 14.4 ms: 1.45x faster                                                   |
| unpickle_pure_python       | 210 us                                                          | 150 us: 1.40x faster                                                    |
| pickle_pure_python         | 286 us                                                          | 205 us: 1.39x faster                                                    |
| sqlglot_parse              | 1.25 ms                                                         | 902 us: 1.38x faster                                                    |
| float                      | 76.7 ms                                                         | 55.9 ms: 1.37x faster                                                   |
| raytrace                   | 308 ms                                                          | 225 ms: 1.37x faster                                                    |
| nbody                      | 127 ms                                                          | 93.0 ms: 1.37x faster                                                   |
| deepcopy_reduce            | 3.23 us                                                         | 2.39 us: 1.35x faster                                                   |
| deepcopy                   | 360 us                                                          | 268 us: 1.34x faster                                                    |
| tomli_loads                | 2.20 sec                                                        | 1.64 sec: 1.34x faster                                                  |
| sqlglot_transpile          | 1.53 ms                                                         | 1.15 ms: 1.34x faster                                                   |
| spectral_norm              | 104 ms                                                          | 78.1 ms: 1.33x faster                                                   |
| typing_runtime_protocols   | 126 us                                                          | 95.7 us: 1.32x faster                                                   |
| xml_etree_process          | 53.2 ms                                                         | 41.2 ms: 1.29x faster                                                   |
| mako                       | 9.96 ms                                                         | 7.75 ms: 1.28x faster                                                   |
| chameleon                  | 7.75 ms                                                         | 6.09 ms: 1.27x faster                                                   |
| comprehensions             | 19.2 us                                                         | 15.1 us: 1.27x faster                                                   |
| logging_simple             | 9.75 us                                                         | 7.90 us: 1.23x faster                                                   |
| xml_etree_generate         | 72.1 ms                                                         | 59.2 ms: 1.22x faster                                                   |
| regex_compile              | 129 ms                                                          | 106 ms: 1.21x faster                                                    |
| logging_format             | 10.4 us                                                         | 8.61 us: 1.21x faster                                                   |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.23 ms: 1.19x faster                                                   |
| pycparser                  | 978 ms                                                          | 826 ms: 1.18x faster                                                    |
| chaos                      | 69.4 ms                                                         | 58.8 ms: 1.18x faster                                                   |
| go                         | 137 ms                                                          | 117 ms: 1.18x faster                                                    |
| fannkuch                   | 354 ms                                                          | 302 ms: 1.17x faster                                                    |
| pyflate                    | 424 ms                                                          | 366 ms: 1.16x faster                                                    |
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                    |
| async_tree_memoization_tg  | 350 ms                                                          | 307 ms: 1.14x faster                                                    |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.5 ms: 1.13x faster                                                   |
| sqlglot_optimize           | 48.5 ms                                                         | 42.7 ms: 1.13x faster                                                   |
| async_tree_none_tg         | 278 ms                                                          | 247 ms: 1.13x faster                                                    |
| async_tree_memoization     | 364 ms                                                          | 324 ms: 1.12x faster                                                    |
| async_tree_io              | 693 ms                                                          | 617 ms: 1.12x faster                                                    |
| sympy_str                  | 240 ms                                                          | 214 ms: 1.12x faster                                                    |
| sympy_sum                  | 123 ms                                                          | 110 ms: 1.12x faster                                                    |
| sympy_integrate            | 17.5 ms                                                         | 15.7 ms: 1.11x faster                                                   |
| async_tree_io_tg           | 677 ms                                                          | 609 ms: 1.11x faster                                                    |
| crypto_pyaes               | 69.2 ms                                                         | 62.5 ms: 1.11x faster                                                   |
| sqlite_synth               | 2.07 us                                                         | 1.88 us: 1.10x faster                                                   |
| sympy_expand               | 398 ms                                                          | 362 ms: 1.10x faster                                                    |
| 2to3                       | 280 ms                                                          | 255 ms: 1.10x faster                                                    |
| bench_thread_pool          | 1.10 ms                                                         | 1.01 ms: 1.09x faster                                                   |
| docutils                   | 1.98 sec                                                        | 1.82 sec: 1.09x faster                                                  |
| json_dumps                 | 7.40 ms                                                         | 6.78 ms: 1.09x faster                                                   |
| scimark_fft                | 271 ms                                                          | 249 ms: 1.09x faster                                                    |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 520 ms: 1.08x faster                                                    |
| nqueens                    | 93.7 ms                                                         | 86.6 ms: 1.08x faster                                                   |
| tornado_http               | 105 ms                                                          | 98.2 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 511 ms: 1.07x faster                                                    |
| pprint_pformat             | 1.50 sec                                                        | 1.40 sec: 1.07x faster                                                  |
| dask                       | 323 ms                                                          | 303 ms: 1.07x faster                                                    |
| pprint_safe_repr           | 721 ms                                                          | 676 ms: 1.07x faster                                                    |
| async_generators           | 313 ms                                                          | 295 ms: 1.06x faster                                                    |
| regex_effbot               | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                   |
| hexiom                     | 6.82 ms                                                         | 6.45 ms: 1.06x faster                                                   |
| regex_dna                  | 127 ms                                                          | 120 ms: 1.06x faster                                                    |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                    |
| mdp                        | 1.91 sec                                                        | 1.84 sec: 1.04x faster                                                  |
| pickle_list                | 3.37 us                                                         | 3.26 us: 1.03x faster                                                   |
| meteor_contest             | 86.9 ms                                                         | 84.3 ms: 1.03x faster                                                   |
| pathlib                    | 91.4 ms                                                         | 89.0 ms: 1.03x faster                                                   |
| bench_mp_pool              | 75.4 ms                                                         | 73.8 ms: 1.02x faster                                                   |
| json_loads                 | 20.4 us                                                         | 20.1 us: 1.02x faster                                                   |
| json                       | 4.15 ms                                                         | 4.18 ms: 1.01x slower                                                   |
| create_gc_cycles           | 652 us                                                          | 662 us: 1.02x slower                                                    |
| pidigits                   | 199 ms                                                          | 204 ms: 1.02x slower                                                    |
| python_startup             | 22.4 ms                                                         | 22.9 ms: 1.03x slower                                                   |
| unpickle                   | 9.71 us                                                         | 10.2 us: 1.05x slower                                                   |
| pickle                     | 7.79 us                                                         | 8.23 us: 1.06x slower                                                   |
| scimark_monte_carlo        | 66.4 ms                                                         | 70.8 ms: 1.07x slower                                                   |
| telco                      | 5.51 ms                                                         | 5.94 ms: 1.08x slower                                                   |
| python_startup_no_site     | 19.1 ms                                                         | 20.7 ms: 1.08x slower                                                   |
| regex_v8                   | 15.0 ms                                                         | 16.4 ms: 1.09x slower                                                   |
| unpickle_list              | 2.95 us                                                         | 3.23 us: 1.10x slower                                                   |
| sqlglot_normalize          | 100 ms                                                          | 219 ms: 2.18x slower                                                    |
| coverage                   | 48.4 ms                                                         | 499 ms: 10.31x slower                                                   |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                            |

Benchmark hidden because not significant (4): asyncio_tcp, gc_traversal, asyncio_tcp_ssl, pickle_dict
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown