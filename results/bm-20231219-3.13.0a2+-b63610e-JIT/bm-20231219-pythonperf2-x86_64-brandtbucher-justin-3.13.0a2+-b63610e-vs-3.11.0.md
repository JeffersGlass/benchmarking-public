
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.02x faster
- HPT reliability: 67.51%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 302 ms: 1.06x slower                                                 |
| chameleon      | 7.92 ms                                                      | 7.78 ms: 1.02x faster                                                |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                               |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                                 |
| Geometric mean | (ref)                                                        | 1.01x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 447 ms: 1.16x faster                                                 |
| async_tree_memoization     | 629 ms                                                       | 559 ms: 1.13x faster                                                 |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                               |
| async_tree_none_tg         | 474 ms                                                       | 446 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                                 |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.05x faster                                               |
| async_tree_memoization_tg  | 600 ms                                                       | 570 ms: 1.05x faster                                                 |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                 |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 263 ms: 1.05x slower                                                 |
| float          | 74.9 ms                                                      | 82.2 ms: 1.10x slower                                                |
| nbody          | 92.9 ms                                                      | 108 ms: 1.16x slower                                                 |
| Geometric mean | (ref)                                                        | 1.10x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 150 ms: 1.04x faster                                                 |
| regex_v8       | 24.4 ms                                                      | 25.3 ms: 1.04x slower                                                |
| regex_dna      | 227 ms                                                       | 244 ms: 1.07x slower                                                 |
| regex_effbot   | 3.34 ms                                                      | 3.60 ms: 1.08x slower                                                |
| Geometric mean | (ref)                                                        | 1.04x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                |
| json_loads           | 28.9 us                                                      | 24.5 us: 1.18x faster                                                |
| unpickle_pure_python | 238 us                                                       | 221 us: 1.08x faster                                                 |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                                 |
| pickle_pure_python   | 316 us                                                       | 313 us: 1.01x faster                                                 |
| unpickle_list        | 4.60 us                                                      | 4.71 us: 1.03x slower                                                |
| tomli_loads          | 2.25 sec                                                     | 2.36 sec: 1.05x slower                                               |
| xml_etree_process    | 55.9 ms                                                      | 59.5 ms: 1.07x slower                                                |
| pickle_list          | 3.94 us                                                      | 4.23 us: 1.07x slower                                                |
| xml_etree_generate   | 79.7 ms                                                      | 88.0 ms: 1.10x slower                                                |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.11x slower                                                |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                         |

