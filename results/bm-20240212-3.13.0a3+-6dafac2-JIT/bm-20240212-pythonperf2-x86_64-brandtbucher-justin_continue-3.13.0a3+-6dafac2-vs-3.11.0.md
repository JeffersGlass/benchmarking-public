
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.04x faster \*
- HPT reliability: 96.37%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 298 ms: 1.04x slower                                                          |
| chameleon      | 7.92 ms                                                      | 7.83 ms: 1.01x faster                                                         |
| docutils       | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                          |
| async_tree_memoization     | 629 ms                                                       | 549 ms: 1.15x faster                                                          |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                                          |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 703 ms: 1.07x faster                                                          |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 564 ms: 1.06x faster                                                          |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 707 ms: 1.06x faster                                                          |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                          |
| float          | 74.9 ms                                                      | 79.4 ms: 1.06x slower                                                         |
| nbody          | 92.9 ms                                                      | 98.7 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 145 ms: 1.07x faster                                                          |
| regex_effbot   | 3.34 ms                                                      | 3.46 ms: 1.04x slower                                                         |
| regex_v8       | 24.4 ms                                                      | 26.2 ms: 1.07x slower                                                         |
| regex_dna      | 227 ms                                                       | 255 ms: 1.12x slower                                                          |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.4 ms: 1.28x faster                                                         |
| json_loads           | 28.9 us                                                      | 25.3 us: 1.15x faster                                                         |
| tomli_loads          | 2.25 sec                                                     | 2.13 sec: 1.06x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.05x faster                                                          |
| xml_etree_iterparse  | 107 ms                                                       | 102 ms: 1.04x faster                                                          |
| unpickle_pure_python | 238 us                                                       | 232 us: 1.03x faster                                                          |
| pickle_dict          | 32.3 us                                                      | 31.9 us: 1.01x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.00x faster                                                          |
| unpickle_list        | 4.60 us                                                      | 4.77 us: 1.04x slower                                                         |
| xml_etree_process    | 55.9 ms                                                      | 57.9 ms: 1.04x slower                                                         |
| xml_etree_generate   | 79.7 ms                                                      | 84.1 ms: 1.05x slower                                                         |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                         |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                                         |
| pickle_list          | 3.94 us                                                      | 4.37 us: 1.11x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                         |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.6 ms: 1.04x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 121 us: 4.39x faster                                                          |
| asyncio_tcp                | 747 ms                                                       | 370 ms: 2.02x faster                                                          |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.95x faster                                                        |
| generators                 | 54.6 ms                                                      | 33.9 ms: 1.61x faster                                                         |
| comprehensions             | 25.1 us                                                      | 19.0 us: 1.32x faster                                                         |
| json_dumps                 | 13.3 ms                                                      | 10.4 ms: 1.28x faster                                                         |
| coroutines                 | 27.8 ms                                                      | 22.2 ms: 1.25x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.43 ms: 1.21x faster                                                         |
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                          |
| sympy_sum                  | 186 ms                                                       | 159 ms: 1.17x faster                                                          |
| json_loads                 | 28.9 us                                                      | 25.3 us: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 549 ms: 1.15x faster                                                          |
| sympy_str                  | 337 ms                                                       | 299 ms: 1.13x faster                                                          |
| scimark_lu                 | 114 ms                                                       | 101 ms: 1.13x faster                                                          |
| raytrace                   | 309 ms                                                       | 276 ms: 1.12x faster                                                          |
| nqueens                    | 103 ms                                                       | 92.6 ms: 1.11x faster                                                         |
| richards_super             | 63.6 ms                                                      | 57.4 ms: 1.11x faster                                                         |
| sympy_expand               | 553 ms                                                       | 504 ms: 1.10x faster                                                          |
| chaos                      | 74.9 ms                                                      | 68.3 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                                          |
| deltablue                  | 3.97 ms                                                      | 3.68 ms: 1.08x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 77.4 ms: 1.08x faster                                                         |
| regex_compile              | 156 ms                                                       | 145 ms: 1.07x faster                                                          |
| sqlglot_parse              | 1.51 ms                                                      | 1.41 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 703 ms: 1.07x faster                                                          |
| logging_simple             | 7.24 us                                                      | 6.76 us: 1.07x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.60 sec: 1.07x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 24.2 ms: 1.06x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 564 ms: 1.06x faster                                                          |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 707 ms: 1.06x faster                                                          |
| fannkuch                   | 416 ms                                                       | 392 ms: 1.06x faster                                                          |
| tomli_loads                | 2.25 sec                                                     | 2.13 sec: 1.06x faster                                                        |
| json                       | 5.58 ms                                                      | 5.29 ms: 1.06x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.05x faster                                                          |
| sqlglot_transpile          | 1.91 ms                                                      | 1.82 ms: 1.05x faster                                                         |
| logging_silent             | 100 ns                                                       | 95.9 ns: 1.05x faster                                                         |
| logging_format             | 7.71 us                                                      | 7.38 us: 1.04x faster                                                         |
| xml_etree_iterparse        | 107 ms                                                       | 102 ms: 1.04x faster                                                          |
| deepcopy                   | 391 us                                                       | 375 us: 1.04x faster                                                          |
| mako                       | 11.0 ms                                                      | 10.6 ms: 1.04x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 118 ms: 1.03x faster                                                          |
| unpickle_pure_python       | 238 us                                                       | 232 us: 1.03x faster                                                          |
| unpack_sequence            | 45.7 ns                                                      | 44.6 ns: 1.02x faster                                                         |
| pycparser                  | 1.31 sec                                                     | 1.28 sec: 1.02x faster                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.54 ms: 1.02x faster                                                         |
| meteor_contest             | 131 ms                                                       | 128 ms: 1.02x faster                                                          |
| deepcopy_reduce            | 3.40 us                                                      | 3.35 us: 1.01x faster                                                         |
| chameleon                  | 7.92 ms                                                      | 7.83 ms: 1.01x faster                                                         |
| pickle_dict                | 32.3 us                                                      | 31.9 us: 1.01x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.00x faster                                                          |
| docutils                   | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                                        |
| deepcopy_memo              | 37.5 us                                                      | 37.9 us: 1.01x slower                                                         |
| dulwich_log                | 67.4 ms                                                      | 68.5 ms: 1.02x slower                                                         |
| sqlglot_optimize           | 59.0 ms                                                      | 60.6 ms: 1.03x slower                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.71 sec: 1.03x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.46 ms: 1.04x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.77 us: 1.04x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 57.9 ms: 1.04x slower                                                         |
| richards                   | 49.7 ms                                                      | 51.5 ms: 1.04x slower                                                         |
| 2to3                       | 287 ms                                                       | 298 ms: 1.04x slower                                                          |
| pprint_safe_repr           | 805 ms                                                       | 837 ms: 1.04x slower                                                          |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                          |
| spectral_norm              | 95.1 ms                                                      | 99.8 ms: 1.05x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 7.33 ms: 1.05x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 84.1 ms: 1.05x slower                                                         |
| float                      | 74.9 ms                                                      | 79.4 ms: 1.06x slower                                                         |
| nbody                      | 92.9 ms                                                      | 98.7 ms: 1.06x slower                                                         |
| go                         | 158 ms                                                       | 168 ms: 1.06x slower                                                          |
| pickle                     | 9.89 us                                                      | 10.6 us: 1.07x slower                                                         |
| regex_v8                   | 24.4 ms                                                      | 26.2 ms: 1.07x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.37 ms: 1.08x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.72 us: 1.08x slower                                                         |
| unpickle                   | 13.3 us                                                      | 14.6 us: 1.10x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.37 us: 1.11x slower                                                         |
| regex_dna                  | 227 ms                                                       | 255 ms: 1.12x slower                                                          |
| scimark_monte_carlo        | 69.8 ms                                                      | 79.2 ms: 1.13x slower                                                         |
| async_generators           | 322 ms                                                       | 368 ms: 1.14x slower                                                          |
| scimark_fft                | 281 ms                                                       | 325 ms: 1.16x slower                                                          |
| pyflate                    | 449 ms                                                       | 522 ms: 1.16x slower                                                          |
| mypy2                      | 762 ms                                                       | 890 ms: 1.17x slower                                                          |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                         |
| telco                      | 6.81 ms                                                      | 8.01 ms: 1.18x slower                                                         |
| coverage                   | 66.1 ms                                                      | 81.8 ms: 1.24x slower                                                         |
| scimark_sor                | 110 ms                                                       | 142 ms: 1.30x slower                                                          |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.04x faster                                                                  |

Benchmark hidden because not significant (6): bench_thread_pool, dask, asyncio_websockets, tornado_http, pathlib, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 96.37% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x