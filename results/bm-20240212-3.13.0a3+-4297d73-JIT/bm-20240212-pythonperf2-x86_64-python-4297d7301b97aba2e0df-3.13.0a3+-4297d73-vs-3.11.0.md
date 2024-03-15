
# Results vs. 3.11.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: linux-x86_64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.03x faster \*
- HPT reliability: 85.62%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 298 ms: 1.04x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.54 ms: 1.05x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                                       |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 431 ms: 1.20x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 547 ms: 1.15x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 545 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 435 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 699 ms: 1.08x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.07x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 701 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 263 ms: 1.05x slower                                                         |
| float          | 74.9 ms                                                      | 81.7 ms: 1.09x slower                                                        |
| nbody          | 92.9 ms                                                      | 107 ms: 1.15x slower                                                         |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                         |
| regex_dna      | 227 ms                                                       | 240 ms: 1.06x slower                                                         |
| regex_v8       | 24.4 ms                                                      | 26.3 ms: 1.08x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.69 ms: 1.11x slower                                                        |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.27x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.2 us: 1.15x faster                                                        |
| pickle_pure_python   | 316 us                                                       | 301 us: 1.05x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                                         |
| unpickle_pure_python | 238 us                                                       | 228 us: 1.04x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 32.7 us: 1.01x slower                                                        |
| unpickle_list        | 4.60 us                                                      | 4.66 us: 1.01x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                                        |
| pickle               | 9.89 us                                                      | 10.5 us: 1.06x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 84.5 ms: 1.06x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.12x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.44 us: 1.13x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 11.8 ms: 1.08x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 119 us: 4.45x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 369 ms: 2.03x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 33.6 ms: 1.63x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.27x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                        |
| comprehensions             | 25.1 us                                                      | 20.7 us: 1.21x faster                                                        |
| async_tree_none            | 518 ms                                                       | 431 ms: 1.20x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 97.6 ms: 1.17x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 159 ms: 1.16x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 547 ms: 1.15x faster                                                         |
| json_loads                 | 28.9 us                                                      | 25.2 us: 1.15x faster                                                        |
| gc_traversal               | 4.15 ms                                                      | 3.64 ms: 1.14x faster                                                        |
| raytrace                   | 309 ms                                                       | 275 ms: 1.13x faster                                                         |
| sympy_str                  | 337 ms                                                       | 299 ms: 1.13x faster                                                         |
| richards_super             | 63.6 ms                                                      | 56.9 ms: 1.12x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.37 ms: 1.10x faster                                                        |
| sympy_expand               | 553 ms                                                       | 501 ms: 1.10x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 545 ms: 1.10x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.60 us: 1.10x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 435 ms: 1.09x faster                                                         |
| mdp                        | 2.77 sec                                                     | 2.56 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 699 ms: 1.08x faster                                                         |
| deltablue                  | 3.97 ms                                                      | 3.68 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.07x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 701 ms: 1.07x faster                                                         |
| regex_compile              | 156 ms                                                       | 146 ms: 1.07x faster                                                         |
| chaos                      | 74.9 ms                                                      | 70.3 ms: 1.07x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 24.3 ms: 1.06x faster                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.80 ms: 1.06x faster                                                        |
| deepcopy                   | 391 us                                                       | 369 us: 1.06x faster                                                         |
| logging_silent             | 100 ns                                                       | 95.1 ns: 1.05x faster                                                        |
| nqueens                    | 103 ms                                                       | 97.4 ms: 1.05x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.33 us: 1.05x faster                                                        |
| chameleon                  | 7.92 ms                                                      | 7.54 ms: 1.05x faster                                                        |
| pickle_pure_python         | 316 us                                                       | 301 us: 1.05x faster                                                         |
| json                       | 5.58 ms                                                      | 5.33 ms: 1.05x faster                                                        |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.04x faster                                                         |
| unpickle_pure_python       | 238 us                                                       | 228 us: 1.04x faster                                                         |
| bench_thread_pool          | 1.00 ms                                                      | 966 us: 1.03x faster                                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.53 ms: 1.03x faster                                                        |
| sqlglot_normalize          | 122 ms                                                       | 119 ms: 1.02x faster                                                         |
| fannkuch                   | 416 ms                                                       | 406 ms: 1.02x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 81.5 ms: 1.02x faster                                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.34 us: 1.02x faster                                                        |
| dask                       | 410 ms                                                       | 403 ms: 1.02x faster                                                         |
| deepcopy_memo              | 37.5 us                                                      | 37.0 us: 1.01x faster                                                        |
| meteor_contest             | 131 ms                                                       | 130 ms: 1.01x faster                                                         |
| docutils                   | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                                       |
| pickle_dict                | 32.3 us                                                      | 32.7 us: 1.01x slower                                                        |
| unpickle_list              | 4.60 us                                                      | 4.66 us: 1.01x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                                       |
| richards                   | 49.7 ms                                                      | 51.0 ms: 1.03x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 69.3 ms: 1.03x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.72 sec: 1.03x slower                                                       |
| sqlglot_optimize           | 59.0 ms                                                      | 61.1 ms: 1.04x slower                                                        |
| 2to3                       | 287 ms                                                       | 298 ms: 1.04x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                                        |
| pidigits                   | 251 ms                                                       | 263 ms: 1.05x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 847 ms: 1.05x slower                                                         |
| regex_dna                  | 227 ms                                                       | 240 ms: 1.06x slower                                                         |
| pickle                     | 9.89 us                                                      | 10.5 us: 1.06x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 84.5 ms: 1.06x slower                                                        |
| go                         | 158 ms                                                       | 169 ms: 1.07x slower                                                         |
| mako                       | 11.0 ms                                                      | 11.8 ms: 1.08x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 26.3 ms: 1.08x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.74 us: 1.09x slower                                                        |
| float                      | 74.9 ms                                                      | 81.7 ms: 1.09x slower                                                        |
| hexiom                     | 6.98 ms                                                      | 7.70 ms: 1.10x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.69 ms: 1.11x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.12x slower                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 78.5 ms: 1.12x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.44 us: 1.13x slower                                                        |
| nbody                      | 92.9 ms                                                      | 107 ms: 1.15x slower                                                         |
| async_generators           | 322 ms                                                       | 370 ms: 1.15x slower                                                         |
| pyflate                    | 449 ms                                                       | 521 ms: 1.16x slower                                                         |
| mypy2                      | 762 ms                                                       | 887 ms: 1.17x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.15 ms: 1.20x slower                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.01 ms: 1.23x slower                                                        |
| coverage                   | 66.1 ms                                                      | 81.8 ms: 1.24x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 118 ms: 1.24x slower                                                         |
| scimark_fft                | 281 ms                                                       | 360 ms: 1.28x slower                                                         |
| scimark_sor                | 110 ms                                                       | 142 ms: 1.29x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.03x faster                                                                 |

Benchmark hidden because not significant (7): unpack_sequence, asyncio_websockets, tornado_http, xml_etree_iterparse, pathlib, pycparser, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 85.62% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x