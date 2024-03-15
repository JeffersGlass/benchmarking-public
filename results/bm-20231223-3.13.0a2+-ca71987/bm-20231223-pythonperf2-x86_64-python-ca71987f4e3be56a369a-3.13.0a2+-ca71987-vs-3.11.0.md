
# Results vs. 3.11.0

- fork: python
- ref: ca71987f4e3be56a369a
- machine: linux-x86_64
- commit hash: ca71987
- commit date: 2023-12-23
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 294 ms: 1.03x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.37 ms: 1.08x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.81 sec: 1.01x faster                                                       |
| tornado_http   | 124 ms                                                       | 118 ms: 1.06x faster                                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 432 ms: 1.20x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 431 ms: 1.10x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 546 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.10x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 692 ms: 1.09x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 699 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 87.7 ms: 1.06x faster                                                        |
| pidigits       | 251 ms                                                       | 264 ms: 1.05x slower                                                         |
| float          | 74.9 ms                                                      | 79.4 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 142 ms: 1.10x faster                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 26.1 ms: 1.07x slower                                                        |
| regex_dna      | 227 ms                                                       | 245 ms: 1.08x slower                                                         |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.2 us: 1.15x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 210 us: 1.13x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 30.4 us: 1.06x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 149 ms: 1.03x faster                                                         |
| tomli_loads          | 2.25 sec                                                     | 2.21 sec: 1.02x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 310 us: 1.02x faster                                                         |
| unpickle_list        | 4.60 us                                                      | 4.65 us: 1.01x slower                                                        |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 59.4 ms: 1.06x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 86.3 ms: 1.08x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.4 us: 1.09x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 120 us: 4.44x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 366 ms: 2.04x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.0 ms: 1.61x faster                                                        |
| comprehensions             | 25.1 us                                                      | 16.4 us: 1.53x faster                                                        |
| chaos                      | 74.9 ms                                                      | 58.8 ms: 1.27x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.1 ms: 1.26x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 152 ms: 1.22x faster                                                         |
| raytrace                   | 309 ms                                                       | 257 ms: 1.20x faster                                                         |
| async_tree_none            | 518 ms                                                       | 432 ms: 1.20x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 69.6 ms: 1.20x faster                                                        |
| nqueens                    | 103 ms                                                       | 87.0 ms: 1.18x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                                         |
| sympy_str                  | 337 ms                                                       | 292 ms: 1.15x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 99.0 ms: 1.15x faster                                                        |
| json_loads                 | 28.9 us                                                      | 25.2 us: 1.15x faster                                                        |
| unpickle_pure_python       | 238 us                                                       | 210 us: 1.13x faster                                                         |
| deltablue                  | 3.97 ms                                                      | 3.53 ms: 1.13x faster                                                        |
| logging_simple             | 7.24 us                                                      | 6.45 us: 1.12x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 23.1 ms: 1.12x faster                                                        |
| sympy_expand               | 553 ms                                                       | 498 ms: 1.11x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.74 ms: 1.11x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.50 sec: 1.11x faster                                                       |
| hexiom                     | 6.98 ms                                                      | 6.33 ms: 1.10x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.37 ms: 1.10x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 431 ms: 1.10x faster                                                         |
| regex_compile              | 156 ms                                                       | 142 ms: 1.10x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 546 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.10x faster                                                       |
| logging_format             | 7.71 us                                                      | 7.06 us: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 692 ms: 1.09x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.08x faster                                                       |
| richards_super             | 63.6 ms                                                      | 59.0 ms: 1.08x faster                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.78 ms: 1.08x faster                                                        |
| chameleon                  | 7.92 ms                                                      | 7.37 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 699 ms: 1.07x faster                                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 65.3 ms: 1.07x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 30.4 us: 1.06x faster                                                        |
| json                       | 5.58 ms                                                      | 5.26 ms: 1.06x faster                                                        |
| fannkuch                   | 416 ms                                                       | 392 ms: 1.06x faster                                                         |
| nbody                      | 92.9 ms                                                      | 87.7 ms: 1.06x faster                                                        |
| tornado_http               | 124 ms                                                       | 118 ms: 1.06x faster                                                         |
| mako                       | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                        |
| deepcopy                   | 391 us                                                       | 374 us: 1.05x faster                                                         |
| spectral_norm              | 95.1 ms                                                      | 90.9 ms: 1.05x faster                                                        |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                                         |
| bench_thread_pool          | 1.00 ms                                                      | 957 us: 1.05x faster                                                         |
| logging_silent             | 100 ns                                                       | 96.3 ns: 1.04x faster                                                        |
| xml_etree_parse            | 155 ms                                                       | 149 ms: 1.03x faster                                                         |
| dask                       | 410 ms                                                       | 396 ms: 1.03x faster                                                         |
| unpack_sequence            | 45.7 ns                                                      | 44.8 ns: 1.02x faster                                                        |
| meteor_contest             | 131 ms                                                       | 128 ms: 1.02x faster                                                         |
| deepcopy_reduce            | 3.40 us                                                      | 3.33 us: 1.02x faster                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.21 sec: 1.02x faster                                                       |
| pickle_pure_python         | 316 us                                                       | 310 us: 1.02x faster                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.64 sec: 1.01x faster                                                       |
| docutils                   | 2.85 sec                                                     | 2.81 sec: 1.01x faster                                                       |
| sqlglot_optimize           | 59.0 ms                                                      | 58.5 ms: 1.01x faster                                                        |
| pathlib                    | 18.9 ms                                                      | 18.8 ms: 1.01x faster                                                        |
| pprint_safe_repr           | 805 ms                                                       | 808 ms: 1.00x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.65 us: 1.01x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.0 us: 1.01x slower                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.60 ms: 1.02x slower                                                        |
| 2to3                       | 287 ms                                                       | 294 ms: 1.03x slower                                                         |
| deepcopy_memo              | 37.5 us                                                      | 38.7 us: 1.03x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.20 ms: 1.03x slower                                                        |
| pidigits                   | 251 ms                                                       | 264 ms: 1.05x slower                                                         |
| scimark_fft                | 281 ms                                                       | 296 ms: 1.05x slower                                                         |
| float                      | 74.9 ms                                                      | 79.4 ms: 1.06x slower                                                        |
| go                         | 158 ms                                                       | 167 ms: 1.06x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 59.4 ms: 1.06x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 26.1 ms: 1.07x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.70 us: 1.07x slower                                                        |
| richards                   | 49.7 ms                                                      | 53.3 ms: 1.07x slower                                                        |
| regex_dna                  | 227 ms                                                       | 245 ms: 1.08x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 86.3 ms: 1.08x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.4 us: 1.09x slower                                                        |
| async_generators           | 322 ms                                                       | 357 ms: 1.11x slower                                                         |
| pyflate                    | 449 ms                                                       | 500 ms: 1.11x slower                                                         |
| mypy2                      | 762 ms                                                       | 857 ms: 1.13x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| python_startup             | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| coverage                   | 66.1 ms                                                      | 78.4 ms: 1.19x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.16 ms: 1.20x slower                                                        |
| scimark_sor                | 110 ms                                                       | 143 ms: 1.31x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                                 |

Benchmark hidden because not significant (5): bench_mp_pool, asyncio_websockets, xml_etree_iterparse, pycparser, dulwich_log
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x