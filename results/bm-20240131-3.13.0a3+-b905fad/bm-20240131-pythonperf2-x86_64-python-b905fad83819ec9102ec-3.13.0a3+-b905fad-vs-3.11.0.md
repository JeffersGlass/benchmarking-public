
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 291 ms: 1.01x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.28 ms: 1.09x faster                                                        |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 428 ms: 1.21x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 541 ms: 1.16x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 543 ms: 1.11x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 429 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.06 sec: 1.10x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 693 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 697 ms: 1.08x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.12x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 85.6 ms: 1.09x faster                                                        |
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                         |
| float          | 74.9 ms                                                      | 79.6 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 139 ms: 1.12x faster                                                         |
| regex_dna      | 227 ms                                                       | 238 ms: 1.04x slower                                                         |
| regex_v8       | 24.4 ms                                                      | 25.8 ms: 1.06x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.67 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.9 us: 1.16x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 209 us: 1.14x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 30.8 us: 1.05x faster                                                        |
| pickle_pure_python   | 316 us                                                       | 303 us: 1.04x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                                         |
| tomli_loads          | 2.25 sec                                                     | 2.23 sec: 1.01x faster                                                       |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 109 ms: 1.02x slower                                                         |
| xml_etree_process    | 55.9 ms                                                      | 58.8 ms: 1.05x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 84.4 ms: 1.06x slower                                                        |
| unpickle_list        | 4.60 us                                                      | 4.89 us: 1.06x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| unpickle             | 13.3 us                                                      | 15.4 us: 1.16x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 117 us: 4.55x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 366 ms: 2.04x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 33.8 ms: 1.62x faster                                                        |
| comprehensions             | 25.1 us                                                      | 16.4 us: 1.53x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 21.8 ms: 1.27x faster                                                        |
| chaos                      | 74.9 ms                                                      | 59.0 ms: 1.27x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 151 ms: 1.23x faster                                                         |
| async_tree_none            | 518 ms                                                       | 428 ms: 1.21x faster                                                         |
| raytrace                   | 309 ms                                                       | 258 ms: 1.20x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 69.8 ms: 1.19x faster                                                        |
| gc_traversal               | 4.15 ms                                                      | 3.51 ms: 1.18x faster                                                        |
| nqueens                    | 103 ms                                                       | 87.5 ms: 1.17x faster                                                        |
| sympy_str                  | 337 ms                                                       | 289 ms: 1.17x faster                                                         |
| json_loads                 | 28.9 us                                                      | 24.9 us: 1.16x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 541 ms: 1.16x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 98.6 ms: 1.16x faster                                                        |
| unpickle_pure_python       | 238 us                                                       | 209 us: 1.14x faster                                                         |
| sympy_expand               | 553 ms                                                       | 494 ms: 1.12x faster                                                         |
| regex_compile              | 156 ms                                                       | 139 ms: 1.12x faster                                                         |
| sympy_integrate            | 25.8 ms                                                      | 23.2 ms: 1.11x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.49 sec: 1.11x faster                                                       |
| deltablue                  | 3.97 ms                                                      | 3.58 ms: 1.11x faster                                                        |
| hexiom                     | 6.98 ms                                                      | 6.31 ms: 1.11x faster                                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 543 ms: 1.11x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 429 ms: 1.10x faster                                                         |
| richards_super             | 63.6 ms                                                      | 57.6 ms: 1.10x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.06 sec: 1.10x faster                                                       |
| logging_simple             | 7.24 us                                                      | 6.59 us: 1.10x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.38 ms: 1.10x faster                                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.06 sec: 1.09x faster                                                       |
| chameleon                  | 7.92 ms                                                      | 7.28 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 693 ms: 1.09x faster                                                         |
| nbody                      | 92.9 ms                                                      | 85.6 ms: 1.09x faster                                                        |
| json                       | 5.58 ms                                                      | 5.16 ms: 1.08x faster                                                        |
| fannkuch                   | 416 ms                                                       | 385 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 697 ms: 1.08x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.79 ms: 1.07x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.23 us: 1.07x faster                                                        |
| logging_silent             | 100 ns                                                       | 94.1 ns: 1.07x faster                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 65.6 ms: 1.06x faster                                                        |
| deepcopy                   | 391 us                                                       | 367 us: 1.06x faster                                                         |
| mako                       | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                        |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                                         |
| pickle_dict                | 32.3 us                                                      | 30.8 us: 1.05x faster                                                        |
| pickle_pure_python         | 316 us                                                       | 303 us: 1.04x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.04x faster                                                         |
| pycparser                  | 1.31 sec                                                     | 1.26 sec: 1.04x faster                                                       |
| dask                       | 410 ms                                                       | 397 ms: 1.03x faster                                                         |
| bench_mp_pool              | 4.70 ms                                                      | 4.56 ms: 1.03x faster                                                        |
| meteor_contest             | 131 ms                                                       | 127 ms: 1.03x faster                                                         |
| tornado_http               | 124 ms                                                       | 121 ms: 1.03x faster                                                         |
| spectral_norm              | 95.1 ms                                                      | 92.6 ms: 1.03x faster                                                        |
| bench_thread_pool          | 1.00 ms                                                      | 975 us: 1.03x faster                                                         |
| deepcopy_reduce            | 3.40 us                                                      | 3.32 us: 1.02x faster                                                        |
| pathlib                    | 18.9 ms                                                      | 18.7 ms: 1.01x faster                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 58.4 ms: 1.01x faster                                                        |
| deepcopy_memo              | 37.5 us                                                      | 37.2 us: 1.01x faster                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.23 sec: 1.01x faster                                                       |
| pprint_pformat             | 1.67 sec                                                     | 1.66 sec: 1.01x faster                                                       |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.12 ms: 1.01x slower                                                        |
| 2to3                       | 287 ms                                                       | 291 ms: 1.01x slower                                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| xml_etree_iterparse        | 107 ms                                                       | 109 ms: 1.02x slower                                                         |
| richards                   | 49.7 ms                                                      | 51.6 ms: 1.04x slower                                                        |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                         |
| regex_dna                  | 227 ms                                                       | 238 ms: 1.04x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 58.8 ms: 1.05x slower                                                        |
| go                         | 158 ms                                                       | 166 ms: 1.06x slower                                                         |
| regex_v8                   | 24.4 ms                                                      | 25.8 ms: 1.06x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 84.4 ms: 1.06x slower                                                        |
| scimark_fft                | 281 ms                                                       | 298 ms: 1.06x slower                                                         |
| float                      | 74.9 ms                                                      | 79.6 ms: 1.06x slower                                                        |
| unpickle_list              | 4.60 us                                                      | 4.89 us: 1.06x slower                                                        |
| unpack_sequence            | 45.7 ns                                                      | 48.8 ns: 1.07x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.72 us: 1.08x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.67 ms: 1.10x slower                                                        |
| pyflate                    | 449 ms                                                       | 502 ms: 1.12x slower                                                         |
| async_generators           | 322 ms                                                       | 360 ms: 1.12x slower                                                         |
| mypy2                      | 762 ms                                                       | 859 ms: 1.13x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| unpickle                   | 13.3 us                                                      | 15.4 us: 1.16x slower                                                        |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.02 ms: 1.18x slower                                                        |
| coverage                   | 66.1 ms                                                      | 78.7 ms: 1.19x slower                                                        |
| scimark_sor                | 110 ms                                                       | 141 ms: 1.28x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                                 |

Benchmark hidden because not significant (4): asyncio_websockets, dulwich_log, docutils, pprint_safe_repr
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x