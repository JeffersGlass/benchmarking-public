
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.03x faster
- HPT reliability: 67.79%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 303 ms: 1.06x slower                                                                   |
| chameleon      | 7.92 ms                                                      | 7.67 ms: 1.03x faster                                                                  |
| docutils       | 2.85 sec                                                     | 2.90 sec: 1.02x slower                                                                 |
| tornado_http   | 124 ms                                                       | 126 ms: 1.01x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 545 ms: 1.15x faster                                                                   |
| async_tree_memoization_tg  | 600 ms                                                       | 548 ms: 1.10x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                                 |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 700 ms: 1.08x faster                                                                   |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 707 ms: 1.06x faster                                                                   |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 263 ms: 1.05x slower                                                                   |
| float          | 74.9 ms                                                      | 82.1 ms: 1.10x slower                                                                  |
| nbody          | 92.9 ms                                                      | 104 ms: 1.12x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 147 ms: 1.06x faster                                                                   |
| regex_v8       | 24.4 ms                                                      | 25.6 ms: 1.05x slower                                                                  |
| regex_dna      | 227 ms                                                       | 241 ms: 1.06x slower                                                                   |
| regex_effbot   | 3.34 ms                                                      | 3.59 ms: 1.07x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                                                  |
| json_loads           | 28.9 us                                                      | 25.3 us: 1.14x faster                                                                  |
| unpickle_pure_python | 238 us                                                       | 224 us: 1.06x faster                                                                   |
| pickle_dict          | 32.3 us                                                      | 31.0 us: 1.04x faster                                                                  |
| pickle_pure_python   | 316 us                                                       | 304 us: 1.04x faster                                                                   |
| xml_etree_parse      | 155 ms                                                       | 149 ms: 1.04x faster                                                                   |
| tomli_loads          | 2.25 sec                                                     | 2.34 sec: 1.04x slower                                                                 |
| xml_etree_process    | 55.9 ms                                                      | 58.6 ms: 1.05x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| xml_etree_generate   | 79.7 ms                                                      | 85.1 ms: 1.07x slower                                                                  |
| unpickle_list        | 4.60 us                                                      | 4.95 us: 1.08x slower                                                                  |
| pickle_list          | 3.94 us                                                      | 4.37 us: 1.11x slower                                                                  |
| unpickle             | 13.3 us                                                      | 15.3 us: 1.15x slower                                                                  |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                                           |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.19x slower                                                                  |
| python_startup_no_site | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 11.8 ms: 1.07x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 122 us: 4.37x faster                                                                   |
| asyncio_tcp                | 747 ms                                                       | 370 ms: 2.02x faster                                                                   |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.95x faster                                                                 |
| generators                 | 54.6 ms                                                      | 34.4 ms: 1.59x faster                                                                  |
| json_dumps                 | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                                                  |
| coroutines                 | 27.8 ms                                                      | 22.5 ms: 1.23x faster                                                                  |
| gc_traversal               | 4.15 ms                                                      | 3.42 ms: 1.21x faster                                                                  |
| comprehensions             | 25.1 us                                                      | 20.8 us: 1.20x faster                                                                  |
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 545 ms: 1.15x faster                                                                   |
| json_loads                 | 28.9 us                                                      | 25.3 us: 1.14x faster                                                                  |
| sympy_sum                  | 186 ms                                                       | 163 ms: 1.14x faster                                                                   |
| scimark_lu                 | 114 ms                                                       | 101 ms: 1.13x faster                                                                   |
| raytrace                   | 309 ms                                                       | 277 ms: 1.12x faster                                                                   |
| sympy_str                  | 337 ms                                                       | 304 ms: 1.11x faster                                                                   |
| richards_super             | 63.6 ms                                                      | 57.4 ms: 1.11x faster                                                                  |
| sqlglot_parse              | 1.51 ms                                                      | 1.38 ms: 1.10x faster                                                                  |
| async_tree_memoization_tg  | 600 ms                                                       | 548 ms: 1.10x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                                 |
| logging_simple             | 7.24 us                                                      | 6.65 us: 1.09x faster                                                                  |
| mdp                        | 2.77 sec                                                     | 2.55 sec: 1.09x faster                                                                 |
| sympy_expand               | 553 ms                                                       | 509 ms: 1.09x faster                                                                   |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                                 |
| deepcopy                   | 391 us                                                       | 363 us: 1.08x faster                                                                   |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 700 ms: 1.08x faster                                                                   |
| chaos                      | 74.9 ms                                                      | 69.8 ms: 1.07x faster                                                                  |
| sqlglot_transpile          | 1.91 ms                                                      | 1.79 ms: 1.07x faster                                                                  |
| unpickle_pure_python       | 238 us                                                       | 224 us: 1.06x faster                                                                   |
| regex_compile              | 156 ms                                                       | 147 ms: 1.06x faster                                                                   |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 707 ms: 1.06x faster                                                                   |
| sympy_integrate            | 25.8 ms                                                      | 24.5 ms: 1.05x faster                                                                  |
| logging_silent             | 100 ns                                                       | 95.6 ns: 1.05x faster                                                                  |
| unpack_sequence            | 45.7 ns                                                      | 43.7 ns: 1.04x faster                                                                  |
| pickle_dict                | 32.3 us                                                      | 31.0 us: 1.04x faster                                                                  |
| nqueens                    | 103 ms                                                       | 98.4 ms: 1.04x faster                                                                  |
| json                       | 5.58 ms                                                      | 5.36 ms: 1.04x faster                                                                  |
| pickle_pure_python         | 316 us                                                       | 304 us: 1.04x faster                                                                   |
| xml_etree_parse            | 155 ms                                                       | 149 ms: 1.04x faster                                                                   |
| deepcopy_reduce            | 3.40 us                                                      | 3.28 us: 1.04x faster                                                                  |
| create_gc_cycles           | 1.58 ms                                                      | 1.52 ms: 1.03x faster                                                                  |
| logging_format             | 7.71 us                                                      | 7.46 us: 1.03x faster                                                                  |
| chameleon                  | 7.92 ms                                                      | 7.67 ms: 1.03x faster                                                                  |
| pathlib                    | 18.9 ms                                                      | 18.4 ms: 1.03x faster                                                                  |
| pycparser                  | 1.31 sec                                                     | 1.27 sec: 1.03x faster                                                                 |
| asyncio_websockets         | 390 ms                                                       | 383 ms: 1.02x faster                                                                   |
| crypto_pyaes               | 83.3 ms                                                      | 82.1 ms: 1.01x faster                                                                  |
| sqlglot_normalize          | 122 ms                                                       | 121 ms: 1.01x faster                                                                   |
| deltablue                  | 3.97 ms                                                      | 3.94 ms: 1.01x faster                                                                  |
| tornado_http               | 124 ms                                                       | 126 ms: 1.01x slower                                                                   |
| docutils                   | 2.85 sec                                                     | 2.90 sec: 1.02x slower                                                                 |
| meteor_contest             | 131 ms                                                       | 134 ms: 1.02x slower                                                                   |
| richards                   | 49.7 ms                                                      | 51.0 ms: 1.03x slower                                                                  |
| fannkuch                   | 416 ms                                                       | 430 ms: 1.03x slower                                                                   |
| tomli_loads                | 2.25 sec                                                     | 2.34 sec: 1.04x slower                                                                 |
| dulwich_log                | 67.4 ms                                                      | 70.4 ms: 1.04x slower                                                                  |
| pidigits                   | 251 ms                                                       | 263 ms: 1.05x slower                                                                   |
| regex_v8                   | 24.4 ms                                                      | 25.6 ms: 1.05x slower                                                                  |
| xml_etree_process          | 55.9 ms                                                      | 58.6 ms: 1.05x slower                                                                  |
| pickle                     | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| sqlglot_optimize           | 59.0 ms                                                      | 62.1 ms: 1.05x slower                                                                  |
| 2to3                       | 287 ms                                                       | 303 ms: 1.06x slower                                                                   |
| regex_dna                  | 227 ms                                                       | 241 ms: 1.06x slower                                                                   |
| bench_mp_pool              | 4.70 ms                                                      | 5.00 ms: 1.06x slower                                                                  |
| pprint_pformat             | 1.67 sec                                                     | 1.78 sec: 1.07x slower                                                                 |
| xml_etree_generate         | 79.7 ms                                                      | 85.1 ms: 1.07x slower                                                                  |
| go                         | 158 ms                                                       | 168 ms: 1.07x slower                                                                   |
| pprint_safe_repr           | 805 ms                                                       | 860 ms: 1.07x slower                                                                   |
| mako                       | 11.0 ms                                                      | 11.8 ms: 1.07x slower                                                                  |
| regex_effbot               | 3.34 ms                                                      | 3.59 ms: 1.07x slower                                                                  |
| unpickle_list              | 4.60 us                                                      | 4.95 us: 1.08x slower                                                                  |
| float                      | 74.9 ms                                                      | 82.1 ms: 1.10x slower                                                                  |
| sqlite_synth               | 2.52 us                                                      | 2.78 us: 1.10x slower                                                                  |
| pickle_list                | 3.94 us                                                      | 4.37 us: 1.11x slower                                                                  |
| nbody                      | 92.9 ms                                                      | 104 ms: 1.12x slower                                                                   |
| scimark_monte_carlo        | 69.8 ms                                                      | 79.0 ms: 1.13x slower                                                                  |
| async_generators           | 322 ms                                                       | 368 ms: 1.14x slower                                                                   |
| pyflate                    | 449 ms                                                       | 517 ms: 1.15x slower                                                                   |
| hexiom                     | 6.98 ms                                                      | 8.04 ms: 1.15x slower                                                                  |
| unpickle                   | 13.3 us                                                      | 15.3 us: 1.15x slower                                                                  |
| mypy2                      | 762 ms                                                       | 892 ms: 1.17x slower                                                                   |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.19x slower                                                                  |
| telco                      | 6.81 ms                                                      | 8.22 ms: 1.21x slower                                                                  |
| coverage                   | 66.1 ms                                                      | 80.7 ms: 1.22x slower                                                                  |
| spectral_norm              | 95.1 ms                                                      | 116 ms: 1.22x slower                                                                   |
| scimark_fft                | 281 ms                                                       | 359 ms: 1.28x slower                                                                   |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.22 ms: 1.29x slower                                                                  |
| scimark_sor                | 110 ms                                                       | 143 ms: 1.30x slower                                                                   |
| python_startup_no_site     | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                                  |
| Geometric mean             | (ref)                                                        | 1.03x faster                                                                           |

Benchmark hidden because not significant (4): bench_thread_pool, dask, deepcopy_memo, xml_etree_iterparse
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 67.79% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.03x