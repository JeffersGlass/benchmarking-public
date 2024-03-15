
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.03x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 298 ms: 1.04x slower                                                          |
| chameleon      | 7.23 ms                                                      | 7.83 ms: 1.08x slower                                                         |
| tornado_http   | 121 ms                                                       | 124 ms: 1.02x slower                                                          |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                  |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 434 ms: 1.04x faster                                                          |
| async_tree_memoization     | 544 ms                                                       | 549 ms: 1.01x slower                                                          |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 707 ms: 1.01x slower                                                          |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                                          |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                        |
| async_tree_memoization_tg  | 540 ms                                                       | 564 ms: 1.04x slower                                                          |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                          |
| float          | 76.6 ms                                                      | 79.4 ms: 1.04x slower                                                         |
| nbody          | 88.0 ms                                                      | 98.7 ms: 1.12x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                         |
| regex_compile  | 144 ms                                                       | 145 ms: 1.01x slower                                                          |
| regex_dna      | 239 ms                                                       | 255 ms: 1.07x slower                                                          |
| regex_v8       | 23.6 ms                                                      | 26.2 ms: 1.11x slower                                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| xml_etree_generate   | 86.1 ms                                                      | 84.1 ms: 1.02x faster                                                         |
| pickle_dict          | 32.5 us                                                      | 31.9 us: 1.02x faster                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.13 sec: 1.01x faster                                                        |
| pickle_list          | 4.43 us                                                      | 4.37 us: 1.01x faster                                                         |
| pickle_pure_python   | 318 us                                                       | 314 us: 1.01x faster                                                          |
| unpickle             | 14.8 us                                                      | 14.6 us: 1.01x faster                                                         |
| xml_etree_process    | 58.4 ms                                                      | 57.9 ms: 1.01x faster                                                         |
| json_dumps           | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                                         |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                          |
| unpickle_list        | 4.66 us                                                      | 4.77 us: 1.02x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.3 us: 1.04x slower                                                         |
| unpickle_pure_python | 210 us                                                       | 232 us: 1.11x slower                                                          |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                         |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.6 ms: 1.06x slower                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 121 us: 1.25x faster                                                          |
| unpack_sequence            | 53.2 ns                                                      | 44.6 ns: 1.19x faster                                                         |
| comprehensions             | 21.9 us                                                      | 19.0 us: 1.15x faster                                                         |
| generators                 | 37.4 ms                                                      | 33.9 ms: 1.10x faster                                                         |
| raytrace                   | 298 ms                                                       | 276 ms: 1.08x faster                                                          |
| async_generators           | 390 ms                                                       | 368 ms: 1.06x faster                                                          |
| async_tree_none            | 452 ms                                                       | 434 ms: 1.04x faster                                                          |
| crypto_pyaes               | 80.3 ms                                                      | 77.4 ms: 1.04x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.2 ms: 1.03x faster                                                         |
| regex_effbot               | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                         |
| create_gc_cycles           | 1.59 ms                                                      | 1.54 ms: 1.03x faster                                                         |
| xml_etree_generate         | 86.1 ms                                                      | 84.1 ms: 1.02x faster                                                         |
| asyncio_tcp                | 378 ms                                                       | 370 ms: 1.02x faster                                                          |
| sympy_sum                  | 162 ms                                                       | 159 ms: 1.02x faster                                                          |
| pickle_dict                | 32.5 us                                                      | 31.9 us: 1.02x faster                                                         |
| sqlite_synth               | 2.77 us                                                      | 2.72 us: 1.02x faster                                                         |
| gc_traversal               | 3.48 ms                                                      | 3.43 ms: 1.01x faster                                                         |
| logging_format             | 7.48 us                                                      | 7.38 us: 1.01x faster                                                         |
| tomli_loads                | 2.16 sec                                                     | 2.13 sec: 1.01x faster                                                        |
| pickle_list                | 4.43 us                                                      | 4.37 us: 1.01x faster                                                         |
| pickle_pure_python         | 318 us                                                       | 314 us: 1.01x faster                                                          |
| sympy_str                  | 302 ms                                                       | 299 ms: 1.01x faster                                                          |
| unpickle                   | 14.8 us                                                      | 14.6 us: 1.01x faster                                                         |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                          |
| xml_etree_process          | 58.4 ms                                                      | 57.9 ms: 1.01x faster                                                         |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                                        |
| deepcopy_reduce            | 3.37 us                                                      | 3.35 us: 1.01x faster                                                         |
| pathlib                    | 18.9 ms                                                      | 19.0 ms: 1.00x slower                                                         |
| logging_simple             | 6.71 us                                                      | 6.76 us: 1.01x slower                                                         |
| regex_compile              | 144 ms                                                       | 145 ms: 1.01x slower                                                          |
| async_tree_memoization     | 544 ms                                                       | 549 ms: 1.01x slower                                                          |
| mdp                        | 2.57 sec                                                     | 2.60 sec: 1.01x slower                                                        |
| sympy_integrate            | 23.9 ms                                                      | 24.2 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 707 ms: 1.01x slower                                                          |
| json_dumps                 | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                                          |
| logging_silent             | 94.4 ns                                                      | 95.9 ns: 1.02x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 118 ms: 1.02x slower                                                          |
| deepcopy                   | 368 us                                                       | 375 us: 1.02x slower                                                          |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                          |
| unpickle_list              | 4.66 us                                                      | 4.77 us: 1.02x slower                                                         |
| tornado_http               | 121 ms                                                       | 124 ms: 1.02x slower                                                          |
| sqlglot_parse              | 1.38 ms                                                      | 1.41 ms: 1.03x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 101 ms: 1.03x slower                                                          |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.82 ms: 1.03x slower                                                         |
| nqueens                    | 89.9 ms                                                      | 92.6 ms: 1.03x slower                                                         |
| deepcopy_memo              | 36.8 us                                                      | 37.9 us: 1.03x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                        |
| json                       | 5.12 ms                                                      | 5.29 ms: 1.03x slower                                                         |
| pycparser                  | 1.23 sec                                                     | 1.28 sec: 1.04x slower                                                        |
| bench_thread_pool          | 950 us                                                       | 983 us: 1.04x slower                                                          |
| float                      | 76.6 ms                                                      | 79.4 ms: 1.04x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.71 sec: 1.04x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 837 ms: 1.04x slower                                                          |
| json_loads                 | 24.4 us                                                      | 25.3 us: 1.04x slower                                                         |
| dask                       | 392 ms                                                       | 408 ms: 1.04x slower                                                          |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.37 ms: 1.04x slower                                                         |
| sympy_expand               | 484 ms                                                       | 504 ms: 1.04x slower                                                          |
| async_tree_memoization_tg  | 540 ms                                                       | 564 ms: 1.04x slower                                                          |
| 2to3                       | 285 ms                                                       | 298 ms: 1.04x slower                                                          |
| dulwich_log                | 65.4 ms                                                      | 68.5 ms: 1.05x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 60.6 ms: 1.05x slower                                                         |
| mako                       | 10.0 ms                                                      | 10.6 ms: 1.06x slower                                                         |
| chaos                      | 64.0 ms                                                      | 68.3 ms: 1.07x slower                                                         |
| regex_dna                  | 239 ms                                                       | 255 ms: 1.07x slower                                                          |
| scimark_fft                | 301 ms                                                       | 325 ms: 1.08x slower                                                          |
| chameleon                  | 7.23 ms                                                      | 7.83 ms: 1.08x slower                                                         |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                         |
| spectral_norm              | 91.6 ms                                                      | 99.8 ms: 1.09x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 26.2 ms: 1.11x slower                                                         |
| unpickle_pure_python       | 210 us                                                       | 232 us: 1.11x slower                                                          |
| richards_super             | 51.3 ms                                                      | 57.4 ms: 1.12x slower                                                         |
| go                         | 150 ms                                                       | 168 ms: 1.12x slower                                                          |
| fannkuch                   | 350 ms                                                       | 392 ms: 1.12x slower                                                          |
| nbody                      | 88.0 ms                                                      | 98.7 ms: 1.12x slower                                                         |
| richards                   | 45.7 ms                                                      | 51.5 ms: 1.13x slower                                                         |
| deltablue                  | 3.24 ms                                                      | 3.68 ms: 1.14x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 79.2 ms: 1.15x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.01 ms: 1.15x slower                                                         |
| pyflate                    | 439 ms                                                       | 522 ms: 1.19x slower                                                          |
| coverage                   | 66.7 ms                                                      | 81.8 ms: 1.23x slower                                                         |
| hexiom                     | 5.96 ms                                                      | 7.33 ms: 1.23x slower                                                         |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                         |
| scimark_sor                | 109 ms                                                       | 142 ms: 1.31x slower                                                          |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                  |

Benchmark hidden because not significant (8): xml_etree_iterparse, meteor_contest, docutils, pickle, asyncio_websockets, async_tree_cpu_io_mixed, bench_mp_pool, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.91x