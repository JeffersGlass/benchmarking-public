
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.03x slower
- HPT reliability: 93.94%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.28x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 316 ms: 1.10x slower                                                                   |
| chameleon      | 7.92 ms                                                      | 8.17 ms: 1.03x slower                                                                  |
| docutils       | 2.85 sec                                                     | 2.92 sec: 1.03x slower                                                                 |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 444 ms: 1.17x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 560 ms: 1.12x faster                                                                   |
| async_tree_memoization_tg  | 600 ms                                                       | 549 ms: 1.09x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.08x faster                                                                 |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 713 ms: 1.06x faster                                                                   |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 716 ms: 1.05x faster                                                                   |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 266 ms: 1.06x slower                                                                   |
| float          | 74.9 ms                                                      | 105 ms: 1.40x slower                                                                   |
| nbody          | 92.9 ms                                                      | 134 ms: 1.44x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.29x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                                  |
| regex_dna      | 227 ms                                                       | 240 ms: 1.05x slower                                                                   |
| regex_v8       | 24.4 ms                                                      | 26.0 ms: 1.07x slower                                                                  |
| regex_compile  | 156 ms                                                       | 171 ms: 1.10x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                                  |
| json_loads           | 28.9 us                                                      | 24.8 us: 1.17x faster                                                                  |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.05x faster                                                                   |
| pickle_pure_python   | 316 us                                                       | 310 us: 1.02x faster                                                                   |
| pickle_dict          | 32.3 us                                                      | 32.4 us: 1.00x slower                                                                  |
| unpickle_pure_python | 238 us                                                       | 242 us: 1.01x slower                                                                   |
| unpickle_list        | 4.60 us                                                      | 4.69 us: 1.02x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| xml_etree_iterparse  | 107 ms                                                       | 118 ms: 1.10x slower                                                                   |
| xml_etree_process    | 55.9 ms                                                      | 62.0 ms: 1.11x slower                                                                  |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.12x slower                                                                  |
| pickle_list          | 3.94 us                                                      | 4.43 us: 1.13x slower                                                                  |
| xml_etree_generate   | 79.7 ms                                                      | 91.7 ms: 1.15x slower                                                                  |
| tomli_loads          | 2.25 sec                                                     | 2.83 sec: 1.26x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.03x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                                  |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 14.8 ms: 1.34x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 128 us: 4.17x faster                                                                   |
| asyncio_tcp                | 747 ms                                                       | 377 ms: 1.98x faster                                                                   |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                                 |
| generators                 | 54.6 ms                                                      | 33.9 ms: 1.61x faster                                                                  |
| coroutines                 | 27.8 ms                                                      | 22.2 ms: 1.25x faster                                                                  |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                                  |
| gc_traversal               | 4.15 ms                                                      | 3.52 ms: 1.18x faster                                                                  |
| json_loads                 | 28.9 us                                                      | 24.8 us: 1.17x faster                                                                  |
| async_tree_none            | 518 ms                                                       | 444 ms: 1.17x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 560 ms: 1.12x faster                                                                   |
| sympy_sum                  | 186 ms                                                       | 169 ms: 1.10x faster                                                                   |
| async_tree_memoization_tg  | 600 ms                                                       | 549 ms: 1.09x faster                                                                   |
| scimark_lu                 | 114 ms                                                       | 105 ms: 1.08x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.08x faster                                                                 |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                                 |
| json                       | 5.58 ms                                                      | 5.28 ms: 1.06x faster                                                                  |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 713 ms: 1.06x faster                                                                   |
| sqlglot_parse              | 1.51 ms                                                      | 1.44 ms: 1.05x faster                                                                  |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.05x faster                                                                   |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 716 ms: 1.05x faster                                                                   |
| logging_simple             | 7.24 us                                                      | 6.94 us: 1.04x faster                                                                  |
| sympy_str                  | 337 ms                                                       | 324 ms: 1.04x faster                                                                   |
| richards_super             | 63.6 ms                                                      | 61.1 ms: 1.04x faster                                                                  |
| logging_format             | 7.71 us                                                      | 7.42 us: 1.04x faster                                                                  |
| asyncio_websockets         | 390 ms                                                       | 376 ms: 1.04x faster                                                                   |
| sympy_expand               | 553 ms                                                       | 535 ms: 1.03x faster                                                                   |
| bench_thread_pool          | 1.00 ms                                                      | 968 us: 1.03x faster                                                                   |
| mdp                        | 2.77 sec                                                     | 2.69 sec: 1.03x faster                                                                 |
| sqlglot_transpile          | 1.91 ms                                                      | 1.85 ms: 1.03x faster                                                                  |
| sympy_integrate            | 25.8 ms                                                      | 25.1 ms: 1.03x faster                                                                  |
| pickle_pure_python         | 316 us                                                       | 310 us: 1.02x faster                                                                   |
| raytrace                   | 309 ms                                                       | 304 ms: 1.02x faster                                                                   |
| deepcopy                   | 391 us                                                       | 384 us: 1.02x faster                                                                   |
| logging_silent             | 100 ns                                                       | 99.8 ns: 1.01x faster                                                                  |
| pickle_dict                | 32.3 us                                                      | 32.4 us: 1.00x slower                                                                  |
| pathlib                    | 18.9 ms                                                      | 19.0 ms: 1.00x slower                                                                  |
| unpickle_pure_python       | 238 us                                                       | 242 us: 1.01x slower                                                                   |
| unpickle_list              | 4.60 us                                                      | 4.69 us: 1.02x slower                                                                  |
| sqlglot_normalize          | 122 ms                                                       | 124 ms: 1.02x slower                                                                   |
| comprehensions             | 25.1 us                                                      | 25.7 us: 1.02x slower                                                                  |
| bench_mp_pool              | 4.70 ms                                                      | 4.82 ms: 1.03x slower                                                                  |
| docutils                   | 2.85 sec                                                     | 2.92 sec: 1.03x slower                                                                 |
| chameleon                  | 7.92 ms                                                      | 8.17 ms: 1.03x slower                                                                  |
| pycparser                  | 1.31 sec                                                     | 1.36 sec: 1.04x slower                                                                 |
| crypto_pyaes               | 83.3 ms                                                      | 86.6 ms: 1.04x slower                                                                  |
| chaos                      | 74.9 ms                                                      | 77.9 ms: 1.04x slower                                                                  |
| pickle                     | 9.89 us                                                      | 10.4 us: 1.05x slower                                                                  |
| regex_effbot               | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                                  |
| regex_dna                  | 227 ms                                                       | 240 ms: 1.05x slower                                                                   |
| meteor_contest             | 131 ms                                                       | 138 ms: 1.06x slower                                                                   |
| pidigits                   | 251 ms                                                       | 266 ms: 1.06x slower                                                                   |
| regex_v8                   | 24.4 ms                                                      | 26.0 ms: 1.07x slower                                                                  |
| dulwich_log                | 67.4 ms                                                      | 71.9 ms: 1.07x slower                                                                  |
| nqueens                    | 103 ms                                                       | 111 ms: 1.08x slower                                                                   |
| sqlglot_optimize           | 59.0 ms                                                      | 64.2 ms: 1.09x slower                                                                  |
| deepcopy_memo              | 37.5 us                                                      | 40.9 us: 1.09x slower                                                                  |
| regex_compile              | 156 ms                                                       | 171 ms: 1.10x slower                                                                   |
| xml_etree_iterparse        | 107 ms                                                       | 118 ms: 1.10x slower                                                                   |
| richards                   | 49.7 ms                                                      | 54.7 ms: 1.10x slower                                                                  |
| 2to3                       | 287 ms                                                       | 316 ms: 1.10x slower                                                                   |
| xml_etree_process          | 55.9 ms                                                      | 62.0 ms: 1.11x slower                                                                  |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.12x slower                                                                  |
| sqlite_synth               | 2.52 us                                                      | 2.82 us: 1.12x slower                                                                  |
| pickle_list                | 3.94 us                                                      | 4.43 us: 1.13x slower                                                                  |
| pprint_pformat             | 1.67 sec                                                     | 1.90 sec: 1.14x slower                                                                 |
| pprint_safe_repr           | 805 ms                                                       | 920 ms: 1.14x slower                                                                   |
| fannkuch                   | 416 ms                                                       | 478 ms: 1.15x slower                                                                   |
| xml_etree_generate         | 79.7 ms                                                      | 91.7 ms: 1.15x slower                                                                  |
| async_generators           | 322 ms                                                       | 370 ms: 1.15x slower                                                                   |
| go                         | 158 ms                                                       | 185 ms: 1.17x slower                                                                   |
| mypy2                      | 762 ms                                                       | 896 ms: 1.18x slower                                                                   |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                                  |
| coverage                   | 66.1 ms                                                      | 80.2 ms: 1.21x slower                                                                  |
| telco                      | 6.81 ms                                                      | 8.54 ms: 1.25x slower                                                                  |
| tomli_loads                | 2.25 sec                                                     | 2.83 sec: 1.26x slower                                                                 |
| scimark_monte_carlo        | 69.8 ms                                                      | 90.4 ms: 1.29x slower                                                                  |
| pyflate                    | 449 ms                                                       | 588 ms: 1.31x slower                                                                   |
| scimark_sor                | 110 ms                                                       | 146 ms: 1.33x slower                                                                   |
| mako                       | 11.0 ms                                                      | 14.8 ms: 1.34x slower                                                                  |
| deltablue                  | 3.97 ms                                                      | 5.50 ms: 1.38x slower                                                                  |
| float                      | 74.9 ms                                                      | 105 ms: 1.40x slower                                                                   |
| hexiom                     | 6.98 ms                                                      | 9.90 ms: 1.42x slower                                                                  |
| nbody                      | 92.9 ms                                                      | 134 ms: 1.44x slower                                                                   |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                                  |
| scimark_fft                | 281 ms                                                       | 424 ms: 1.51x slower                                                                   |
| spectral_norm              | 95.1 ms                                                      | 152 ms: 1.60x slower                                                                   |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.58 ms: 1.62x slower                                                                  |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                           |

Benchmark hidden because not significant (5): tornado_http, dask, unpack_sequence, create_gc_cycles, deepcopy_reduce
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.94% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.28x