
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.03x faster
- HPT reliability: 72.82%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 299 ms: 1.04x slower                                                 |
| chameleon      | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                                |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                               |
| Geometric mean | (ref)                                                        | 1.00x faster                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                 |
| async_tree_memoization     | 629 ms                                                       | 542 ms: 1.16x faster                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 545 ms: 1.10x faster                                                 |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.10x faster                                               |
| async_tree_none_tg         | 474 ms                                                       | 435 ms: 1.09x faster                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 694 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                               |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 702 ms: 1.07x faster                                                 |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 263 ms: 1.05x slower                                                 |
| float          | 74.9 ms                                                      | 82.4 ms: 1.10x slower                                                |
| nbody          | 92.9 ms                                                      | 107 ms: 1.15x slower                                                 |
| Geometric mean | (ref)                                                        | 1.10x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 147 ms: 1.06x faster                                                 |
| regex_effbot   | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                                |
| regex_dna      | 227 ms                                                       | 246 ms: 1.08x slower                                                 |
| regex_v8       | 24.4 ms                                                      | 26.7 ms: 1.09x slower                                                |
| Geometric mean | (ref)                                                        | 1.05x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                                |
| json_loads           | 28.9 us                                                      | 24.8 us: 1.17x faster                                                |
| xml_etree_parse      | 155 ms                                                       | 144 ms: 1.08x faster                                                 |
| pickle_dict          | 32.3 us                                                      | 31.4 us: 1.03x faster                                                |
| pickle_pure_python   | 316 us                                                       | 310 us: 1.02x faster                                                 |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.01x faster                                                 |
| unpickle_pure_python | 238 us                                                       | 235 us: 1.01x faster                                                 |
| tomli_loads          | 2.25 sec                                                     | 2.30 sec: 1.02x slower                                               |
| xml_etree_process    | 55.9 ms                                                      | 58.7 ms: 1.05x slower                                                |
| xml_etree_generate   | 79.7 ms                                                      | 84.9 ms: 1.07x slower                                                |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                |
| unpickle_list        | 4.60 us                                                      | 5.09 us: 1.11x slower                                                |
| pickle_list          | 3.94 us                                                      | 4.38 us: 1.11x slower                                                |
| unpickle             | 13.3 us                                                      | 15.5 us: 1.17x slower                                                |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 11.9 ms: 1.08x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 119 us: 4.47x faster                                                 |
| asyncio_tcp                | 747 ms                                                       | 367 ms: 2.03x faster                                                 |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.60 sec: 1.92x faster                                               |
| generators                 | 54.6 ms                                                      | 33.7 ms: 1.62x faster                                                |
| json_dumps                 | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                                |
| coroutines                 | 27.8 ms                                                      | 23.0 ms: 1.21x faster                                                |
| gc_traversal               | 4.15 ms                                                      | 3.43 ms: 1.21x faster                                                |
| comprehensions             | 25.1 us                                                      | 20.8 us: 1.20x faster                                                |
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                 |
| json_loads                 | 28.9 us                                                      | 24.8 us: 1.17x faster                                                |
| sympy_sum                  | 186 ms                                                       | 159 ms: 1.16x faster                                                 |
| async_tree_memoization     | 629 ms                                                       | 542 ms: 1.16x faster                                                 |
| sympy_str                  | 337 ms                                                       | 298 ms: 1.13x faster                                                 |
| scimark_lu                 | 114 ms                                                       | 102 ms: 1.12x faster                                                 |
| raytrace                   | 309 ms                                                       | 278 ms: 1.11x faster                                                 |
| sympy_expand               | 553 ms                                                       | 501 ms: 1.10x faster                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 545 ms: 1.10x faster                                                 |
| sqlglot_parse              | 1.51 ms                                                      | 1.38 ms: 1.10x faster                                                |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.10x faster                                               |
| async_tree_none_tg         | 474 ms                                                       | 435 ms: 1.09x faster                                                 |
| richards_super             | 63.6 ms                                                      | 58.4 ms: 1.09x faster                                                |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 694 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                               |
| mdp                        | 2.77 sec                                                     | 2.56 sec: 1.08x faster                                               |
| xml_etree_parse            | 155 ms                                                       | 144 ms: 1.08x faster                                                 |
| logging_simple             | 7.24 us                                                      | 6.73 us: 1.08x faster                                                |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 702 ms: 1.07x faster                                                 |
| sqlglot_transpile          | 1.91 ms                                                      | 1.79 ms: 1.07x faster                                                |
| unpack_sequence            | 45.7 ns                                                      | 42.9 ns: 1.06x faster                                                |
| json                       | 5.58 ms                                                      | 5.24 ms: 1.06x faster                                                |
| deepcopy                   | 391 us                                                       | 368 us: 1.06x faster                                                 |
| sympy_integrate            | 25.8 ms                                                      | 24.3 ms: 1.06x faster                                                |
| chaos                      | 74.9 ms                                                      | 70.7 ms: 1.06x faster                                                |
| regex_compile              | 156 ms                                                       | 147 ms: 1.06x faster                                                 |
| chameleon                  | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                                |
| nqueens                    | 103 ms                                                       | 98.5 ms: 1.04x faster                                                |
| logging_format             | 7.71 us                                                      | 7.41 us: 1.04x faster                                                |
| logging_silent             | 100 ns                                                       | 96.7 ns: 1.04x faster                                                |
| create_gc_cycles           | 1.58 ms                                                      | 1.53 ms: 1.03x faster                                                |
| pickle_dict                | 32.3 us                                                      | 31.4 us: 1.03x faster                                                |
| sqlglot_normalize          | 122 ms                                                       | 118 ms: 1.03x faster                                                 |
| deepcopy_reduce            | 3.40 us                                                      | 3.33 us: 1.02x faster                                                |
| pickle_pure_python         | 316 us                                                       | 310 us: 1.02x faster                                                 |
| dask                       | 410 ms                                                       | 403 ms: 1.02x faster                                                 |
| xml_etree_iterparse        | 107 ms                                                       | 105 ms: 1.01x faster                                                 |
| unpickle_pure_python       | 238 us                                                       | 235 us: 1.01x faster                                                 |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                 |
| pathlib                    | 18.9 ms                                                      | 18.8 ms: 1.01x faster                                                |
| deltablue                  | 3.97 ms                                                      | 3.99 ms: 1.01x slower                                                |
| dulwich_log                | 67.4 ms                                                      | 67.9 ms: 1.01x slower                                                |
| deepcopy_memo              | 37.5 us                                                      | 37.8 us: 1.01x slower                                                |
| pycparser                  | 1.31 sec                                                     | 1.32 sec: 1.01x slower                                               |
| docutils                   | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                               |
| meteor_contest             | 131 ms                                                       | 133 ms: 1.02x slower                                                 |
| tomli_loads                | 2.25 sec                                                     | 2.30 sec: 1.02x slower                                               |
| richards                   | 49.7 ms                                                      | 50.9 ms: 1.03x slower                                                |
| sqlglot_optimize           | 59.0 ms                                                      | 61.0 ms: 1.03x slower                                                |
| 2to3                       | 287 ms                                                       | 299 ms: 1.04x slower                                                 |
| pidigits                   | 251 ms                                                       | 263 ms: 1.05x slower                                                 |
| xml_etree_process          | 55.9 ms                                                      | 58.7 ms: 1.05x slower                                                |
| xml_etree_generate         | 79.7 ms                                                      | 84.9 ms: 1.07x slower                                                |
| regex_effbot               | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                                |
| pickle                     | 9.89 us                                                      | 10.6 us: 1.07x slower                                                |
| pprint_safe_repr           | 805 ms                                                       | 864 ms: 1.07x slower                                                 |
| pprint_pformat             | 1.67 sec                                                     | 1.80 sec: 1.08x slower                                               |
| bench_mp_pool              | 4.70 ms                                                      | 5.07 ms: 1.08x slower                                                |
| regex_dna                  | 227 ms                                                       | 246 ms: 1.08x slower                                                 |
| mako                       | 11.0 ms                                                      | 11.9 ms: 1.08x slower                                                |
| sqlite_synth               | 2.52 us                                                      | 2.75 us: 1.09x slower                                                |
| regex_v8                   | 24.4 ms                                                      | 26.7 ms: 1.09x slower                                                |
| float                      | 74.9 ms                                                      | 82.4 ms: 1.10x slower                                                |
| unpickle_list              | 4.60 us                                                      | 5.09 us: 1.11x slower                                                |
| pickle_list                | 3.94 us                                                      | 4.38 us: 1.11x slower                                                |
| go                         | 158 ms                                                       | 178 ms: 1.13x slower                                                 |
| hexiom                     | 6.98 ms                                                      | 7.91 ms: 1.13x slower                                                |
| scimark_monte_carlo        | 69.8 ms                                                      | 79.3 ms: 1.14x slower                                                |
| async_generators           | 322 ms                                                       | 367 ms: 1.14x slower                                                 |
| nbody                      | 92.9 ms                                                      | 107 ms: 1.15x slower                                                 |
| unpickle                   | 13.3 us                                                      | 15.5 us: 1.17x slower                                                |
| mypy2                      | 762 ms                                                       | 891 ms: 1.17x slower                                                 |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                |
| pyflate                    | 449 ms                                                       | 542 ms: 1.21x slower                                                 |
| spectral_norm              | 95.1 ms                                                      | 116 ms: 1.22x slower                                                 |
| telco                      | 6.81 ms                                                      | 8.37 ms: 1.23x slower                                                |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.24 ms: 1.29x slower                                                |
| scimark_sor                | 110 ms                                                       | 142 ms: 1.30x slower                                                 |
| scimark_fft                | 281 ms                                                       | 368 ms: 1.31x slower                                                 |
| coverage                   | 66.1 ms                                                      | 88.0 ms: 1.33x slower                                                |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                |
| Geometric mean             | (ref)                                                        | 1.03x faster                                                         |

Benchmark hidden because not significant (4): bench_thread_pool, tornado_http, crypto_pyaes, fannkuch
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 72.82% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.03x