
# Results vs. 3.11.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.07x faster
- HPT reliability: 99.79%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 292 ms: 1.02x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.48 ms: 1.06x faster                                                        |
| tornado_http   | 124 ms                                                       | 119 ms: 1.05x faster                                                         |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 430 ms: 1.20x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 543 ms: 1.16x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 425 ms: 1.12x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 543 ms: 1.11x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 696 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 698 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 86.7 ms: 1.07x faster                                                        |
| float          | 74.9 ms                                                      | 78.0 ms: 1.04x slower                                                        |
| pidigits       | 251 ms                                                       | 263 ms: 1.05x slower                                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 141 ms: 1.11x faster                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.53 ms: 1.06x slower                                                        |
| regex_dna      | 227 ms                                                       | 247 ms: 1.09x slower                                                         |
| regex_v8       | 24.4 ms                                                      | 26.8 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.6 us: 1.18x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 212 us: 1.12x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 149 ms: 1.04x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 305 us: 1.04x faster                                                         |
| unpickle_list        | 4.60 us                                                      | 4.67 us: 1.02x slower                                                        |
| pickle_dict          | 32.3 us                                                      | 33.0 us: 1.02x slower                                                        |
| pickle               | 9.89 us                                                      | 10.1 us: 1.03x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.35 sec: 1.04x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 85.1 ms: 1.07x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.3 ms: 1.07x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 116 us: 4.58x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 369 ms: 2.02x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 33.6 ms: 1.63x faster                                                        |
| comprehensions             | 25.1 us                                                      | 16.4 us: 1.53x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                        |
| chaos                      | 74.9 ms                                                      | 61.0 ms: 1.23x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 152 ms: 1.22x faster                                                         |
| async_tree_none            | 518 ms                                                       | 430 ms: 1.20x faster                                                         |
| json_loads                 | 28.9 us                                                      | 24.6 us: 1.18x faster                                                        |
| raytrace                   | 309 ms                                                       | 264 ms: 1.17x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 71.1 ms: 1.17x faster                                                        |
| gc_traversal               | 4.15 ms                                                      | 3.56 ms: 1.16x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 543 ms: 1.16x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 98.6 ms: 1.16x faster                                                        |
| sympy_str                  | 337 ms                                                       | 292 ms: 1.16x faster                                                         |
| nqueens                    | 103 ms                                                       | 88.9 ms: 1.15x faster                                                        |
| unpickle_pure_python       | 238 us                                                       | 212 us: 1.12x faster                                                         |
| sympy_integrate            | 25.8 ms                                                      | 23.1 ms: 1.12x faster                                                        |
| deltablue                  | 3.97 ms                                                      | 3.55 ms: 1.12x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 425 ms: 1.12x faster                                                         |
| mdp                        | 2.77 sec                                                     | 2.49 sec: 1.11x faster                                                       |
| sympy_expand               | 553 ms                                                       | 498 ms: 1.11x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.53 us: 1.11x faster                                                        |
| regex_compile              | 156 ms                                                       | 141 ms: 1.11x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 543 ms: 1.11x faster                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.38 ms: 1.10x faster                                                        |
| hexiom                     | 6.98 ms                                                      | 6.37 ms: 1.10x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 696 ms: 1.08x faster                                                         |
| logging_format             | 7.71 us                                                      | 7.16 us: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 698 ms: 1.07x faster                                                         |
| fannkuch                   | 416 ms                                                       | 387 ms: 1.07x faster                                                         |
| deepcopy                   | 391 us                                                       | 364 us: 1.07x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.78 ms: 1.07x faster                                                        |
| nbody                      | 92.9 ms                                                      | 86.7 ms: 1.07x faster                                                        |
| mako                       | 11.0 ms                                                      | 10.3 ms: 1.07x faster                                                        |
| json                       | 5.58 ms                                                      | 5.26 ms: 1.06x faster                                                        |
| chameleon                  | 7.92 ms                                                      | 7.48 ms: 1.06x faster                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 66.4 ms: 1.05x faster                                                        |
| richards_super             | 63.6 ms                                                      | 60.6 ms: 1.05x faster                                                        |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                                         |
| bench_thread_pool          | 1.00 ms                                                      | 954 us: 1.05x faster                                                         |
| tornado_http               | 124 ms                                                       | 119 ms: 1.05x faster                                                         |
| dask                       | 410 ms                                                       | 395 ms: 1.04x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 149 ms: 1.04x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 305 us: 1.04x faster                                                         |
| deepcopy_reduce            | 3.40 us                                                      | 3.30 us: 1.03x faster                                                        |
| spectral_norm              | 95.1 ms                                                      | 92.6 ms: 1.03x faster                                                        |
| logging_silent             | 100 ns                                                       | 98.4 ns: 1.02x faster                                                        |
| meteor_contest             | 131 ms                                                       | 129 ms: 1.01x faster                                                         |
| pathlib                    | 18.9 ms                                                      | 18.8 ms: 1.01x faster                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.66 sec: 1.01x faster                                                       |
| sqlglot_optimize           | 59.0 ms                                                      | 59.2 ms: 1.00x slower                                                        |
| pprint_safe_repr           | 805 ms                                                       | 812 ms: 1.01x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.67 us: 1.02x slower                                                        |
| unpack_sequence            | 45.7 ns                                                      | 46.4 ns: 1.02x slower                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.13 ms: 1.02x slower                                                        |
| 2to3                       | 287 ms                                                       | 292 ms: 1.02x slower                                                         |
| pickle_dict                | 32.3 us                                                      | 33.0 us: 1.02x slower                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.1 us: 1.03x slower                                                        |
| float                      | 74.9 ms                                                      | 78.0 ms: 1.04x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.35 sec: 1.04x slower                                                       |
| pidigits                   | 251 ms                                                       | 263 ms: 1.05x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.53 ms: 1.06x slower                                                        |
| scimark_fft                | 281 ms                                                       | 297 ms: 1.06x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 85.1 ms: 1.07x slower                                                        |
| go                         | 158 ms                                                       | 169 ms: 1.07x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.71 us: 1.08x slower                                                        |
| regex_dna                  | 227 ms                                                       | 247 ms: 1.09x slower                                                         |
| richards                   | 49.7 ms                                                      | 54.4 ms: 1.10x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 26.8 ms: 1.10x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.6 us: 1.10x slower                                                        |
| pyflate                    | 449 ms                                                       | 505 ms: 1.12x slower                                                         |
| mypy2                      | 762 ms                                                       | 858 ms: 1.13x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| async_generators           | 322 ms                                                       | 366 ms: 1.14x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.04 ms: 1.18x slower                                                        |
| coverage                   | 66.1 ms                                                      | 80.8 ms: 1.22x slower                                                        |
| scimark_sor                | 110 ms                                                       | 143 ms: 1.31x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                                 |

Benchmark hidden because not significant (7): bench_mp_pool, xml_etree_iterparse, docutils, deepcopy_memo, dulwich_log, asyncio_websockets, pycparser
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.79% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.98x