Benchmark hidden because not significant (3): pickle, pickle_dict, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 12.0 ms: 1.09x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 120 us: 4.42x faster                                                 |
| asyncio_tcp                | 747 ms                                                       | 369 ms: 2.02x faster                                                 |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.94x faster                                               |
| generators                 | 54.6 ms                                                      | 34.9 ms: 1.57x faster                                                |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                |
| coroutines                 | 27.8 ms                                                      | 22.5 ms: 1.23x faster                                                |
| comprehensions             | 25.1 us                                                      | 21.0 us: 1.19x faster                                                |
| json_loads                 | 28.9 us                                                      | 24.5 us: 1.18x faster                                                |
| async_tree_none            | 518 ms                                                       | 447 ms: 1.16x faster                                                 |
| sympy_sum                  | 186 ms                                                       | 161 ms: 1.15x faster                                                 |
| async_tree_memoization     | 629 ms                                                       | 559 ms: 1.13x faster                                                 |
| raytrace                   | 309 ms                                                       | 277 ms: 1.12x faster                                                 |
| scimark_lu                 | 114 ms                                                       | 103 ms: 1.11x faster                                                 |
| sympy_str                  | 337 ms                                                       | 304 ms: 1.11x faster                                                 |
| richards_super             | 63.6 ms                                                      | 57.8 ms: 1.10x faster                                                |
| logging_simple             | 7.24 us                                                      | 6.61 us: 1.10x faster                                                |
| sympy_expand               | 553 ms                                                       | 509 ms: 1.09x faster                                                 |
| unpickle_pure_python       | 238 us                                                       | 221 us: 1.08x faster                                                 |
| sqlglot_parse              | 1.51 ms                                                      | 1.41 ms: 1.08x faster                                                |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                               |
| logging_format             | 7.71 us                                                      | 7.24 us: 1.06x faster                                                |
| async_tree_none_tg         | 474 ms                                                       | 446 ms: 1.06x faster                                                 |
| json                       | 5.58 ms                                                      | 5.25 ms: 1.06x faster                                                |
| mdp                        | 2.77 sec                                                     | 2.62 sec: 1.06x faster                                               |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                                 |
| sympy_integrate            | 25.8 ms                                                      | 24.4 ms: 1.06x faster                                                |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.05x faster                                               |
| chaos                      | 74.9 ms                                                      | 71.2 ms: 1.05x faster                                                |
| deepcopy                   | 391 us                                                       | 371 us: 1.05x faster                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 570 ms: 1.05x faster                                                 |
| sqlglot_transpile          | 1.91 ms                                                      | 1.82 ms: 1.05x faster                                                |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                 |
| bench_thread_pool          | 1.00 ms                                                      | 958 us: 1.04x faster                                                 |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.04x faster                                                 |
| regex_compile              | 156 ms                                                       | 150 ms: 1.04x faster                                                 |
| unpack_sequence            | 45.7 ns                                                      | 44.0 ns: 1.04x faster                                                |
| tornado_http               | 124 ms                                                       | 121 ms: 1.03x faster                                                 |
| pycparser                  | 1.31 sec                                                     | 1.28 sec: 1.02x faster                                               |
| chameleon                  | 7.92 ms                                                      | 7.78 ms: 1.02x faster                                                |
| asyncio_websockets         | 390 ms                                                       | 385 ms: 1.01x faster                                                 |
| sqlglot_normalize          | 122 ms                                                       | 120 ms: 1.01x faster                                                 |
| gc_traversal               | 4.15 ms                                                      | 4.10 ms: 1.01x faster                                                |
| pickle_pure_python         | 316 us                                                       | 313 us: 1.01x faster                                                 |
| docutils                   | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                               |
| dulwich_log                | 67.4 ms                                                      | 68.2 ms: 1.01x slower                                                |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                                |
| meteor_contest             | 131 ms                                                       | 133 ms: 1.02x slower                                                 |
| deltablue                  | 3.97 ms                                                      | 4.06 ms: 1.02x slower                                                |
| unpickle_list              | 4.60 us                                                      | 4.71 us: 1.03x slower                                                |
| regex_v8                   | 24.4 ms                                                      | 25.3 ms: 1.04x slower                                                |
| richards                   | 49.7 ms                                                      | 51.7 ms: 1.04x slower                                                |
| bench_mp_pool              | 4.70 ms                                                      | 4.90 ms: 1.04x slower                                                |
| pidigits                   | 251 ms                                                       | 263 ms: 1.05x slower                                                 |
| tomli_loads                | 2.25 sec                                                     | 2.36 sec: 1.05x slower                                               |
| sqlglot_optimize           | 59.0 ms                                                      | 62.0 ms: 1.05x slower                                                |
| fannkuch                   | 416 ms                                                       | 439 ms: 1.05x slower                                                 |
| 2to3                       | 287 ms                                                       | 302 ms: 1.06x slower                                                 |
| pprint_pformat             | 1.67 sec                                                     | 1.77 sec: 1.06x slower                                               |
| xml_etree_process          | 55.9 ms                                                      | 59.5 ms: 1.07x slower                                                |
| pprint_safe_repr           | 805 ms                                                       | 861 ms: 1.07x slower                                                 |
| regex_dna                  | 227 ms                                                       | 244 ms: 1.07x slower                                                 |
| pickle_list                | 3.94 us                                                      | 4.23 us: 1.07x slower                                                |
| regex_effbot               | 3.34 ms                                                      | 3.60 ms: 1.08x slower                                                |
| sqlite_synth               | 2.52 us                                                      | 2.73 us: 1.08x slower                                                |
| mako                       | 11.0 ms                                                      | 12.0 ms: 1.09x slower                                                |
| float                      | 74.9 ms                                                      | 82.2 ms: 1.10x slower                                                |
| go                         | 158 ms                                                       | 174 ms: 1.10x slower                                                 |
| xml_etree_generate         | 79.7 ms                                                      | 88.0 ms: 1.10x slower                                                |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.11x slower                                                |
| scimark_monte_carlo        | 69.8 ms                                                      | 79.1 ms: 1.13x slower                                                |
| hexiom                     | 6.98 ms                                                      | 7.96 ms: 1.14x slower                                                |
| pyflate                    | 449 ms                                                       | 517 ms: 1.15x slower                                                 |
| nbody                      | 92.9 ms                                                      | 108 ms: 1.16x slower                                                 |
| mypy2                      | 762 ms                                                       | 889 ms: 1.17x slower                                                 |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                |
| async_generators           | 322 ms                                                       | 380 ms: 1.18x slower                                                 |
| telco                      | 6.81 ms                                                      | 8.25 ms: 1.21x slower                                                |
| coverage                   | 66.1 ms                                                      | 83.1 ms: 1.26x slower                                                |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.11 ms: 1.26x slower                                                |
| spectral_norm              | 95.1 ms                                                      | 121 ms: 1.27x slower                                                 |
| scimark_sor                | 110 ms                                                       | 144 ms: 1.31x slower                                                 |
| scimark_fft                | 281 ms                                                       | 371 ms: 1.32x slower                                                 |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                |
| Geometric mean             | (ref)                                                        | 1.02x faster                                                         |

Benchmark hidden because not significant (10): logging_silent, create_gc_cycles, dask, deepcopy_reduce, deepcopy_memo, nqueens, pickle, pickle_dict, crypto_pyaes, xml_etree_iterparse
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 67.51% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.03x