
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.03x faster
- HPT reliability: 76.84%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 299 ms: 1.04x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.69 ms: 1.03x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.89 sec: 1.01x slower                                                       |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 550 ms: 1.14x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 558 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 700 ms: 1.08x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 442 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 710 ms: 1.06x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                         |
| float          | 74.9 ms                                                      | 81.7 ms: 1.09x slower                                                        |
| nbody          | 92.9 ms                                                      | 107 ms: 1.15x slower                                                         |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 147 ms: 1.06x faster                                                         |
| regex_v8       | 24.4 ms                                                      | 24.4 ms: 1.00x faster                                                        |
| regex_dna      | 227 ms                                                       | 232 ms: 1.02x slower                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.46 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.1 us: 1.15x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.06x faster                                                         |
| unpickle_pure_python | 238 us                                                       | 232 us: 1.03x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 308 us: 1.02x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 32.8 us: 1.01x slower                                                        |
| unpickle_list        | 4.60 us                                                      | 4.77 us: 1.04x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.35 sec: 1.04x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 59.6 ms: 1.07x slower                                                        |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 86.6 ms: 1.09x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.12x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.62 us: 1.17x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 12.0 ms: 1.09x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 119 us: 4.47x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 372 ms: 2.01x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 35.6 ms: 1.54x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.5 ms: 1.24x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                        |
| comprehensions             | 25.1 us                                                      | 20.7 us: 1.21x faster                                                        |
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                                         |
| sympy_sum                  | 186 ms                                                       | 159 ms: 1.17x faster                                                         |
| json_loads                 | 28.9 us                                                      | 25.1 us: 1.15x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 550 ms: 1.14x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.65 ms: 1.14x faster                                                        |
| scimark_lu                 | 114 ms                                                       | 101 ms: 1.13x faster                                                         |
| sympy_str                  | 337 ms                                                       | 300 ms: 1.12x faster                                                         |
| richards_super             | 63.6 ms                                                      | 56.9 ms: 1.12x faster                                                        |
| raytrace                   | 309 ms                                                       | 281 ms: 1.10x faster                                                         |
| sympy_expand               | 553 ms                                                       | 505 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                       |
| logging_simple             | 7.24 us                                                      | 6.70 us: 1.08x faster                                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 558 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 700 ms: 1.08x faster                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.41 ms: 1.07x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.58 sec: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 442 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                       |
| sympy_integrate            | 25.8 ms                                                      | 24.2 ms: 1.07x faster                                                        |
| json                       | 5.58 ms                                                      | 5.24 ms: 1.07x faster                                                        |
| nqueens                    | 103 ms                                                       | 96.9 ms: 1.06x faster                                                        |
| regex_compile              | 156 ms                                                       | 147 ms: 1.06x faster                                                         |
| logging_silent             | 100 ns                                                       | 94.9 ns: 1.06x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 710 ms: 1.06x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.06x faster                                                         |
| chaos                      | 74.9 ms                                                      | 71.6 ms: 1.05x faster                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.84 ms: 1.04x faster                                                        |
| deepcopy                   | 391 us                                                       | 378 us: 1.04x faster                                                         |
| chameleon                  | 7.92 ms                                                      | 7.69 ms: 1.03x faster                                                        |
| unpickle_pure_python       | 238 us                                                       | 232 us: 1.03x faster                                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.54 ms: 1.03x faster                                                        |
| sqlglot_normalize          | 122 ms                                                       | 119 ms: 1.03x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 308 us: 1.02x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 81.5 ms: 1.02x faster                                                        |
| bench_thread_pool          | 1.00 ms                                                      | 979 us: 1.02x faster                                                         |
| pycparser                  | 1.31 sec                                                     | 1.28 sec: 1.02x faster                                                       |
| deepcopy_reduce            | 3.40 us                                                      | 3.33 us: 1.02x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.58 us: 1.02x faster                                                        |
| dask                       | 410 ms                                                       | 406 ms: 1.01x faster                                                         |
| regex_v8                   | 24.4 ms                                                      | 24.4 ms: 1.00x faster                                                        |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                        |
| pickle_dict                | 32.3 us                                                      | 32.8 us: 1.01x slower                                                        |
| docutils                   | 2.85 sec                                                     | 2.89 sec: 1.01x slower                                                       |
| deltablue                  | 3.97 ms                                                      | 4.03 ms: 1.02x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 68.7 ms: 1.02x slower                                                        |
| regex_dna                  | 227 ms                                                       | 232 ms: 1.02x slower                                                         |
| richards                   | 49.7 ms                                                      | 50.8 ms: 1.02x slower                                                        |
| meteor_contest             | 131 ms                                                       | 134 ms: 1.03x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.46 ms: 1.04x slower                                                        |
| unpickle_list              | 4.60 us                                                      | 4.77 us: 1.04x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 61.5 ms: 1.04x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.35 sec: 1.04x slower                                                       |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                         |
| 2to3                       | 287 ms                                                       | 299 ms: 1.04x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 59.6 ms: 1.07x slower                                                        |
| bench_mp_pool              | 4.70 ms                                                      | 5.02 ms: 1.07x slower                                                        |
| go                         | 158 ms                                                       | 169 ms: 1.07x slower                                                         |
| pickle                     | 9.89 us                                                      | 10.6 us: 1.07x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.79 sec: 1.07x slower                                                       |
| pprint_safe_repr           | 805 ms                                                       | 865 ms: 1.08x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.72 us: 1.08x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 86.6 ms: 1.09x slower                                                        |
| float                      | 74.9 ms                                                      | 81.7 ms: 1.09x slower                                                        |
| mako                       | 11.0 ms                                                      | 12.0 ms: 1.09x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.12x slower                                                        |
| hexiom                     | 6.98 ms                                                      | 7.86 ms: 1.13x slower                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 79.0 ms: 1.13x slower                                                        |
| nbody                      | 92.9 ms                                                      | 107 ms: 1.15x slower                                                         |
| pyflate                    | 449 ms                                                       | 520 ms: 1.16x slower                                                         |
| async_generators           | 322 ms                                                       | 374 ms: 1.16x slower                                                         |
| mypy2                      | 762 ms                                                       | 887 ms: 1.16x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.62 us: 1.17x slower                                                        |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 116 ms: 1.22x slower                                                         |
| telco                      | 6.81 ms                                                      | 8.34 ms: 1.22x slower                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.14 ms: 1.27x slower                                                        |
| scimark_fft                | 281 ms                                                       | 365 ms: 1.30x slower                                                         |
| coverage                   | 66.1 ms                                                      | 86.7 ms: 1.31x slower                                                        |
| scimark_sor                | 110 ms                                                       | 144 ms: 1.31x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.03x faster                                                                 |

Benchmark hidden because not significant (6): asyncio_websockets, xml_etree_iterparse, fannkuch, tornado_http, deepcopy_memo, unpack_sequence
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 76.84% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x