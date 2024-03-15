
# Results vs. 3.11.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 4448793
- commit date: 2024-01-16
- overall geometric mean: 1.06x slower
- HPT reliability: 99.82%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 318 ms: 1.11x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.85 ms: 1.01x faster                                                        |
| docutils       | 2.85 sec                                                     | 3.08 sec: 1.08x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 562 ms: 1.12x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 712 ms: 1.06x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 571 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 715 ms: 1.05x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 265 ms: 1.05x slower                                                         |
| float          | 74.9 ms                                                      | 106 ms: 1.41x slower                                                         |
| nbody          | 92.9 ms                                                      | 131 ms: 1.41x slower                                                         |
| Geometric mean | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.48 ms: 1.04x slower                                                        |
| regex_dna      | 227 ms                                                       | 250 ms: 1.10x slower                                                         |
| regex_v8       | 24.4 ms                                                      | 26.9 ms: 1.10x slower                                                        |
| regex_compile  | 156 ms                                                       | 194 ms: 1.24x slower                                                         |
| Geometric mean | (ref)                                                        | 1.12x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 11.0 ms: 1.21x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.6 us: 1.18x faster                                                        |
| pickle_dict          | 32.3 us                                                      | 30.8 us: 1.05x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.05x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 310 us: 1.02x faster                                                         |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 114 ms: 1.07x slower                                                         |
| unpickle_list        | 4.60 us                                                      | 4.97 us: 1.08x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.7 us: 1.11x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 62.6 ms: 1.12x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.50 us: 1.14x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 92.5 ms: 1.16x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.89 sec: 1.28x slower                                                       |
| unpickle_pure_python | 238 us                                                       | 317 us: 1.33x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 14.9 ms: 1.36x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 127 us: 4.19x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 373 ms: 2.00x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 33.6 ms: 1.63x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.1 ms: 1.26x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 11.0 ms: 1.21x faster                                                        |
| json_loads                 | 28.9 us                                                      | 24.6 us: 1.18x faster                                                        |
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 562 ms: 1.12x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.81 ms: 1.09x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                       |
| sympy_sum                  | 186 ms                                                       | 175 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| json                       | 5.58 ms                                                      | 5.28 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 712 ms: 1.06x faster                                                         |
| pickle_dict                | 32.3 us                                                      | 30.8 us: 1.05x faster                                                        |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.05x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 571 ms: 1.05x faster                                                         |
| mdp                        | 2.77 sec                                                     | 2.64 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 715 ms: 1.05x faster                                                         |
| logging_simple             | 7.24 us                                                      | 7.03 us: 1.03x faster                                                        |
| deepcopy                   | 391 us                                                       | 381 us: 1.02x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 310 us: 1.02x faster                                                         |
| logging_format             | 7.71 us                                                      | 7.57 us: 1.02x faster                                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.34 us: 1.02x faster                                                        |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| logging_silent             | 100 ns                                                       | 99.4 ns: 1.01x faster                                                        |
| chameleon                  | 7.92 ms                                                      | 7.85 ms: 1.01x faster                                                        |
| sympy_str                  | 337 ms                                                       | 336 ms: 1.00x faster                                                         |
| sympy_expand               | 553 ms                                                       | 556 ms: 1.01x slower                                                         |
| sympy_integrate            | 25.8 ms                                                      | 26.0 ms: 1.01x slower                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.54 ms: 1.02x slower                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.96 ms: 1.02x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 85.7 ms: 1.03x slower                                                        |
| raytrace                   | 309 ms                                                       | 319 ms: 1.03x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.5 ms: 1.03x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.48 ms: 1.04x slower                                                        |
| chaos                      | 74.9 ms                                                      | 78.5 ms: 1.05x slower                                                        |
| comprehensions             | 25.1 us                                                      | 26.2 us: 1.05x slower                                                        |
| sqlglot_normalize          | 122 ms                                                       | 128 ms: 1.05x slower                                                         |
| pidigits                   | 251 ms                                                       | 265 ms: 1.05x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                       | 114 ms: 1.07x slower                                                         |
| meteor_contest             | 131 ms                                                       | 141 ms: 1.08x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.97 us: 1.08x slower                                                        |
| docutils                   | 2.85 sec                                                     | 3.08 sec: 1.08x slower                                                       |
| pycparser                  | 1.31 sec                                                     | 1.44 sec: 1.10x slower                                                       |
| deepcopy_memo              | 37.5 us                                                      | 41.2 us: 1.10x slower                                                        |
| regex_dna                  | 227 ms                                                       | 250 ms: 1.10x slower                                                         |
| regex_v8                   | 24.4 ms                                                      | 26.9 ms: 1.10x slower                                                        |
| 2to3                       | 287 ms                                                       | 318 ms: 1.11x slower                                                         |
| unpickle                   | 13.3 us                                                      | 14.7 us: 1.11x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.81 us: 1.11x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 62.6 ms: 1.12x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 75.7 ms: 1.12x slower                                                        |
| nqueens                    | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| sqlglot_optimize           | 59.0 ms                                                      | 67.3 ms: 1.14x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.50 us: 1.14x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 92.5 ms: 1.16x slower                                                        |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| async_generators           | 322 ms                                                       | 379 ms: 1.18x slower                                                         |
| coverage                   | 66.1 ms                                                      | 79.1 ms: 1.20x slower                                                        |
| mypy2                      | 762 ms                                                       | 929 ms: 1.22x slower                                                         |
| scimark_lu                 | 114 ms                                                       | 140 ms: 1.22x slower                                                         |
| pprint_pformat             | 1.67 sec                                                     | 2.05 sec: 1.23x slower                                                       |
| pprint_safe_repr           | 805 ms                                                       | 998 ms: 1.24x slower                                                         |
| fannkuch                   | 416 ms                                                       | 516 ms: 1.24x slower                                                         |
| regex_compile              | 156 ms                                                       | 194 ms: 1.24x slower                                                         |
| telco                      | 6.81 ms                                                      | 8.51 ms: 1.25x slower                                                        |
| richards_super             | 63.6 ms                                                      | 80.0 ms: 1.26x slower                                                        |
| go                         | 158 ms                                                       | 202 ms: 1.28x slower                                                         |
| tomli_loads                | 2.25 sec                                                     | 2.89 sec: 1.28x slower                                                       |
| unpickle_pure_python       | 238 us                                                       | 317 us: 1.33x slower                                                         |
| mako                       | 11.0 ms                                                      | 14.9 ms: 1.36x slower                                                        |
| float                      | 74.9 ms                                                      | 106 ms: 1.41x slower                                                         |
| nbody                      | 92.9 ms                                                      | 131 ms: 1.41x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| richards                   | 49.7 ms                                                      | 71.6 ms: 1.44x slower                                                        |
| deltablue                  | 3.97 ms                                                      | 5.76 ms: 1.45x slower                                                        |
| unpack_sequence            | 45.7 ns                                                      | 66.4 ns: 1.45x slower                                                        |
| scimark_sor                | 110 ms                                                       | 160 ms: 1.46x slower                                                         |
| pyflate                    | 449 ms                                                       | 660 ms: 1.47x slower                                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 105 ms: 1.51x slower                                                         |
| scimark_fft                | 281 ms                                                       | 426 ms: 1.52x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.23 ms: 1.53x slower                                                        |
| hexiom                     | 6.98 ms                                                      | 10.9 ms: 1.56x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 161 ms: 1.69x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.06x slower                                                                 |

Benchmark hidden because not significant (5): bench_thread_pool, tornado_http, dask, bench_mp_pool, create_gc_cycles
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.82% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.99x