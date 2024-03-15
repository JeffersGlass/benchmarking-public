
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.03x faster \*
- HPT reliability: 76.61%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 300 ms: 1.05x slower                                                          |
| chameleon      | 7.92 ms                                                      | 7.81 ms: 1.01x faster                                                         |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 442 ms: 1.17x faster                                                          |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                          |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 442 ms: 1.07x faster                                                          |
| async_tree_memoization_tg  | 600 ms                                                       | 562 ms: 1.07x faster                                                          |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 708 ms: 1.06x faster                                                          |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 710 ms: 1.06x faster                                                          |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                          |
| float          | 74.9 ms                                                      | 80.4 ms: 1.07x slower                                                         |
| nbody          | 92.9 ms                                                      | 104 ms: 1.12x slower                                                          |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                          |
| regex_effbot   | 3.34 ms                                                      | 3.41 ms: 1.02x slower                                                         |
| regex_dna      | 227 ms                                                       | 238 ms: 1.04x slower                                                          |
| regex_v8       | 24.4 ms                                                      | 26.0 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                         |
| json_loads           | 28.9 us                                                      | 25.0 us: 1.16x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.06x faster                                                          |
| pickle_dict          | 32.3 us                                                      | 30.8 us: 1.05x faster                                                         |
| unpickle_pure_python | 238 us                                                       | 233 us: 1.02x faster                                                          |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.02x faster                                                          |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.00x faster                                                          |
| tomli_loads          | 2.25 sec                                                     | 2.27 sec: 1.01x slower                                                        |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                         |
| xml_etree_process    | 55.9 ms                                                      | 58.6 ms: 1.05x slower                                                         |
| unpickle_list        | 4.60 us                                                      | 4.83 us: 1.05x slower                                                         |
| xml_etree_generate   | 79.7 ms                                                      | 84.6 ms: 1.06x slower                                                         |
| pickle_list          | 3.94 us                                                      | 4.40 us: 1.12x slower                                                         |
| unpickle             | 13.3 us                                                      | 15.2 us: 1.15x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                         |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                  |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 120 us: 4.41x faster                                                          |
| asyncio_tcp                | 747 ms                                                       | 368 ms: 2.03x faster                                                          |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.95x faster                                                        |
| generators                 | 54.6 ms                                                      | 34.6 ms: 1.58x faster                                                         |
| comprehensions             | 25.1 us                                                      | 19.9 us: 1.26x faster                                                         |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                         |
| coroutines                 | 27.8 ms                                                      | 22.2 ms: 1.25x faster                                                         |
| async_tree_none            | 518 ms                                                       | 442 ms: 1.17x faster                                                          |
| json_loads                 | 28.9 us                                                      | 25.0 us: 1.16x faster                                                         |
| sympy_sum                  | 186 ms                                                       | 161 ms: 1.15x faster                                                          |
| scimark_lu                 | 114 ms                                                       | 99.9 ms: 1.14x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                          |
| sympy_str                  | 337 ms                                                       | 300 ms: 1.12x faster                                                          |
| raytrace                   | 309 ms                                                       | 276 ms: 1.12x faster                                                          |
| richards_super             | 63.6 ms                                                      | 57.4 ms: 1.11x faster                                                         |
| sympy_expand               | 553 ms                                                       | 503 ms: 1.10x faster                                                          |
| mdp                        | 2.77 sec                                                     | 2.53 sec: 1.09x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.40 ms: 1.08x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 442 ms: 1.07x faster                                                          |
| deltablue                  | 3.97 ms                                                      | 3.70 ms: 1.07x faster                                                         |
| regex_compile              | 156 ms                                                       | 146 ms: 1.07x faster                                                          |
| async_tree_memoization_tg  | 600 ms                                                       | 562 ms: 1.07x faster                                                          |
| nqueens                    | 103 ms                                                       | 96.3 ms: 1.07x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 78.3 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 708 ms: 1.06x faster                                                          |
| gc_traversal               | 4.15 ms                                                      | 3.90 ms: 1.06x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.83 us: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 24.4 ms: 1.06x faster                                                         |
| chaos                      | 74.9 ms                                                      | 70.9 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 710 ms: 1.06x faster                                                          |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.06x faster                                                          |
| json                       | 5.58 ms                                                      | 5.29 ms: 1.05x faster                                                         |
| pickle_dict                | 32.3 us                                                      | 30.8 us: 1.05x faster                                                         |
| logging_silent             | 100 ns                                                       | 95.8 ns: 1.05x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.83 ms: 1.04x faster                                                         |
| bench_thread_pool          | 1.00 ms                                                      | 968 us: 1.03x faster                                                          |
| fannkuch                   | 416 ms                                                       | 405 ms: 1.03x faster                                                          |
| logging_format             | 7.71 us                                                      | 7.53 us: 1.02x faster                                                         |
| unpickle_pure_python       | 238 us                                                       | 233 us: 1.02x faster                                                          |
| xml_etree_iterparse        | 107 ms                                                       | 105 ms: 1.02x faster                                                          |
| unpack_sequence            | 45.7 ns                                                      | 44.9 ns: 1.02x faster                                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.55 ms: 1.02x faster                                                         |
| deepcopy                   | 391 us                                                       | 385 us: 1.01x faster                                                          |
| chameleon                  | 7.92 ms                                                      | 7.81 ms: 1.01x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 120 ms: 1.01x faster                                                          |
| asyncio_websockets         | 390 ms                                                       | 385 ms: 1.01x faster                                                          |
| pathlib                    | 18.9 ms                                                      | 18.9 ms: 1.00x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.00x faster                                                          |
| meteor_contest             | 131 ms                                                       | 132 ms: 1.01x slower                                                          |
| tomli_loads                | 2.25 sec                                                     | 2.27 sec: 1.01x slower                                                        |
| docutils                   | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                                        |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.01x slower                                                        |
| richards                   | 49.7 ms                                                      | 50.6 ms: 1.02x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.41 ms: 1.02x slower                                                         |
| deepcopy_memo              | 37.5 us                                                      | 38.3 us: 1.02x slower                                                         |
| dulwich_log                | 67.4 ms                                                      | 69.1 ms: 1.02x slower                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.72 sec: 1.04x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 61.2 ms: 1.04x slower                                                         |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                          |
| pprint_safe_repr           | 805 ms                                                       | 840 ms: 1.04x slower                                                          |
| regex_dna                  | 227 ms                                                       | 238 ms: 1.04x slower                                                          |
| pickle                     | 9.89 us                                                      | 10.4 us: 1.05x slower                                                         |
| 2to3                       | 287 ms                                                       | 300 ms: 1.05x slower                                                          |
| xml_etree_process          | 55.9 ms                                                      | 58.6 ms: 1.05x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.83 us: 1.05x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 84.6 ms: 1.06x slower                                                         |
| regex_v8                   | 24.4 ms                                                      | 26.0 ms: 1.06x slower                                                         |
| float                      | 74.9 ms                                                      | 80.4 ms: 1.07x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 7.56 ms: 1.08x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.74 us: 1.09x slower                                                         |
| go                         | 158 ms                                                       | 172 ms: 1.09x slower                                                          |
| scimark_monte_carlo        | 69.8 ms                                                      | 77.8 ms: 1.11x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.40 us: 1.12x slower                                                         |
| nbody                      | 92.9 ms                                                      | 104 ms: 1.12x slower                                                          |
| spectral_norm              | 95.1 ms                                                      | 108 ms: 1.14x slower                                                          |
| async_generators           | 322 ms                                                       | 367 ms: 1.14x slower                                                          |
| pyflate                    | 449 ms                                                       | 514 ms: 1.14x slower                                                          |
| unpickle                   | 13.3 us                                                      | 15.2 us: 1.15x slower                                                         |
| mypy2                      | 762 ms                                                       | 891 ms: 1.17x slower                                                          |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                         |
| coverage                   | 66.1 ms                                                      | 78.3 ms: 1.18x slower                                                         |
| telco                      | 6.81 ms                                                      | 8.09 ms: 1.19x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.89 ms: 1.20x slower                                                         |
| scimark_fft                | 281 ms                                                       | 354 ms: 1.26x slower                                                          |
| scimark_sor                | 110 ms                                                       | 144 ms: 1.31x slower                                                          |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.03x faster                                                                  |

Benchmark hidden because not significant (5): mako, dask, deepcopy_reduce, tornado_http, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 76.61% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x