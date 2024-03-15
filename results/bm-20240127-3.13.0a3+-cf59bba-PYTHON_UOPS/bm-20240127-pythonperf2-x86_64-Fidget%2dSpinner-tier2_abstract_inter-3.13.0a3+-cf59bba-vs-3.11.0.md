
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.01x slower
- HPT reliability: 84.91%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 310 ms: 1.08x slower                                                                   |
| chameleon      | 7.92 ms                                                      | 7.83 ms: 1.01x faster                                                                  |
| docutils       | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                                                 |
| tornado_http   | 124 ms                                                       | 127 ms: 1.02x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 441 ms: 1.17x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 554 ms: 1.14x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                                 |
| async_tree_none_tg         | 474 ms                                                       | 441 ms: 1.08x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 561 ms: 1.07x faster                                                                   |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 705 ms: 1.07x faster                                                                   |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 711 ms: 1.05x faster                                                                   |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 265 ms: 1.06x slower                                                                   |
| nbody          | 92.9 ms                                                      | 112 ms: 1.20x slower                                                                   |
| float          | 74.9 ms                                                      | 94.0 ms: 1.25x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.17x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.47 ms: 1.04x slower                                                                  |
| regex_v8       | 24.4 ms                                                      | 25.4 ms: 1.04x slower                                                                  |
| regex_dna      | 227 ms                                                       | 241 ms: 1.06x slower                                                                   |
| regex_compile  | 156 ms                                                       | 167 ms: 1.07x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                                  |
| json_loads           | 28.9 us                                                      | 24.8 us: 1.17x faster                                                                  |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                                                   |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.01x faster                                                                   |
| unpickle_pure_python | 238 us                                                       | 241 us: 1.01x slower                                                                   |
| pickle_dict          | 32.3 us                                                      | 32.8 us: 1.02x slower                                                                  |
| unpickle_list        | 4.60 us                                                      | 4.74 us: 1.03x slower                                                                  |
| xml_etree_iterparse  | 107 ms                                                       | 114 ms: 1.07x slower                                                                   |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                                  |
| xml_etree_process    | 55.9 ms                                                      | 61.6 ms: 1.10x slower                                                                  |
| xml_etree_generate   | 79.7 ms                                                      | 90.0 ms: 1.13x slower                                                                  |
| unpickle             | 13.3 us                                                      | 15.1 us: 1.14x slower                                                                  |
| pickle_list          | 3.94 us                                                      | 4.52 us: 1.15x slower                                                                  |
| tomli_loads          | 2.25 sec                                                     | 2.60 sec: 1.16x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.03x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.19x slower                                                                  |
| python_startup_no_site | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 13.3 ms: 1.21x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 126 us: 4.21x faster                                                                   |
| asyncio_tcp                | 747 ms                                                       | 373 ms: 2.00x faster                                                                   |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                                 |
| generators                 | 54.6 ms                                                      | 34.2 ms: 1.60x faster                                                                  |
| coroutines                 | 27.8 ms                                                      | 22.0 ms: 1.26x faster                                                                  |
| json_dumps                 | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                                  |
| gc_traversal               | 4.15 ms                                                      | 3.53 ms: 1.17x faster                                                                  |
| async_tree_none            | 518 ms                                                       | 441 ms: 1.17x faster                                                                   |
| json_loads                 | 28.9 us                                                      | 24.8 us: 1.17x faster                                                                  |
| async_tree_memoization     | 629 ms                                                       | 554 ms: 1.14x faster                                                                   |
| sympy_sum                  | 186 ms                                                       | 167 ms: 1.11x faster                                                                   |
| scimark_lu                 | 114 ms                                                       | 104 ms: 1.09x faster                                                                   |
| comprehensions             | 25.1 us                                                      | 23.0 us: 1.09x faster                                                                  |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                                 |
| async_tree_none_tg         | 474 ms                                                       | 441 ms: 1.08x faster                                                                   |
| richards_super             | 63.6 ms                                                      | 59.1 ms: 1.08x faster                                                                  |
| sqlglot_parse              | 1.51 ms                                                      | 1.41 ms: 1.07x faster                                                                  |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 561 ms: 1.07x faster                                                                   |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 705 ms: 1.07x faster                                                                   |
| mdp                        | 2.77 sec                                                     | 2.60 sec: 1.07x faster                                                                 |
| json                       | 5.58 ms                                                      | 5.25 ms: 1.06x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 711 ms: 1.05x faster                                                                   |
| sympy_str                  | 337 ms                                                       | 320 ms: 1.05x faster                                                                   |
| sqlglot_transpile          | 1.91 ms                                                      | 1.82 ms: 1.05x faster                                                                  |
| sympy_integrate            | 25.8 ms                                                      | 24.7 ms: 1.04x faster                                                                  |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.04x faster                                                                   |
| raytrace                   | 309 ms                                                       | 298 ms: 1.04x faster                                                                   |
| logging_simple             | 7.24 us                                                      | 6.98 us: 1.04x faster                                                                  |
| crypto_pyaes               | 83.3 ms                                                      | 80.5 ms: 1.03x faster                                                                  |
| chaos                      | 74.9 ms                                                      | 72.8 ms: 1.03x faster                                                                  |
| sympy_expand               | 553 ms                                                       | 537 ms: 1.03x faster                                                                   |
| logging_format             | 7.71 us                                                      | 7.50 us: 1.03x faster                                                                  |
| deepcopy                   | 391 us                                                       | 383 us: 1.02x faster                                                                   |
| asyncio_websockets         | 390 ms                                                       | 385 ms: 1.01x faster                                                                   |
| chameleon                  | 7.92 ms                                                      | 7.83 ms: 1.01x faster                                                                  |
| logging_silent             | 100 ns                                                       | 99.6 ns: 1.01x faster                                                                  |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.01x faster                                                                   |
| pathlib                    | 18.9 ms                                                      | 19.0 ms: 1.00x slower                                                                  |
| deepcopy_reduce            | 3.40 us                                                      | 3.42 us: 1.01x slower                                                                  |
| unpickle_pure_python       | 238 us                                                       | 241 us: 1.01x slower                                                                   |
| pickle_dict                | 32.3 us                                                      | 32.8 us: 1.02x slower                                                                  |
| unpack_sequence            | 45.7 ns                                                      | 46.5 ns: 1.02x slower                                                                  |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                                                 |
| tornado_http               | 124 ms                                                       | 127 ms: 1.02x slower                                                                   |
| create_gc_cycles           | 1.58 ms                                                      | 1.62 ms: 1.02x slower                                                                  |
| docutils                   | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                                                 |
| unpickle_list              | 4.60 us                                                      | 4.74 us: 1.03x slower                                                                  |
| regex_effbot               | 3.34 ms                                                      | 3.47 ms: 1.04x slower                                                                  |
| regex_v8                   | 24.4 ms                                                      | 25.4 ms: 1.04x slower                                                                  |
| meteor_contest             | 131 ms                                                       | 136 ms: 1.04x slower                                                                   |
| pidigits                   | 251 ms                                                       | 265 ms: 1.06x slower                                                                   |
| regex_dna                  | 227 ms                                                       | 241 ms: 1.06x slower                                                                   |
| dulwich_log                | 67.4 ms                                                      | 72.0 ms: 1.07x slower                                                                  |
| fannkuch                   | 416 ms                                                       | 445 ms: 1.07x slower                                                                   |
| xml_etree_iterparse        | 107 ms                                                       | 114 ms: 1.07x slower                                                                   |
| sqlglot_optimize           | 59.0 ms                                                      | 63.3 ms: 1.07x slower                                                                  |
| pickle                     | 9.89 us                                                      | 10.6 us: 1.07x slower                                                                  |
| regex_compile              | 156 ms                                                       | 167 ms: 1.07x slower                                                                   |
| richards                   | 49.7 ms                                                      | 53.5 ms: 1.08x slower                                                                  |
| 2to3                       | 287 ms                                                       | 310 ms: 1.08x slower                                                                   |
| deepcopy_memo              | 37.5 us                                                      | 40.7 us: 1.08x slower                                                                  |
| xml_etree_process          | 55.9 ms                                                      | 61.6 ms: 1.10x slower                                                                  |
| sqlite_synth               | 2.52 us                                                      | 2.80 us: 1.11x slower                                                                  |
| pprint_pformat             | 1.67 sec                                                     | 1.85 sec: 1.11x slower                                                                 |
| pprint_safe_repr           | 805 ms                                                       | 901 ms: 1.12x slower                                                                   |
| xml_etree_generate         | 79.7 ms                                                      | 90.0 ms: 1.13x slower                                                                  |
| unpickle                   | 13.3 us                                                      | 15.1 us: 1.14x slower                                                                  |
| go                         | 158 ms                                                       | 180 ms: 1.14x slower                                                                   |
| pickle_list                | 3.94 us                                                      | 4.52 us: 1.15x slower                                                                  |
| tomli_loads                | 2.25 sec                                                     | 2.60 sec: 1.16x slower                                                                 |
| scimark_monte_carlo        | 69.8 ms                                                      | 81.1 ms: 1.16x slower                                                                  |
| async_generators           | 322 ms                                                       | 374 ms: 1.16x slower                                                                   |
| mypy2                      | 762 ms                                                       | 897 ms: 1.18x slower                                                                   |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.19x slower                                                                  |
| nbody                      | 92.9 ms                                                      | 112 ms: 1.20x slower                                                                   |
| mako                       | 11.0 ms                                                      | 13.3 ms: 1.21x slower                                                                  |
| coverage                   | 66.1 ms                                                      | 80.4 ms: 1.22x slower                                                                  |
| telco                      | 6.81 ms                                                      | 8.29 ms: 1.22x slower                                                                  |
| deltablue                  | 3.97 ms                                                      | 4.86 ms: 1.22x slower                                                                  |
| float                      | 74.9 ms                                                      | 94.0 ms: 1.25x slower                                                                  |
| pyflate                    | 449 ms                                                       | 576 ms: 1.28x slower                                                                   |
| hexiom                     | 6.98 ms                                                      | 9.05 ms: 1.30x slower                                                                  |
| scimark_sor                | 110 ms                                                       | 143 ms: 1.31x slower                                                                   |
| scimark_fft                | 281 ms                                                       | 392 ms: 1.40x slower                                                                   |
| python_startup_no_site     | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                                  |
| spectral_norm              | 95.1 ms                                                      | 138 ms: 1.45x slower                                                                   |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.01 ms: 1.48x slower                                                                  |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                           |

Benchmark hidden because not significant (5): bench_mp_pool, bench_thread_pool, nqueens, dask, sqlglot_normalize
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 84.91% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x