
# Results vs. 3.11.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 77a6740
- commit date: 2024-02-14
- overall geometric mean: 1.05x slower \*
- HPT reliability: 99.76%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 319 ms: 1.11x slower                                                         |
| docutils       | 2.85 sec                                                     | 3.06 sec: 1.08x slower                                                       |
| tornado_http   | 124 ms                                                       | 126 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 563 ms: 1.12x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 561 ms: 1.07x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 445 ms: 1.07x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.06x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 717 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 715 ms: 1.05x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 266 ms: 1.06x slower                                                         |
| nbody          | 92.9 ms                                                      | 123 ms: 1.32x slower                                                         |
| float          | 74.9 ms                                                      | 102 ms: 1.36x slower                                                         |
| Geometric mean | (ref)                                                        | 1.24x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 227 ms                                                       | 235 ms: 1.03x slower                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.58 ms: 1.07x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                                        |
| regex_compile  | 156 ms                                                       | 192 ms: 1.23x slower                                                         |
| Geometric mean | (ref)                                                        | 1.10x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.22x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.1 us: 1.15x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.06x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.01x faster                                                         |
| unpickle_list        | 4.60 us                                                      | 4.74 us: 1.03x slower                                                        |
| pickle_dict          | 32.3 us                                                      | 33.6 us: 1.04x slower                                                        |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 116 ms: 1.08x slower                                                         |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.11x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 62.5 ms: 1.12x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 91.2 ms: 1.15x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.87 sec: 1.28x slower                                                       |
| unpickle_pure_python | 238 us                                                       | 310 us: 1.30x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.19x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 14.1 ms: 1.28x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 124 us: 4.28x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 374 ms: 2.00x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.0 ms: 1.61x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.3 ms: 1.25x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.22x faster                                                        |
| gc_traversal               | 4.15 ms                                                      | 3.57 ms: 1.16x faster                                                        |
| json_loads                 | 28.9 us                                                      | 25.1 us: 1.15x faster                                                        |
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 563 ms: 1.12x faster                                                         |
| sympy_sum                  | 186 ms                                                       | 172 ms: 1.08x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 561 ms: 1.07x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 445 ms: 1.07x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.06x faster                                                       |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 717 ms: 1.05x faster                                                         |
| mdp                        | 2.77 sec                                                     | 2.64 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 715 ms: 1.05x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.91 us: 1.05x faster                                                        |
| json                       | 5.58 ms                                                      | 5.34 ms: 1.04x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 25.3 ms: 1.02x faster                                                        |
| comprehensions             | 25.1 us                                                      | 24.5 us: 1.02x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.56 us: 1.02x faster                                                        |
| sympy_str                  | 337 ms                                                       | 330 ms: 1.02x faster                                                         |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| deepcopy                   | 391 us                                                       | 387 us: 1.01x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.01x faster                                                         |
| chaos                      | 74.9 ms                                                      | 75.5 ms: 1.01x slower                                                        |
| sympy_expand               | 553 ms                                                       | 559 ms: 1.01x slower                                                         |
| sqlglot_normalize          | 122 ms                                                       | 123 ms: 1.01x slower                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.53 ms: 1.01x slower                                                        |
| tornado_http               | 124 ms                                                       | 126 ms: 1.02x slower                                                         |
| deltablue                  | 3.97 ms                                                      | 4.05 ms: 1.02x slower                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.4 ms: 1.02x slower                                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.48 us: 1.03x slower                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.96 ms: 1.03x slower                                                        |
| regex_dna                  | 227 ms                                                       | 235 ms: 1.03x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.74 us: 1.03x slower                                                        |
| pickle_dict                | 32.3 us                                                      | 33.6 us: 1.04x slower                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 86.8 ms: 1.04x slower                                                        |
| pidigits                   | 251 ms                                                       | 266 ms: 1.06x slower                                                         |
| meteor_contest             | 131 ms                                                       | 139 ms: 1.07x slower                                                         |
| pickle                     | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.58 ms: 1.07x slower                                                        |
| docutils                   | 2.85 sec                                                     | 3.06 sec: 1.08x slower                                                       |
| richards_super             | 63.6 ms                                                      | 68.5 ms: 1.08x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                                        |
| xml_etree_iterparse        | 107 ms                                                       | 116 ms: 1.08x slower                                                         |
| pycparser                  | 1.31 sec                                                     | 1.43 sec: 1.10x slower                                                       |
| raytrace                   | 309 ms                                                       | 339 ms: 1.10x slower                                                         |
| deepcopy_memo              | 37.5 us                                                      | 41.7 us: 1.11x slower                                                        |
| nqueens                    | 103 ms                                                       | 114 ms: 1.11x slower                                                         |
| 2to3                       | 287 ms                                                       | 319 ms: 1.11x slower                                                         |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.11x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 66.0 ms: 1.12x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 62.5 ms: 1.12x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 76.0 ms: 1.13x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.85 us: 1.13x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 91.2 ms: 1.15x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.96 sec: 1.18x slower                                                       |
| pprint_safe_repr           | 805 ms                                                       | 952 ms: 1.18x slower                                                         |
| async_generators           | 322 ms                                                       | 381 ms: 1.19x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.19x slower                                                        |
| mypy2                      | 762 ms                                                       | 920 ms: 1.21x slower                                                         |
| coverage                   | 66.1 ms                                                      | 80.0 ms: 1.21x slower                                                        |
| scimark_lu                 | 114 ms                                                       | 140 ms: 1.23x slower                                                         |
| fannkuch                   | 416 ms                                                       | 512 ms: 1.23x slower                                                         |
| telco                      | 6.81 ms                                                      | 8.38 ms: 1.23x slower                                                        |
| regex_compile              | 156 ms                                                       | 192 ms: 1.23x slower                                                         |
| richards                   | 49.7 ms                                                      | 62.0 ms: 1.25x slower                                                        |
| go                         | 158 ms                                                       | 197 ms: 1.25x slower                                                         |
| tomli_loads                | 2.25 sec                                                     | 2.87 sec: 1.28x slower                                                       |
| mako                       | 11.0 ms                                                      | 14.1 ms: 1.28x slower                                                        |
| unpickle_pure_python       | 238 us                                                       | 310 us: 1.30x slower                                                         |
| nbody                      | 92.9 ms                                                      | 123 ms: 1.32x slower                                                         |
| float                      | 74.9 ms                                                      | 102 ms: 1.36x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                        |
| unpack_sequence            | 45.7 ns                                                      | 66.9 ns: 1.46x slower                                                        |
| scimark_sor                | 110 ms                                                       | 163 ms: 1.49x slower                                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 104 ms: 1.49x slower                                                         |
| scimark_fft                | 281 ms                                                       | 420 ms: 1.50x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 10.5 ms: 1.50x slower                                                        |
| pyflate                    | 449 ms                                                       | 676 ms: 1.50x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.22 ms: 1.53x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 149 ms: 1.57x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (5): bench_mp_pool, logging_silent, bench_thread_pool, dask, chameleon
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.76% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x