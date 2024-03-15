
# Results vs. 3.11.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.06x faster
- HPT reliability: 99.95%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 295 ms: 1.03x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.40 ms: 1.07x faster                                                        |
| tornado_http   | 124 ms                                                       | 118 ms: 1.05x faster                                                         |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 432 ms: 1.20x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 544 ms: 1.10x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 430 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 695 ms: 1.08x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 698 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 91.2 ms: 1.02x faster                                                        |
| float          | 74.9 ms                                                      | 78.8 ms: 1.05x slower                                                        |
| pidigits       | 251 ms                                                       | 264 ms: 1.05x slower                                                         |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 141 ms: 1.11x faster                                                         |
| regex_v8       | 24.4 ms                                                      | 26.1 ms: 1.07x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.64 ms: 1.09x slower                                                        |
| regex_dna      | 227 ms                                                       | 256 ms: 1.12x slower                                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.27x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.7 us: 1.13x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 222 us: 1.07x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.05x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 310 us: 1.02x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 31.8 us: 1.02x faster                                                        |
| pickle               | 9.89 us                                                      | 9.99 us: 1.01x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                                       |
| unpickle_list        | 4.60 us                                                      | 4.69 us: 1.02x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 57.9 ms: 1.04x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.19 us: 1.06x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 85.4 ms: 1.07x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.5 us: 1.10x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.1 ms: 1.09x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 116 us: 4.59x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 367 ms: 2.04x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 35.6 ms: 1.54x faster                                                        |
| comprehensions             | 25.1 us                                                      | 16.4 us: 1.53x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.27x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.3 ms: 1.24x faster                                                        |
| chaos                      | 74.9 ms                                                      | 60.3 ms: 1.24x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 151 ms: 1.23x faster                                                         |
| async_tree_none            | 518 ms                                                       | 432 ms: 1.20x faster                                                         |
| raytrace                   | 309 ms                                                       | 259 ms: 1.20x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 70.3 ms: 1.18x faster                                                        |
| nqueens                    | 103 ms                                                       | 87.4 ms: 1.17x faster                                                        |
| gc_traversal               | 4.15 ms                                                      | 3.56 ms: 1.16x faster                                                        |
| scimark_lu                 | 114 ms                                                       | 98.2 ms: 1.16x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                                         |
| sympy_str                  | 337 ms                                                       | 293 ms: 1.15x faster                                                         |
| json_loads                 | 28.9 us                                                      | 25.7 us: 1.13x faster                                                        |
| deltablue                  | 3.97 ms                                                      | 3.54 ms: 1.12x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 23.1 ms: 1.12x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.49 sec: 1.11x faster                                                       |
| regex_compile              | 156 ms                                                       | 141 ms: 1.11x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.56 us: 1.10x faster                                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 544 ms: 1.10x faster                                                         |
| sympy_expand               | 553 ms                                                       | 502 ms: 1.10x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 430 ms: 1.10x faster                                                         |
| hexiom                     | 6.98 ms                                                      | 6.35 ms: 1.10x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| mako                       | 11.0 ms                                                      | 10.1 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 695 ms: 1.08x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 698 ms: 1.07x faster                                                         |
| unpickle_pure_python       | 238 us                                                       | 222 us: 1.07x faster                                                         |
| chameleon                  | 7.92 ms                                                      | 7.40 ms: 1.07x faster                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 65.3 ms: 1.07x faster                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.80 ms: 1.06x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.27 us: 1.06x faster                                                        |
| deepcopy                   | 391 us                                                       | 369 us: 1.06x faster                                                         |
| json                       | 5.58 ms                                                      | 5.29 ms: 1.06x faster                                                        |
| bench_thread_pool          | 1.00 ms                                                      | 947 us: 1.06x faster                                                         |
| tornado_http               | 124 ms                                                       | 118 ms: 1.05x faster                                                         |
| fannkuch                   | 416 ms                                                       | 395 ms: 1.05x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.05x faster                                                         |
| spectral_norm              | 95.1 ms                                                      | 91.2 ms: 1.04x faster                                                        |
| richards_super             | 63.6 ms                                                      | 61.2 ms: 1.04x faster                                                        |
| logging_silent             | 100 ns                                                       | 96.5 ns: 1.04x faster                                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.30 us: 1.03x faster                                                        |
| bench_mp_pool              | 4.70 ms                                                      | 4.57 ms: 1.03x faster                                                        |
| dask                       | 410 ms                                                       | 400 ms: 1.03x faster                                                         |
| meteor_contest             | 131 ms                                                       | 128 ms: 1.02x faster                                                         |
| nbody                      | 92.9 ms                                                      | 91.2 ms: 1.02x faster                                                        |
| pickle_pure_python         | 316 us                                                       | 310 us: 1.02x faster                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.64 sec: 1.02x faster                                                       |
| deepcopy_memo              | 37.5 us                                                      | 36.9 us: 1.02x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 31.8 us: 1.02x faster                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 58.8 ms: 1.00x faster                                                        |
| pickle                     | 9.89 us                                                      | 9.99 us: 1.01x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                                       |
| unpickle_list              | 4.60 us                                                      | 4.69 us: 1.02x slower                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.18 ms: 1.03x slower                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.62 ms: 1.03x slower                                                        |
| 2to3                       | 287 ms                                                       | 295 ms: 1.03x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 57.9 ms: 1.04x slower                                                        |
| float                      | 74.9 ms                                                      | 78.8 ms: 1.05x slower                                                        |
| pidigits                   | 251 ms                                                       | 264 ms: 1.05x slower                                                         |
| unpack_sequence            | 45.7 ns                                                      | 48.2 ns: 1.06x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.19 us: 1.06x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 26.1 ms: 1.07x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 85.4 ms: 1.07x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.71 us: 1.07x slower                                                        |
| go                         | 158 ms                                                       | 169 ms: 1.08x slower                                                         |
| scimark_fft                | 281 ms                                                       | 305 ms: 1.09x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.64 ms: 1.09x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.5 us: 1.10x slower                                                        |
| richards                   | 49.7 ms                                                      | 54.8 ms: 1.10x slower                                                        |
| async_generators           | 322 ms                                                       | 356 ms: 1.11x slower                                                         |
| regex_dna                  | 227 ms                                                       | 256 ms: 1.12x slower                                                         |
| pyflate                    | 449 ms                                                       | 508 ms: 1.13x slower                                                         |
| mypy2                      | 762 ms                                                       | 861 ms: 1.13x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                        |
| coverage                   | 66.1 ms                                                      | 78.0 ms: 1.18x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.15 ms: 1.20x slower                                                        |
| scimark_sor                | 110 ms                                                       | 144 ms: 1.32x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.06x faster                                                                 |

Benchmark hidden because not significant (7): xml_etree_iterparse, asyncio_websockets, dulwich_log, docutils, pprint_safe_repr, pathlib, pycparser
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.95% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.98x