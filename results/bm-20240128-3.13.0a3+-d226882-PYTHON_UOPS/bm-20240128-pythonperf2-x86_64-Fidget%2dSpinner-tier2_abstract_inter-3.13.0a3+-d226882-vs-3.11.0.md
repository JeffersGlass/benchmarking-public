
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.01x slower
- HPT reliability: 91.58%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 309 ms: 1.08x slower                                                                   |
| chameleon      | 7.92 ms                                                      | 8.09 ms: 1.02x slower                                                                  |
| docutils       | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                                 |
| tornado_http   | 124 ms                                                       | 129 ms: 1.03x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 549 ms: 1.15x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                                 |
| async_tree_memoization_tg  | 600 ms                                                       | 555 ms: 1.08x faster                                                                   |
| async_tree_none_tg         | 474 ms                                                       | 441 ms: 1.08x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 702 ms: 1.07x faster                                                                   |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 707 ms: 1.06x faster                                                                   |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 264 ms: 1.05x slower                                                                   |
| nbody          | 92.9 ms                                                      | 114 ms: 1.23x slower                                                                   |
| float          | 74.9 ms                                                      | 95.3 ms: 1.27x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.18x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                                                  |
| regex_v8       | 24.4 ms                                                      | 26.3 ms: 1.08x slower                                                                  |
| regex_compile  | 156 ms                                                       | 169 ms: 1.08x slower                                                                   |
| regex_dna      | 227 ms                                                       | 251 ms: 1.10x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.22x faster                                                                  |
| json_loads           | 28.9 us                                                      | 24.9 us: 1.16x faster                                                                  |
| xml_etree_parse      | 155 ms                                                       | 144 ms: 1.07x faster                                                                   |
| unpickle_pure_python | 238 us                                                       | 229 us: 1.04x faster                                                                   |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.01x faster                                                                   |
| unpickle_list        | 4.60 us                                                      | 4.75 us: 1.03x slower                                                                  |
| xml_etree_iterparse  | 107 ms                                                       | 112 ms: 1.05x slower                                                                   |
| pickle_dict          | 32.3 us                                                      | 34.6 us: 1.07x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.7 us: 1.08x slower                                                                  |
| unpickle             | 13.3 us                                                      | 14.5 us: 1.09x slower                                                                  |
| xml_etree_process    | 55.9 ms                                                      | 61.6 ms: 1.10x slower                                                                  |
| pickle_list          | 3.94 us                                                      | 4.44 us: 1.13x slower                                                                  |
| xml_etree_generate   | 79.7 ms                                                      | 89.9 ms: 1.13x slower                                                                  |
| tomli_loads          | 2.25 sec                                                     | 2.61 sec: 1.16x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                                  |
| python_startup_no_site | 7.73 ms                                                      | 11.2 ms: 1.44x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 13.6 ms: 1.23x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 127 us: 4.19x faster                                                                   |
| asyncio_tcp                | 747 ms                                                       | 377 ms: 1.98x faster                                                                   |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.94x faster                                                                 |
| generators                 | 54.6 ms                                                      | 34.2 ms: 1.60x faster                                                                  |
| coroutines                 | 27.8 ms                                                      | 22.2 ms: 1.25x faster                                                                  |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.22x faster                                                                  |
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                                                   |
| gc_traversal               | 4.15 ms                                                      | 3.56 ms: 1.16x faster                                                                  |
| json_loads                 | 28.9 us                                                      | 24.9 us: 1.16x faster                                                                  |
| async_tree_memoization     | 629 ms                                                       | 549 ms: 1.15x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                                 |
| sympy_sum                  | 186 ms                                                       | 170 ms: 1.09x faster                                                                   |
| logging_simple             | 7.24 us                                                      | 6.65 us: 1.09x faster                                                                  |
| comprehensions             | 25.1 us                                                      | 23.1 us: 1.08x faster                                                                  |
| unpack_sequence            | 45.7 ns                                                      | 42.2 ns: 1.08x faster                                                                  |
| async_tree_memoization_tg  | 600 ms                                                       | 555 ms: 1.08x faster                                                                   |
| scimark_lu                 | 114 ms                                                       | 106 ms: 1.08x faster                                                                   |
| async_tree_none_tg         | 474 ms                                                       | 441 ms: 1.08x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 702 ms: 1.07x faster                                                                   |
| richards_super             | 63.6 ms                                                      | 59.4 ms: 1.07x faster                                                                  |
| xml_etree_parse            | 155 ms                                                       | 144 ms: 1.07x faster                                                                   |
| logging_format             | 7.71 us                                                      | 7.20 us: 1.07x faster                                                                  |
| mdp                        | 2.77 sec                                                     | 2.61 sec: 1.06x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 707 ms: 1.06x faster                                                                   |
| sqlglot_parse              | 1.51 ms                                                      | 1.44 ms: 1.06x faster                                                                  |
| json                       | 5.58 ms                                                      | 5.31 ms: 1.05x faster                                                                  |
| unpickle_pure_python       | 238 us                                                       | 229 us: 1.04x faster                                                                   |
| raytrace                   | 309 ms                                                       | 298 ms: 1.04x faster                                                                   |
| sympy_str                  | 337 ms                                                       | 325 ms: 1.04x faster                                                                   |
| sympy_integrate            | 25.8 ms                                                      | 25.0 ms: 1.03x faster                                                                  |
| sqlglot_transpile          | 1.91 ms                                                      | 1.85 ms: 1.03x faster                                                                  |
| asyncio_websockets         | 390 ms                                                       | 380 ms: 1.03x faster                                                                   |
| crypto_pyaes               | 83.3 ms                                                      | 81.8 ms: 1.02x faster                                                                  |
| chaos                      | 74.9 ms                                                      | 73.8 ms: 1.02x faster                                                                  |
| sympy_expand               | 553 ms                                                       | 547 ms: 1.01x faster                                                                   |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.01x faster                                                                   |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                                  |
| nqueens                    | 103 ms                                                       | 104 ms: 1.01x slower                                                                   |
| deepcopy_reduce            | 3.40 us                                                      | 3.44 us: 1.01x slower                                                                  |
| chameleon                  | 7.92 ms                                                      | 8.09 ms: 1.02x slower                                                                  |
| create_gc_cycles           | 1.58 ms                                                      | 1.62 ms: 1.03x slower                                                                  |
| pycparser                  | 1.31 sec                                                     | 1.35 sec: 1.03x slower                                                                 |
| unpickle_list              | 4.60 us                                                      | 4.75 us: 1.03x slower                                                                  |
| tornado_http               | 124 ms                                                       | 129 ms: 1.03x slower                                                                   |
| docutils                   | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                                 |
| meteor_contest             | 131 ms                                                       | 137 ms: 1.05x slower                                                                   |
| xml_etree_iterparse        | 107 ms                                                       | 112 ms: 1.05x slower                                                                   |
| pidigits                   | 251 ms                                                       | 264 ms: 1.05x slower                                                                   |
| regex_effbot               | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                                                  |
| pickle_dict                | 32.3 us                                                      | 34.6 us: 1.07x slower                                                                  |
| fannkuch                   | 416 ms                                                       | 446 ms: 1.07x slower                                                                   |
| sqlglot_optimize           | 59.0 ms                                                      | 63.4 ms: 1.07x slower                                                                  |
| regex_v8                   | 24.4 ms                                                      | 26.3 ms: 1.08x slower                                                                  |
| richards                   | 49.7 ms                                                      | 53.5 ms: 1.08x slower                                                                  |
| 2to3                       | 287 ms                                                       | 309 ms: 1.08x slower                                                                   |
| pickle                     | 9.89 us                                                      | 10.7 us: 1.08x slower                                                                  |
| regex_compile              | 156 ms                                                       | 169 ms: 1.08x slower                                                                   |
| dulwich_log                | 67.4 ms                                                      | 73.5 ms: 1.09x slower                                                                  |
| unpickle                   | 13.3 us                                                      | 14.5 us: 1.09x slower                                                                  |
| deepcopy_memo              | 37.5 us                                                      | 41.3 us: 1.10x slower                                                                  |
| xml_etree_process          | 55.9 ms                                                      | 61.6 ms: 1.10x slower                                                                  |
| regex_dna                  | 227 ms                                                       | 251 ms: 1.10x slower                                                                   |
| pprint_pformat             | 1.67 sec                                                     | 1.85 sec: 1.11x slower                                                                 |
| sqlite_synth               | 2.52 us                                                      | 2.81 us: 1.11x slower                                                                  |
| pprint_safe_repr           | 805 ms                                                       | 901 ms: 1.12x slower                                                                   |
| go                         | 158 ms                                                       | 177 ms: 1.12x slower                                                                   |
| pickle_list                | 3.94 us                                                      | 4.44 us: 1.13x slower                                                                  |
| xml_etree_generate         | 79.7 ms                                                      | 89.9 ms: 1.13x slower                                                                  |
| tomli_loads                | 2.25 sec                                                     | 2.61 sec: 1.16x slower                                                                 |
| async_generators           | 322 ms                                                       | 375 ms: 1.17x slower                                                                   |
| scimark_monte_carlo        | 69.8 ms                                                      | 81.9 ms: 1.17x slower                                                                  |
| mypy2                      | 762 ms                                                       | 898 ms: 1.18x slower                                                                   |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                                  |
| coverage                   | 66.1 ms                                                      | 79.3 ms: 1.20x slower                                                                  |
| telco                      | 6.81 ms                                                      | 8.27 ms: 1.22x slower                                                                  |
| nbody                      | 92.9 ms                                                      | 114 ms: 1.23x slower                                                                   |
| deltablue                  | 3.97 ms                                                      | 4.88 ms: 1.23x slower                                                                  |
| mako                       | 11.0 ms                                                      | 13.6 ms: 1.23x slower                                                                  |
| pyflate                    | 449 ms                                                       | 561 ms: 1.25x slower                                                                   |
| float                      | 74.9 ms                                                      | 95.3 ms: 1.27x slower                                                                  |
| hexiom                     | 6.98 ms                                                      | 8.91 ms: 1.28x slower                                                                  |
| scimark_sor                | 110 ms                                                       | 148 ms: 1.35x slower                                                                   |
| scimark_fft                | 281 ms                                                       | 396 ms: 1.41x slower                                                                   |
| python_startup_no_site     | 7.73 ms                                                      | 11.2 ms: 1.44x slower                                                                  |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.10 ms: 1.50x slower                                                                  |
| spectral_norm              | 95.1 ms                                                      | 144 ms: 1.51x slower                                                                   |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                           |

Benchmark hidden because not significant (6): bench_thread_pool, deepcopy, logging_silent, sqlglot_normalize, dask, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 91.58% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x