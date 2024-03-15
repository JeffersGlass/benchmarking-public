
# Results vs. 3.11.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 482aac3
- commit date: 2024-02-08
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.09%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 287 ms: 1.09x slower                                                           |
| chameleon      | 6.70 ms                                                | 7.39 ms: 1.10x slower                                                          |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                         |
| tornado_http   | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 455 ms: 1.16x faster                                                           |
| async_tree_memoization     | 639 ms                                                 | 585 ms: 1.09x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.07x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 608 ms: 1.03x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                           |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                           |
| float          | 78.9 ms                                                | 101 ms: 1.28x slower                                                           |
| nbody          | 96.0 ms                                                | 129 ms: 1.34x slower                                                           |
| Geometric mean | (ref)                                                  | 1.19x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                          |
| regex_dna      | 205 ms                                                 | 226 ms: 1.10x slower                                                           |
| regex_compile  | 141 ms                                                 | 156 ms: 1.10x slower                                                           |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                          |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                          |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                           |
| json_loads           | 29.2 us                                                | 27.7 us: 1.05x faster                                                          |
| unpickle_list        | 5.21 us                                                | 4.98 us: 1.05x faster                                                          |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                           |
| pickle_dict          | 34.6 us                                                | 33.8 us: 1.02x faster                                                          |
| unpickle_pure_python | 242 us                                                 | 237 us: 1.02x faster                                                           |
| xml_etree_iterparse  | 108 ms                                                 | 113 ms: 1.05x slower                                                           |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                                          |
| xml_etree_process    | 56.9 ms                                                | 61.6 ms: 1.08x slower                                                          |
| xml_etree_generate   | 81.1 ms                                                | 90.3 ms: 1.11x slower                                                          |
| unpickle             | 13.8 us                                                | 15.4 us: 1.11x slower                                                          |
| pickle_list          | 4.59 us                                                | 5.20 us: 1.13x slower                                                          |
| tomli_loads          | 2.30 sec                                               | 2.80 sec: 1.21x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                          |
| python_startup_no_site | 6.01 ms                                                | 8.76 ms: 1.46x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 15.2 ms: 1.42x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.47x faster                                                           |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.54x faster                                                          |
| asyncio_tcp                | 875 ms                                                 | 489 ms: 1.79x faster                                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                         |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                          |
| coroutines                 | 27.0 ms                                                | 22.6 ms: 1.20x faster                                                          |
| async_tree_none            | 528 ms                                                 | 455 ms: 1.16x faster                                                           |
| async_tree_memoization     | 639 ms                                                 | 585 ms: 1.09x faster                                                           |
| richards_super             | 61.9 ms                                                | 57.1 ms: 1.08x faster                                                          |
| gc_traversal               | 4.01 ms                                                | 3.70 ms: 1.08x faster                                                          |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.07x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                         |
| deltablue                  | 3.92 ms                                                | 3.69 ms: 1.06x faster                                                          |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                           |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                         |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.05x faster                                                          |
| sqlglot_parse              | 1.43 ms                                                | 1.36 ms: 1.05x faster                                                          |
| unpickle_list              | 5.21 us                                                | 4.98 us: 1.05x faster                                                          |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                           |
| mdp                        | 2.77 sec                                               | 2.67 sec: 1.04x faster                                                         |
| deepcopy                   | 365 us                                                 | 354 us: 1.03x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 608 ms: 1.03x faster                                                           |
| logging_simple             | 6.22 us                                                | 6.04 us: 1.03x faster                                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                           |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.70 ms: 1.03x faster                                                          |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                          |
| pickle_dict                | 34.6 us                                                | 33.8 us: 1.02x faster                                                          |
| sympy_sum                  | 169 ms                                                 | 166 ms: 1.02x faster                                                           |
| unpickle_pure_python       | 242 us                                                 | 237 us: 1.02x faster                                                           |
| json                       | 5.24 ms                                                | 5.16 ms: 1.02x faster                                                          |
| comprehensions             | 23.6 us                                                | 23.5 us: 1.00x faster                                                          |
| raytrace                   | 309 ms                                                 | 310 ms: 1.00x slower                                                           |
| sympy_integrate            | 21.5 ms                                                | 21.7 ms: 1.01x slower                                                          |
| logging_format             | 6.81 us                                                | 6.87 us: 1.01x slower                                                          |
| tornado_http               | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                          |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                                           |
| deepcopy_memo              | 40.2 us                                                | 40.7 us: 1.01x slower                                                          |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                         |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                          |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                           |
| sympy_expand               | 484 ms                                                 | 495 ms: 1.02x slower                                                           |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                                           |
| richards                   | 49.8 ms                                                | 51.0 ms: 1.02x slower                                                          |
| bench_thread_pool          | 834 us                                                 | 858 us: 1.03x slower                                                           |
| unpack_sequence            | 43.5 ns                                                | 45.0 ns: 1.04x slower                                                          |
| regex_effbot               | 3.51 ms                                                | 3.63 ms: 1.04x slower                                                          |
| pycparser                  | 1.19 sec                                               | 1.23 sec: 1.04x slower                                                         |
| sqlglot_normalize          | 113 ms                                                 | 118 ms: 1.05x slower                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 113 ms: 1.05x slower                                                           |
| meteor_contest             | 109 ms                                                 | 117 ms: 1.07x slower                                                           |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                                          |
| dulwich_log                | 64.6 ms                                                | 69.5 ms: 1.08x slower                                                          |
| sqlglot_optimize           | 55.3 ms                                                | 59.6 ms: 1.08x slower                                                          |
| xml_etree_process          | 56.9 ms                                                | 61.6 ms: 1.08x slower                                                          |
| chaos                      | 71.9 ms                                                | 77.8 ms: 1.08x slower                                                          |
| 2to3                       | 264 ms                                                 | 287 ms: 1.09x slower                                                           |
| chameleon                  | 6.70 ms                                                | 7.39 ms: 1.10x slower                                                          |
| regex_dna                  | 205 ms                                                 | 226 ms: 1.10x slower                                                           |
| regex_compile              | 141 ms                                                 | 156 ms: 1.10x slower                                                           |
| regex_v8                   | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                          |
| xml_etree_generate         | 81.1 ms                                                | 90.3 ms: 1.11x slower                                                          |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.11x slower                                                          |
| pprint_pformat             | 1.55 sec                                               | 1.74 sec: 1.12x slower                                                         |
| sqlite_synth               | 2.57 us                                                | 2.89 us: 1.12x slower                                                          |
| pprint_safe_repr           | 747 ms                                                 | 842 ms: 1.13x slower                                                           |
| pickle_list                | 4.59 us                                                | 5.20 us: 1.13x slower                                                          |
| fannkuch                   | 405 ms                                                 | 476 ms: 1.18x slower                                                           |
| nqueens                    | 87.9 ms                                                | 104 ms: 1.18x slower                                                           |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                          |
| go                         | 149 ms                                                 | 177 ms: 1.19x slower                                                           |
| crypto_pyaes               | 76.7 ms                                                | 92.1 ms: 1.20x slower                                                          |
| coverage                   | 78.8 ms                                                | 94.9 ms: 1.20x slower                                                          |
| tomli_loads                | 2.30 sec                                               | 2.80 sec: 1.21x slower                                                         |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                                           |
| scimark_monte_carlo        | 70.7 ms                                                | 88.3 ms: 1.25x slower                                                          |
| pyflate                    | 434 ms                                                 | 553 ms: 1.27x slower                                                           |
| mypy2                      | 686 ms                                                 | 875 ms: 1.28x slower                                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.42 ms: 1.28x slower                                                          |
| float                      | 78.9 ms                                                | 101 ms: 1.28x slower                                                           |
| telco                      | 6.86 ms                                                | 8.82 ms: 1.29x slower                                                          |
| nbody                      | 96.0 ms                                                | 129 ms: 1.34x slower                                                           |
| hexiom                     | 6.89 ms                                                | 9.42 ms: 1.37x slower                                                          |
| scimark_fft                | 345 ms                                                 | 475 ms: 1.37x slower                                                           |
| mako                       | 10.7 ms                                                | 15.2 ms: 1.42x slower                                                          |
| spectral_norm              | 108 ms                                                 | 157 ms: 1.45x slower                                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.76 ms: 1.46x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                   |

Benchmark hidden because not significant (4): pathlib, bench_mp_pool, asyncio_websockets, sympy_str
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.09% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x