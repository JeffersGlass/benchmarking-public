
# Results vs. 3.11.0

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.06x faster
- HPT reliability: 99.97%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 294 ms: 1.03x slower                                                 |
| chameleon      | 7.92 ms                                                      | 7.36 ms: 1.08x faster                                                |
| docutils       | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                               |
| tornado_http   | 124 ms                                                       | 118 ms: 1.05x faster                                                 |
| Geometric mean | (ref)                                                        | 1.03x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 437 ms: 1.19x faster                                                 |
| async_tree_memoization     | 629 ms                                                       | 547 ms: 1.15x faster                                                 |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.08x faster                                               |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 713 ms: 1.06x faster                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 568 ms: 1.06x faster                                                 |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                               |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 734 ms: 1.02x faster                                                 |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 84.3 ms: 1.10x faster                                                |
| float          | 74.9 ms                                                      | 76.8 ms: 1.02x slower                                                |
| pidigits       | 251 ms                                                       | 267 ms: 1.06x slower                                                 |
| Geometric mean | (ref)                                                        | 1.00x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                 |
| regex_v8       | 24.4 ms                                                      | 24.7 ms: 1.01x slower                                                |
| regex_effbot   | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                |
| regex_dna      | 227 ms                                                       | 240 ms: 1.06x slower                                                 |
| Geometric mean | (ref)                                                        | 1.01x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                                |
| json_loads           | 28.9 us                                                      | 25.2 us: 1.15x faster                                                |
| unpickle_pure_python | 238 us                                                       | 211 us: 1.13x faster                                                 |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.06x faster                                                 |
| pickle_pure_python   | 316 us                                                       | 308 us: 1.03x faster                                                 |
| pickle_dict          | 32.3 us                                                      | 31.6 us: 1.02x faster                                                |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.02x faster                                                 |
| unpickle_list        | 4.60 us                                                      | 4.54 us: 1.01x faster                                                |
| pickle               | 9.89 us                                                      | 9.98 us: 1.01x slower                                                |
| tomli_loads          | 2.25 sec                                                     | 2.35 sec: 1.05x slower                                               |
| xml_etree_process    | 55.9 ms                                                      | 58.7 ms: 1.05x slower                                                |
| xml_etree_generate   | 79.7 ms                                                      | 85.0 ms: 1.07x slower                                                |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                                |
| pickle_list          | 3.94 us                                                      | 4.34 us: 1.10x slower                                                |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.8 ms: 1.19x slower                                                |
| python_startup_no_site | 7.73 ms                                                      | 11.3 ms: 1.46x slower                                                |
| Geometric mean         | (ref)                                                        | 1.32x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.3 ms: 1.07x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 122 us: 4.35x faster                                                 |
| asyncio_tcp                | 747 ms                                                       | 369 ms: 2.02x faster                                                 |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                               |
| generators                 | 54.6 ms                                                      | 34.8 ms: 1.57x faster                                                |
| comprehensions             | 25.1 us                                                      | 16.6 us: 1.51x faster                                                |
| coroutines                 | 27.8 ms                                                      | 22.0 ms: 1.26x faster                                                |
| chaos                      | 74.9 ms                                                      | 60.2 ms: 1.24x faster                                                |
| json_dumps                 | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                                |
| sympy_sum                  | 186 ms                                                       | 150 ms: 1.23x faster                                                 |
| async_tree_none            | 518 ms                                                       | 437 ms: 1.19x faster                                                 |
| nqueens                    | 103 ms                                                       | 87.9 ms: 1.17x faster                                                |
| gc_traversal               | 4.15 ms                                                      | 3.57 ms: 1.16x faster                                                |
| sympy_str                  | 337 ms                                                       | 291 ms: 1.16x faster                                                 |
| async_tree_memoization     | 629 ms                                                       | 547 ms: 1.15x faster                                                 |
| json_loads                 | 28.9 us                                                      | 25.2 us: 1.15x faster                                                |
| scimark_lu                 | 114 ms                                                       | 99.5 ms: 1.15x faster                                                |
| raytrace                   | 309 ms                                                       | 270 ms: 1.15x faster                                                 |
| unpickle_pure_python       | 238 us                                                       | 211 us: 1.13x faster                                                 |
| sympy_integrate            | 25.8 ms                                                      | 23.0 ms: 1.12x faster                                                |
| sympy_expand               | 553 ms                                                       | 496 ms: 1.11x faster                                                 |
| crypto_pyaes               | 83.3 ms                                                      | 74.9 ms: 1.11x faster                                                |
| logging_simple             | 7.24 us                                                      | 6.54 us: 1.11x faster                                                |
| nbody                      | 92.9 ms                                                      | 84.3 ms: 1.10x faster                                                |
| fannkuch                   | 416 ms                                                       | 380 ms: 1.09x faster                                                 |
| mdp                        | 2.77 sec                                                     | 2.53 sec: 1.09x faster                                               |
| sqlglot_parse              | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                                |
| deltablue                  | 3.97 ms                                                      | 3.64 ms: 1.09x faster                                                |
| hexiom                     | 6.98 ms                                                      | 6.41 ms: 1.09x faster                                                |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.08x faster                                               |
| chameleon                  | 7.92 ms                                                      | 7.36 ms: 1.08x faster                                                |
| scimark_monte_carlo        | 69.8 ms                                                      | 65.0 ms: 1.07x faster                                                |
| regex_compile              | 156 ms                                                       | 146 ms: 1.07x faster                                                 |
| mako                       | 11.0 ms                                                      | 10.3 ms: 1.07x faster                                                |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                 |
| sqlglot_transpile          | 1.91 ms                                                      | 1.79 ms: 1.07x faster                                                |
| deepcopy                   | 391 us                                                       | 368 us: 1.06x faster                                                 |
| logging_format             | 7.71 us                                                      | 7.27 us: 1.06x faster                                                |
| json                       | 5.58 ms                                                      | 5.27 ms: 1.06x faster                                                |
| bench_thread_pool          | 1.00 ms                                                      | 945 us: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 713 ms: 1.06x faster                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 568 ms: 1.06x faster                                                 |
| richards_super             | 63.6 ms                                                      | 60.3 ms: 1.06x faster                                                |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.06x faster                                                 |
| sqlglot_normalize          | 122 ms                                                       | 115 ms: 1.05x faster                                                 |
| tornado_http               | 124 ms                                                       | 118 ms: 1.05x faster                                                 |
| logging_silent             | 100 ns                                                       | 95.6 ns: 1.05x faster                                                |
| bench_mp_pool              | 4.70 ms                                                      | 4.48 ms: 1.05x faster                                                |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                               |
| spectral_norm              | 95.1 ms                                                      | 91.5 ms: 1.04x faster                                                |
| pickle_pure_python         | 316 us                                                       | 308 us: 1.03x faster                                                 |
| sqlglot_optimize           | 59.0 ms                                                      | 57.7 ms: 1.02x faster                                                |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 734 ms: 1.02x faster                                                 |
| pickle_dict                | 32.3 us                                                      | 31.6 us: 1.02x faster                                                |
| xml_etree_iterparse        | 107 ms                                                       | 105 ms: 1.02x faster                                                 |
| deepcopy_reduce            | 3.40 us                                                      | 3.33 us: 1.02x faster                                                |
| pprint_pformat             | 1.67 sec                                                     | 1.64 sec: 1.02x faster                                               |
| unpickle_list              | 4.60 us                                                      | 4.54 us: 1.01x faster                                                |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                 |
| docutils                   | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                               |
| deepcopy_memo              | 37.5 us                                                      | 37.3 us: 1.01x faster                                                |
| meteor_contest             | 131 ms                                                       | 130 ms: 1.00x faster                                                 |
| pickle                     | 9.89 us                                                      | 9.98 us: 1.01x slower                                                |
| dulwich_log                | 67.4 ms                                                      | 68.0 ms: 1.01x slower                                                |
| pycparser                  | 1.31 sec                                                     | 1.32 sec: 1.01x slower                                               |
| regex_v8                   | 24.4 ms                                                      | 24.7 ms: 1.01x slower                                                |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.16 ms: 1.02x slower                                                |
| float                      | 74.9 ms                                                      | 76.8 ms: 1.02x slower                                                |
| 2to3                       | 287 ms                                                       | 294 ms: 1.03x slower                                                 |
| regex_effbot               | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                |
| tomli_loads                | 2.25 sec                                                     | 2.35 sec: 1.05x slower                                               |
| xml_etree_process          | 55.9 ms                                                      | 58.7 ms: 1.05x slower                                                |
| regex_dna                  | 227 ms                                                       | 240 ms: 1.06x slower                                                 |
| sqlite_synth               | 2.52 us                                                      | 2.68 us: 1.06x slower                                                |
| pidigits                   | 251 ms                                                       | 267 ms: 1.06x slower                                                 |
| xml_etree_generate         | 79.7 ms                                                      | 85.0 ms: 1.07x slower                                                |
| scimark_fft                | 281 ms                                                       | 299 ms: 1.07x slower                                                 |
| go                         | 158 ms                                                       | 169 ms: 1.07x slower                                                 |
| richards                   | 49.7 ms                                                      | 54.6 ms: 1.10x slower                                                |
| unpickle                   | 13.3 us                                                      | 14.6 us: 1.10x slower                                                |
| pickle_list                | 3.94 us                                                      | 4.34 us: 1.10x slower                                                |
| async_generators           | 322 ms                                                       | 362 ms: 1.13x slower                                                 |
| mypy2                      | 762 ms                                                       | 858 ms: 1.13x slower                                                 |
| pyflate                    | 449 ms                                                       | 507 ms: 1.13x slower                                                 |
| unpack_sequence            | 45.7 ns                                                      | 51.7 ns: 1.13x slower                                                |
| telco                      | 6.81 ms                                                      | 8.11 ms: 1.19x slower                                                |
| python_startup             | 10.7 ms                                                      | 12.8 ms: 1.19x slower                                                |
| coverage                   | 66.1 ms                                                      | 79.4 ms: 1.20x slower                                                |
| scimark_sor                | 110 ms                                                       | 144 ms: 1.31x slower                                                 |
| python_startup_no_site     | 7.73 ms                                                      | 11.3 ms: 1.46x slower                                                |
| Geometric mean             | (ref)                                                        | 1.06x faster                                                         |

Benchmark hidden because not significant (2): pprint_safe_repr, create_gc_cycles
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.97% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x