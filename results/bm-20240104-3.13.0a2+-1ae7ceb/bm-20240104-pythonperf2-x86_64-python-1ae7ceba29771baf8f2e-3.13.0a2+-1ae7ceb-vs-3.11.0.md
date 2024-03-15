
# Results vs. 3.11.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.07x faster
- HPT reliability: 99.96%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 292 ms: 1.02x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                                       |
| tornado_http   | 124 ms                                                       | 118 ms: 1.05x faster                                                         |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 431 ms: 1.20x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 427 ms: 1.11x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 545 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.10x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 693 ms: 1.09x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 698 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 84.6 ms: 1.10x faster                                                        |
| pidigits       | 251 ms                                                       | 263 ms: 1.05x slower                                                         |
| float          | 74.9 ms                                                      | 78.5 ms: 1.05x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 142 ms: 1.10x faster                                                         |
| regex_v8       | 24.4 ms                                                      | 25.4 ms: 1.04x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.58 ms: 1.07x slower                                                        |
| regex_dna      | 227 ms                                                       | 247 ms: 1.09x slower                                                         |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.26x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.8 us: 1.17x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 210 us: 1.14x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 31.4 us: 1.03x faster                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.22 sec: 1.02x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 311 us: 1.02x faster                                                         |
| unpickle_list        | 4.60 us                                                      | 4.66 us: 1.01x slower                                                        |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 59.3 ms: 1.06x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 87.1 ms: 1.09x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.40 us: 1.12x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.9 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.3 ms: 1.06x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 116 us: 4.57x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 365 ms: 2.05x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.2 ms: 1.60x faster                                                        |
| comprehensions             | 25.1 us                                                      | 16.6 us: 1.51x faster                                                        |
| chaos                      | 74.9 ms                                                      | 58.8 ms: 1.27x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.26x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.3 ms: 1.25x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 152 ms: 1.22x faster                                                         |
| async_tree_none            | 518 ms                                                       | 431 ms: 1.20x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 95.9 ms: 1.19x faster                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 70.0 ms: 1.19x faster                                                        |
| nqueens                    | 103 ms                                                       | 86.6 ms: 1.18x faster                                                        |
| json_loads                 | 28.9 us                                                      | 24.8 us: 1.17x faster                                                        |
| sympy_str                  | 337 ms                                                       | 290 ms: 1.16x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.58 ms: 1.16x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                                         |
| raytrace                   | 309 ms                                                       | 270 ms: 1.14x faster                                                         |
| unpickle_pure_python       | 238 us                                                       | 210 us: 1.14x faster                                                         |
| deltablue                  | 3.97 ms                                                      | 3.54 ms: 1.12x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 23.1 ms: 1.12x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 427 ms: 1.11x faster                                                         |
| sympy_expand               | 553 ms                                                       | 498 ms: 1.11x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.54 us: 1.11x faster                                                        |
| hexiom                     | 6.98 ms                                                      | 6.31 ms: 1.11x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.51 sec: 1.10x faster                                                       |
| regex_compile              | 156 ms                                                       | 142 ms: 1.10x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 545 ms: 1.10x faster                                                         |
| nbody                      | 92.9 ms                                                      | 84.6 ms: 1.10x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.10x faster                                                       |
| sqlglot_parse              | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                                        |
| richards_super             | 63.6 ms                                                      | 58.4 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 693 ms: 1.09x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                                       |
| fannkuch                   | 416 ms                                                       | 386 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 698 ms: 1.07x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.79 ms: 1.07x faster                                                        |
| mako                       | 11.0 ms                                                      | 10.3 ms: 1.06x faster                                                        |
| json                       | 5.58 ms                                                      | 5.25 ms: 1.06x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.28 us: 1.06x faster                                                        |
| bench_mp_pool              | 4.70 ms                                                      | 4.46 ms: 1.05x faster                                                        |
| chameleon                  | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                                        |
| tornado_http               | 124 ms                                                       | 118 ms: 1.05x faster                                                         |
| bench_thread_pool          | 1.00 ms                                                      | 951 us: 1.05x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.04x faster                                                         |
| spectral_norm              | 95.1 ms                                                      | 91.4 ms: 1.04x faster                                                        |
| deepcopy                   | 391 us                                                       | 377 us: 1.04x faster                                                         |
| pycparser                  | 1.31 sec                                                     | 1.27 sec: 1.03x faster                                                       |
| scimark_monte_carlo        | 69.8 ms                                                      | 67.8 ms: 1.03x faster                                                        |
| dask                       | 410 ms                                                       | 398 ms: 1.03x faster                                                         |
| pickle_dict                | 32.3 us                                                      | 31.4 us: 1.03x faster                                                        |
| logging_silent             | 100 ns                                                       | 97.6 ns: 1.03x faster                                                        |
| meteor_contest             | 131 ms                                                       | 128 ms: 1.02x faster                                                         |
| tomli_loads                | 2.25 sec                                                     | 2.22 sec: 1.02x faster                                                       |
| pickle_pure_python         | 316 us                                                       | 311 us: 1.02x faster                                                         |
| docutils                   | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                                       |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                                        |
| unpickle_list              | 4.60 us                                                      | 4.66 us: 1.01x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 68.5 ms: 1.02x slower                                                        |
| 2to3                       | 287 ms                                                       | 292 ms: 1.02x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 821 ms: 1.02x slower                                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.62 ms: 1.03x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| deepcopy_memo              | 37.5 us                                                      | 39.0 us: 1.04x slower                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.22 ms: 1.04x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 25.4 ms: 1.04x slower                                                        |
| pidigits                   | 251 ms                                                       | 263 ms: 1.05x slower                                                         |
| float                      | 74.9 ms                                                      | 78.5 ms: 1.05x slower                                                        |
| richards                   | 49.7 ms                                                      | 52.3 ms: 1.05x slower                                                        |
| go                         | 158 ms                                                       | 167 ms: 1.06x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 59.3 ms: 1.06x slower                                                        |
| scimark_fft                | 281 ms                                                       | 299 ms: 1.07x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.58 ms: 1.07x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.70 us: 1.07x slower                                                        |
| regex_dna                  | 227 ms                                                       | 247 ms: 1.09x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 87.1 ms: 1.09x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.40 us: 1.12x slower                                                        |
| pyflate                    | 449 ms                                                       | 503 ms: 1.12x slower                                                         |
| async_generators           | 322 ms                                                       | 360 ms: 1.12x slower                                                         |
| unpickle                   | 13.3 us                                                      | 14.9 us: 1.12x slower                                                        |
| mypy2                      | 762 ms                                                       | 859 ms: 1.13x slower                                                         |
| unpack_sequence            | 45.7 ns                                                      | 53.2 ns: 1.17x slower                                                        |
| python_startup             | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| coverage                   | 66.1 ms                                                      | 78.4 ms: 1.19x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.09 ms: 1.19x slower                                                        |
| scimark_sor                | 110 ms                                                       | 145 ms: 1.32x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                                 |

Benchmark hidden because not significant (5): asyncio_websockets, deepcopy_reduce, xml_etree_iterparse, sqlglot_optimize, pprint_pformat
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x