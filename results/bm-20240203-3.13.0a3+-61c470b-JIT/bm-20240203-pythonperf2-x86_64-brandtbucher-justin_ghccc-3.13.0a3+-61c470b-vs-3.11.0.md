
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.04x faster \*
- HPT reliability: 89.45%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 298 ms: 1.04x slower                                                       |
| chameleon      | 7.92 ms                                                      | 7.60 ms: 1.04x faster                                                      |
| docutils       | 2.85 sec                                                     | 2.90 sec: 1.02x slower                                                     |
| Geometric mean | (ref)                                                        | 1.00x slower                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 435 ms: 1.19x faster                                                       |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 551 ms: 1.09x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                                     |
| async_tree_none_tg         | 474 ms                                                       | 436 ms: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 698 ms: 1.08x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                     |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                                       |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                       |
| float          | 74.9 ms                                                      | 80.5 ms: 1.07x slower                                                      |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                       |
| regex_v8       | 24.4 ms                                                      | 26.1 ms: 1.07x slower                                                      |
| regex_effbot   | 3.34 ms                                                      | 3.61 ms: 1.08x slower                                                      |
| regex_dna      | 227 ms                                                       | 248 ms: 1.09x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                      |
| json_loads           | 28.9 us                                                      | 25.0 us: 1.16x faster                                                      |
| pickle_dict          | 32.3 us                                                      | 30.9 us: 1.05x faster                                                      |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 230 us: 1.04x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 307 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.02x faster                                                       |
| tomli_loads          | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                                     |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| xml_etree_process    | 55.9 ms                                                      | 59.1 ms: 1.06x slower                                                      |
| unpickle_list        | 4.60 us                                                      | 4.93 us: 1.07x slower                                                      |
| xml_etree_generate   | 79.7 ms                                                      | 85.9 ms: 1.08x slower                                                      |
| pickle_list          | 3.94 us                                                      | 4.46 us: 1.13x slower                                                      |
| unpickle             | 13.3 us                                                      | 15.1 us: 1.14x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                      |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 11.6 ms: 1.05x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 121 us: 4.41x faster                                                       |
| asyncio_tcp                | 747 ms                                                       | 370 ms: 2.02x faster                                                       |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                     |
| generators                 | 54.6 ms                                                      | 34.4 ms: 1.59x faster                                                      |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                      |
| comprehensions             | 25.1 us                                                      | 20.3 us: 1.23x faster                                                      |
| coroutines                 | 27.8 ms                                                      | 22.7 ms: 1.23x faster                                                      |
| async_tree_none            | 518 ms                                                       | 435 ms: 1.19x faster                                                       |
| sympy_sum                  | 186 ms                                                       | 158 ms: 1.17x faster                                                       |
| json_loads                 | 28.9 us                                                      | 25.0 us: 1.16x faster                                                      |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                                       |
| raytrace                   | 309 ms                                                       | 270 ms: 1.15x faster                                                       |
| sympy_str                  | 337 ms                                                       | 297 ms: 1.13x faster                                                       |
| richards_super             | 63.6 ms                                                      | 56.4 ms: 1.13x faster                                                      |
| chaos                      | 74.9 ms                                                      | 66.8 ms: 1.12x faster                                                      |
| scimark_lu                 | 114 ms                                                       | 102 ms: 1.12x faster                                                       |
| crypto_pyaes               | 83.3 ms                                                      | 75.0 ms: 1.11x faster                                                      |
| sympy_expand               | 553 ms                                                       | 501 ms: 1.10x faster                                                       |
| logging_simple             | 7.24 us                                                      | 6.57 us: 1.10x faster                                                      |
| sqlglot_parse              | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                                      |
| async_tree_memoization_tg  | 600 ms                                                       | 551 ms: 1.09x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                                     |
| async_tree_none_tg         | 474 ms                                                       | 436 ms: 1.09x faster                                                       |
| mdp                        | 2.77 sec                                                     | 2.55 sec: 1.09x faster                                                     |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 698 ms: 1.08x faster                                                       |
| json                       | 5.58 ms                                                      | 5.18 ms: 1.08x faster                                                      |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                     |
| regex_compile              | 156 ms                                                       | 146 ms: 1.07x faster                                                       |
| nqueens                    | 103 ms                                                       | 95.8 ms: 1.07x faster                                                      |
| sympy_integrate            | 25.8 ms                                                      | 24.1 ms: 1.07x faster                                                      |
| gc_traversal               | 4.15 ms                                                      | 3.88 ms: 1.07x faster                                                      |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                                       |
| logging_format             | 7.71 us                                                      | 7.27 us: 1.06x faster                                                      |
| sqlglot_transpile          | 1.91 ms                                                      | 1.81 ms: 1.06x faster                                                      |
| deepcopy                   | 391 us                                                       | 371 us: 1.06x faster                                                       |
| logging_silent             | 100 ns                                                       | 95.8 ns: 1.05x faster                                                      |
| pickle_dict                | 32.3 us                                                      | 30.9 us: 1.05x faster                                                      |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.04x faster                                                       |
| chameleon                  | 7.92 ms                                                      | 7.60 ms: 1.04x faster                                                      |
| bench_thread_pool          | 1.00 ms                                                      | 964 us: 1.04x faster                                                       |
| unpickle_pure_python       | 238 us                                                       | 230 us: 1.04x faster                                                       |
| create_gc_cycles           | 1.58 ms                                                      | 1.52 ms: 1.04x faster                                                      |
| deepcopy_reduce            | 3.40 us                                                      | 3.29 us: 1.03x faster                                                      |
| pickle_pure_python         | 316 us                                                       | 307 us: 1.03x faster                                                       |
| fannkuch                   | 416 ms                                                       | 409 ms: 1.02x faster                                                       |
| pycparser                  | 1.31 sec                                                     | 1.29 sec: 1.02x faster                                                     |
| xml_etree_iterparse        | 107 ms                                                       | 105 ms: 1.02x faster                                                       |
| deltablue                  | 3.97 ms                                                      | 3.91 ms: 1.02x faster                                                      |
| dask                       | 410 ms                                                       | 404 ms: 1.02x faster                                                       |
| pathlib                    | 18.9 ms                                                      | 18.7 ms: 1.01x faster                                                      |
| sqlglot_normalize          | 122 ms                                                       | 120 ms: 1.01x faster                                                       |
| meteor_contest             | 131 ms                                                       | 131 ms: 1.01x slower                                                       |
| dulwich_log                | 67.4 ms                                                      | 67.9 ms: 1.01x slower                                                      |
| deepcopy_memo              | 37.5 us                                                      | 37.9 us: 1.01x slower                                                      |
| docutils                   | 2.85 sec                                                     | 2.90 sec: 1.02x slower                                                     |
| richards                   | 49.7 ms                                                      | 50.6 ms: 1.02x slower                                                      |
| tomli_loads                | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                                     |
| pickle                     | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| 2to3                       | 287 ms                                                       | 298 ms: 1.04x slower                                                       |
| sqlglot_optimize           | 59.0 ms                                                      | 61.5 ms: 1.04x slower                                                      |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                       |
| mako                       | 11.0 ms                                                      | 11.6 ms: 1.05x slower                                                      |
| xml_etree_process          | 55.9 ms                                                      | 59.1 ms: 1.06x slower                                                      |
| pprint_safe_repr           | 805 ms                                                       | 858 ms: 1.07x slower                                                       |
| regex_v8                   | 24.4 ms                                                      | 26.1 ms: 1.07x slower                                                      |
| go                         | 158 ms                                                       | 168 ms: 1.07x slower                                                       |
| unpickle_list              | 4.60 us                                                      | 4.93 us: 1.07x slower                                                      |
| float                      | 74.9 ms                                                      | 80.5 ms: 1.07x slower                                                      |
| pprint_pformat             | 1.67 sec                                                     | 1.79 sec: 1.08x slower                                                     |
| xml_etree_generate         | 79.7 ms                                                      | 85.9 ms: 1.08x slower                                                      |
| regex_effbot               | 3.34 ms                                                      | 3.61 ms: 1.08x slower                                                      |
| scimark_monte_carlo        | 69.8 ms                                                      | 75.8 ms: 1.09x slower                                                      |
| sqlite_synth               | 2.52 us                                                      | 2.74 us: 1.09x slower                                                      |
| bench_mp_pool              | 4.70 ms                                                      | 5.11 ms: 1.09x slower                                                      |
| regex_dna                  | 227 ms                                                       | 248 ms: 1.09x slower                                                       |
| hexiom                     | 6.98 ms                                                      | 7.60 ms: 1.09x slower                                                      |
| pyflate                    | 449 ms                                                       | 506 ms: 1.13x slower                                                       |
| pickle_list                | 3.94 us                                                      | 4.46 us: 1.13x slower                                                      |
| unpickle                   | 13.3 us                                                      | 15.1 us: 1.14x slower                                                      |
| async_generators           | 322 ms                                                       | 366 ms: 1.14x slower                                                       |
| mypy2                      | 762 ms                                                       | 889 ms: 1.17x slower                                                       |
| spectral_norm              | 95.1 ms                                                      | 112 ms: 1.18x slower                                                       |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                      |
| telco                      | 6.81 ms                                                      | 8.11 ms: 1.19x slower                                                      |
| coverage                   | 66.1 ms                                                      | 79.3 ms: 1.20x slower                                                      |
| scimark_fft                | 281 ms                                                       | 346 ms: 1.23x slower                                                       |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.03 ms: 1.24x slower                                                      |
| scimark_sor                | 110 ms                                                       | 140 ms: 1.28x slower                                                       |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.04x faster                                                               |

Benchmark hidden because not significant (4): asyncio_websockets, tornado_http, unpack_sequence, nbody
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 89.45% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x