
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.02x slower
- HPT reliability: 95.85%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 308 ms: 1.07x slower                                                         |
| chameleon      | 7.92 ms                                                      | 8.14 ms: 1.03x slower                                                        |
| docutils       | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                       |
| tornado_http   | 124 ms                                                       | 126 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 443 ms: 1.17x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 445 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 708 ms: 1.06x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 567 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 714 ms: 1.05x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 266 ms: 1.06x slower                                                         |
| nbody          | 92.9 ms                                                      | 129 ms: 1.39x slower                                                         |
| float          | 74.9 ms                                                      | 104 ms: 1.39x slower                                                         |
| Geometric mean | (ref)                                                        | 1.27x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 25.7 ms: 1.05x slower                                                        |
| regex_dna      | 227 ms                                                       | 243 ms: 1.07x slower                                                         |
| regex_compile  | 156 ms                                                       | 169 ms: 1.08x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.9 us: 1.16x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.05x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 31.1 us: 1.04x faster                                                        |
| pickle_pure_python   | 316 us                                                       | 312 us: 1.01x faster                                                         |
| unpickle_pure_python | 238 us                                                       | 242 us: 1.02x slower                                                         |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| unpickle_list        | 4.60 us                                                      | 4.80 us: 1.04x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| xml_etree_process    | 55.9 ms                                                      | 62.2 ms: 1.11x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.40 us: 1.12x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.9 us: 1.12x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 89.9 ms: 1.13x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.81 sec: 1.25x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.03x slower                                                                 |

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
| mako      | 11.0 ms                                                      | 15.0 ms: 1.36x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 128 us: 4.17x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 374 ms: 2.00x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.60 sec: 1.91x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.1 ms: 1.60x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                        |
| async_tree_none            | 518 ms                                                       | 443 ms: 1.17x faster                                                         |
| json_loads                 | 28.9 us                                                      | 24.9 us: 1.16x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.73 ms: 1.11x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 168 ms: 1.10x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 104 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 445 ms: 1.07x faster                                                         |
| json                       | 5.58 ms                                                      | 5.25 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 708 ms: 1.06x faster                                                         |
| mdp                        | 2.77 sec                                                     | 2.62 sec: 1.06x faster                                                       |
| richards_super             | 63.6 ms                                                      | 60.1 ms: 1.06x faster                                                        |
| logging_simple             | 7.24 us                                                      | 6.85 us: 1.06x faster                                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 567 ms: 1.06x faster                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.43 ms: 1.06x faster                                                        |
| unpack_sequence            | 45.7 ns                                                      | 43.3 ns: 1.06x faster                                                        |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 714 ms: 1.05x faster                                                         |
| sympy_str                  | 337 ms                                                       | 322 ms: 1.05x faster                                                         |
| sympy_integrate            | 25.8 ms                                                      | 24.8 ms: 1.04x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 31.1 us: 1.04x faster                                                        |
| sympy_expand               | 553 ms                                                       | 532 ms: 1.04x faster                                                         |
| raytrace                   | 309 ms                                                       | 298 ms: 1.04x faster                                                         |
| logging_silent             | 100 ns                                                       | 97.0 ns: 1.03x faster                                                        |
| deepcopy                   | 391 us                                                       | 380 us: 1.03x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.86 ms: 1.03x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.54 us: 1.02x faster                                                        |
| pickle_pure_python         | 316 us                                                       | 312 us: 1.01x faster                                                         |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 123 ms: 1.01x slower                                                         |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.01x slower                                                       |
| tornado_http               | 124 ms                                                       | 126 ms: 1.02x slower                                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.60 ms: 1.02x slower                                                        |
| unpickle_pure_python       | 238 us                                                       | 242 us: 1.02x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                        |
| chameleon                  | 7.92 ms                                                      | 8.14 ms: 1.03x slower                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 86.0 ms: 1.03x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| docutils                   | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                       |
| chaos                      | 74.9 ms                                                      | 78.0 ms: 1.04x slower                                                        |
| unpickle_list              | 4.60 us                                                      | 4.80 us: 1.04x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 25.7 ms: 1.05x slower                                                        |
| meteor_contest             | 131 ms                                                       | 137 ms: 1.05x slower                                                         |
| pidigits                   | 251 ms                                                       | 266 ms: 1.06x slower                                                         |
| nqueens                    | 103 ms                                                       | 109 ms: 1.06x slower                                                         |
| regex_dna                  | 227 ms                                                       | 243 ms: 1.07x slower                                                         |
| sqlglot_optimize           | 59.0 ms                                                      | 63.3 ms: 1.07x slower                                                        |
| 2to3                       | 287 ms                                                       | 308 ms: 1.07x slower                                                         |
| dulwich_log                | 67.4 ms                                                      | 72.5 ms: 1.08x slower                                                        |
| regex_compile              | 156 ms                                                       | 169 ms: 1.08x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| richards                   | 49.7 ms                                                      | 54.1 ms: 1.09x slower                                                        |
| deepcopy_memo              | 37.5 us                                                      | 41.2 us: 1.10x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.79 us: 1.10x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 62.2 ms: 1.11x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.40 us: 1.12x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.9 us: 1.12x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 89.9 ms: 1.13x slower                                                        |
| go                         | 158 ms                                                       | 180 ms: 1.14x slower                                                         |
| fannkuch                   | 416 ms                                                       | 474 ms: 1.14x slower                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.93 sec: 1.16x slower                                                       |
| async_generators           | 322 ms                                                       | 372 ms: 1.16x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 931 ms: 1.16x slower                                                         |
| mypy2                      | 762 ms                                                       | 889 ms: 1.17x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| coverage                   | 66.1 ms                                                      | 78.8 ms: 1.19x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.24 ms: 1.21x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.81 sec: 1.25x slower                                                       |
| scimark_monte_carlo        | 69.8 ms                                                      | 87.5 ms: 1.25x slower                                                        |
| pyflate                    | 449 ms                                                       | 586 ms: 1.30x slower                                                         |
| scimark_sor                | 110 ms                                                       | 147 ms: 1.34x slower                                                         |
| mako                       | 11.0 ms                                                      | 15.0 ms: 1.36x slower                                                        |
| deltablue                  | 3.97 ms                                                      | 5.43 ms: 1.37x slower                                                        |
| nbody                      | 92.9 ms                                                      | 129 ms: 1.39x slower                                                         |
| float                      | 74.9 ms                                                      | 104 ms: 1.39x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 9.82 ms: 1.41x slower                                                        |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| scimark_fft                | 281 ms                                                       | 434 ms: 1.55x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.71 ms: 1.65x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 162 ms: 1.71x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (5): bench_thread_pool, dask, comprehensions, deepcopy_reduce, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 95.85% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x