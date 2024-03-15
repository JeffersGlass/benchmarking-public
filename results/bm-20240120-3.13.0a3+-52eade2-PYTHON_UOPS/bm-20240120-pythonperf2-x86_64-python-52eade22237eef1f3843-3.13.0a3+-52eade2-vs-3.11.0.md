
# Results vs. 3.11.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: linux-x86_64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.03x slower
- HPT reliability: 94.26%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 309 ms: 1.08x slower                                                         |
| chameleon      | 7.92 ms                                                      | 8.09 ms: 1.02x slower                                                        |
| docutils       | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 449 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 561 ms: 1.12x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 562 ms: 1.07x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 448 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 715 ms: 1.05x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 266 ms: 1.06x slower                                                         |
| float          | 74.9 ms                                                      | 104 ms: 1.39x slower                                                         |
| nbody          | 92.9 ms                                                      | 130 ms: 1.40x slower                                                         |
| Geometric mean | (ref)                                                        | 1.27x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 25.1 ms: 1.03x slower                                                        |
| regex_dna      | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.64 ms: 1.09x slower                                                        |
| regex_compile  | 156 ms                                                       | 172 ms: 1.10x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.7 us: 1.17x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 150 ms: 1.03x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 31.7 us: 1.02x faster                                                        |
| pickle_pure_python   | 316 us                                                       | 313 us: 1.01x faster                                                         |
| unpickle_pure_python | 238 us                                                       | 243 us: 1.02x slower                                                         |
| unpickle_list        | 4.60 us                                                      | 4.84 us: 1.05x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| pickle               | 9.89 us                                                      | 10.8 us: 1.09x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 62.8 ms: 1.12x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.46 us: 1.13x slower                                                        |
| unpickle             | 13.3 us                                                      | 15.2 us: 1.14x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 94.3 ms: 1.18x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.83 sec: 1.26x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 15.3 ms: 1.39x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 125 us: 4.26x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 377 ms: 1.98x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.5 ms: 1.58x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.1 ms: 1.26x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                        |
| json_loads                 | 28.9 us                                                      | 24.7 us: 1.17x faster                                                        |
| async_tree_none            | 518 ms                                                       | 449 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 561 ms: 1.12x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.72 ms: 1.11x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 167 ms: 1.11x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 104 ms: 1.09x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 562 ms: 1.07x faster                                                         |
| json                       | 5.58 ms                                                      | 5.25 ms: 1.06x faster                                                        |
| richards_super             | 63.6 ms                                                      | 60.0 ms: 1.06x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 448 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| mdp                        | 2.77 sec                                                     | 2.63 sec: 1.05x faster                                                       |
| logging_simple             | 7.24 us                                                      | 6.87 us: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 715 ms: 1.05x faster                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.45 ms: 1.04x faster                                                        |
| sympy_str                  | 337 ms                                                       | 324 ms: 1.04x faster                                                         |
| deepcopy                   | 391 us                                                       | 376 us: 1.04x faster                                                         |
| sympy_integrate            | 25.8 ms                                                      | 24.9 ms: 1.04x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.46 us: 1.03x faster                                                        |
| xml_etree_parse            | 155 ms                                                       | 150 ms: 1.03x faster                                                         |
| unpack_sequence            | 45.7 ns                                                      | 44.4 ns: 1.03x faster                                                        |
| sympy_expand               | 553 ms                                                       | 537 ms: 1.03x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.87 ms: 1.02x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 31.7 us: 1.02x faster                                                        |
| logging_silent             | 100 ns                                                       | 98.5 ns: 1.02x faster                                                        |
| bench_thread_pool          | 1.00 ms                                                      | 982 us: 1.02x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 313 us: 1.01x faster                                                         |
| deepcopy_reduce            | 3.40 us                                                      | 3.36 us: 1.01x faster                                                        |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                        |
| pycparser                  | 1.31 sec                                                     | 1.32 sec: 1.01x slower                                                       |
| create_gc_cycles           | 1.58 ms                                                      | 1.60 ms: 1.02x slower                                                        |
| unpickle_pure_python       | 238 us                                                       | 243 us: 1.02x slower                                                         |
| sqlglot_normalize          | 122 ms                                                       | 124 ms: 1.02x slower                                                         |
| chameleon                  | 7.92 ms                                                      | 8.09 ms: 1.02x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 25.1 ms: 1.03x slower                                                        |
| docutils                   | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                                       |
| chaos                      | 74.9 ms                                                      | 77.8 ms: 1.04x slower                                                        |
| bench_mp_pool              | 4.70 ms                                                      | 4.88 ms: 1.04x slower                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 87.0 ms: 1.04x slower                                                        |
| regex_dna                  | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.84 us: 1.05x slower                                                        |
| meteor_contest             | 131 ms                                                       | 138 ms: 1.06x slower                                                         |
| pidigits                   | 251 ms                                                       | 266 ms: 1.06x slower                                                         |
| dulwich_log                | 67.4 ms                                                      | 71.3 ms: 1.06x slower                                                        |
| nqueens                    | 103 ms                                                       | 109 ms: 1.07x slower                                                         |
| 2to3                       | 287 ms                                                       | 309 ms: 1.08x slower                                                         |
| deepcopy_memo              | 37.5 us                                                      | 40.7 us: 1.08x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 63.9 ms: 1.08x slower                                                        |
| xml_etree_iterparse        | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| richards                   | 49.7 ms                                                      | 54.0 ms: 1.09x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.8 us: 1.09x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.64 ms: 1.09x slower                                                        |
| regex_compile              | 156 ms                                                       | 172 ms: 1.10x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.81 us: 1.12x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 62.8 ms: 1.12x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.46 us: 1.13x slower                                                        |
| go                         | 158 ms                                                       | 179 ms: 1.13x slower                                                         |
| fannkuch                   | 416 ms                                                       | 474 ms: 1.14x slower                                                         |
| unpickle                   | 13.3 us                                                      | 15.2 us: 1.14x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.91 sec: 1.15x slower                                                       |
| pprint_safe_repr           | 805 ms                                                       | 927 ms: 1.15x slower                                                         |
| async_generators           | 322 ms                                                       | 370 ms: 1.15x slower                                                         |
| mypy2                      | 762 ms                                                       | 893 ms: 1.17x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 94.3 ms: 1.18x slower                                                        |
| coverage                   | 66.1 ms                                                      | 80.2 ms: 1.21x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.36 ms: 1.23x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.83 sec: 1.26x slower                                                       |
| scimark_monte_carlo        | 69.8 ms                                                      | 87.8 ms: 1.26x slower                                                        |
| pyflate                    | 449 ms                                                       | 581 ms: 1.29x slower                                                         |
| scimark_sor                | 110 ms                                                       | 146 ms: 1.33x slower                                                         |
| deltablue                  | 3.97 ms                                                      | 5.42 ms: 1.36x slower                                                        |
| mako                       | 11.0 ms                                                      | 15.3 ms: 1.39x slower                                                        |
| float                      | 74.9 ms                                                      | 104 ms: 1.39x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 9.78 ms: 1.40x slower                                                        |
| nbody                      | 92.9 ms                                                      | 130 ms: 1.40x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| scimark_fft                | 281 ms                                                       | 436 ms: 1.55x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.63 ms: 1.63x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 163 ms: 1.71x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (4): tornado_http, dask, raytrace, comprehensions
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.26% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x