
# Results vs. 3.11.0

- fork: mdboom
- ref: pystats_test2
- machine: linux-x86_64
- commit hash: 28e6201
- commit date: 2024-02-07
- overall geometric mean: 1.01x faster \*
- HPT reliability: 76.14%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 280 ms: 1.06x slower                                            |
| chameleon      | 6.70 ms                                                | 7.24 ms: 1.08x slower                                           |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                          |
| tornado_http   | 98.1 ms                                                | 98.7 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                            |
| async_tree_memoization     | 639 ms                                                 | 571 ms: 1.12x faster                                            |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.07x faster                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 730 ms: 1.04x faster                                            |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 720 ms: 1.04x faster                                            |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                            |
| float          | 78.9 ms                                                | 89.7 ms: 1.14x slower                                           |
| nbody          | 96.0 ms                                                | 115 ms: 1.20x slower                                            |
| Geometric mean | (ref)                                                  | 1.10x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.57 ms: 1.02x slower                                           |
| regex_compile  | 141 ms                                                 | 147 ms: 1.04x slower                                            |
| regex_dna      | 205 ms                                                 | 220 ms: 1.07x slower                                            |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.10x slower                                           |
| Geometric mean | (ref)                                                  | 1.06x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                           |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                            |
| unpickle_list        | 5.21 us                                                | 4.97 us: 1.05x faster                                           |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                            |
| unpickle_pure_python | 242 us                                                 | 233 us: 1.04x faster                                            |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                           |
| pickle_dict          | 34.6 us                                                | 34.0 us: 1.02x faster                                           |
| xml_etree_process    | 56.9 ms                                                | 60.2 ms: 1.06x slower                                           |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                           |
| xml_etree_generate   | 81.1 ms                                                | 88.0 ms: 1.09x slower                                           |
| tomli_loads          | 2.30 sec                                               | 2.54 sec: 1.10x slower                                          |
| pickle_list          | 4.59 us                                                | 5.06 us: 1.10x slower                                           |
| unpickle             | 13.8 us                                                | 17.1 us: 1.23x slower                                           |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                    |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                           |
| python_startup_no_site | 6.01 ms                                                | 8.77 ms: 1.46x slower                                           |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.1 ms: 1.23x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.49x faster                                            |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                           |
| asyncio_tcp                | 875 ms                                                 | 489 ms: 1.79x faster                                            |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                          |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                           |
| coroutines                 | 27.0 ms                                                | 21.6 ms: 1.25x faster                                           |
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                            |
| comprehensions             | 23.6 us                                                | 20.4 us: 1.16x faster                                           |
| richards_super             | 61.9 ms                                                | 54.3 ms: 1.14x faster                                           |
| deltablue                  | 3.92 ms                                                | 3.50 ms: 1.12x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 571 ms: 1.12x faster                                            |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.08x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.07x faster                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                          |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                            |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.06x faster                                           |
| unpack_sequence            | 43.5 ns                                                | 41.3 ns: 1.05x faster                                           |
| gc_traversal               | 4.01 ms                                                | 3.81 ms: 1.05x faster                                           |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                            |
| mdp                        | 2.77 sec                                               | 2.64 sec: 1.05x faster                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                            |
| unpickle_list              | 5.21 us                                                | 4.97 us: 1.05x faster                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 730 ms: 1.04x faster                                            |
| logging_simple             | 6.22 us                                                | 5.96 us: 1.04x faster                                           |
| raytrace                   | 309 ms                                                 | 296 ms: 1.04x faster                                            |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 720 ms: 1.04x faster                                            |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                            |
| unpickle_pure_python       | 242 us                                                 | 233 us: 1.04x faster                                            |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                            |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                           |
| richards                   | 49.8 ms                                                | 48.4 ms: 1.03x faster                                           |
| sympy_str                  | 297 ms                                                 | 290 ms: 1.03x faster                                            |
| sympy_integrate            | 21.5 ms                                                | 21.0 ms: 1.02x faster                                           |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                            |
| pickle_dict                | 34.6 us                                                | 34.0 us: 1.02x faster                                           |
| chaos                      | 71.9 ms                                                | 71.3 ms: 1.01x faster                                           |
| sqlglot_normalize          | 113 ms                                                 | 112 ms: 1.01x faster                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.20 us: 1.01x faster                                           |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                           |
| deepcopy_memo              | 40.2 us                                                | 40.0 us: 1.00x faster                                           |
| tornado_http               | 98.1 ms                                                | 98.7 ms: 1.01x slower                                           |
| bench_thread_pool          | 834 us                                                 | 842 us: 1.01x slower                                            |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                          |
| regex_effbot               | 3.51 ms                                                | 3.57 ms: 1.02x slower                                           |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                           |
| meteor_contest             | 109 ms                                                 | 113 ms: 1.03x slower                                            |
| sqlglot_optimize           | 55.3 ms                                                | 57.1 ms: 1.03x slower                                           |
| regex_compile              | 141 ms                                                 | 147 ms: 1.04x slower                                            |
| nqueens                    | 87.9 ms                                                | 91.6 ms: 1.04x slower                                           |
| pprint_pformat             | 1.55 sec                                               | 1.62 sec: 1.04x slower                                          |
| crypto_pyaes               | 76.7 ms                                                | 80.3 ms: 1.05x slower                                           |
| pprint_safe_repr           | 747 ms                                                 | 783 ms: 1.05x slower                                            |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.05x slower                                          |
| xml_etree_process          | 56.9 ms                                                | 60.2 ms: 1.06x slower                                           |
| 2to3                       | 264 ms                                                 | 280 ms: 1.06x slower                                            |
| dulwich_log                | 64.6 ms                                                | 68.8 ms: 1.06x slower                                           |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                           |
| fannkuch                   | 405 ms                                                 | 433 ms: 1.07x slower                                            |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.07x slower                                            |
| chameleon                  | 6.70 ms                                                | 7.24 ms: 1.08x slower                                           |
| xml_etree_generate         | 81.1 ms                                                | 88.0 ms: 1.09x slower                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.49 ms: 1.09x slower                                           |
| scimark_monte_carlo        | 70.7 ms                                                | 77.5 ms: 1.10x slower                                           |
| tomli_loads                | 2.30 sec                                               | 2.54 sec: 1.10x slower                                          |
| pickle_list                | 4.59 us                                                | 5.06 us: 1.10x slower                                           |
| regex_v8                   | 22.9 ms                                                | 25.3 ms: 1.10x slower                                           |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                           |
| float                      | 78.9 ms                                                | 89.7 ms: 1.14x slower                                           |
| go                         | 149 ms                                                 | 172 ms: 1.16x slower                                            |
| hexiom                     | 6.89 ms                                                | 8.04 ms: 1.17x slower                                           |
| pyflate                    | 434 ms                                                 | 509 ms: 1.17x slower                                            |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                           |
| nbody                      | 96.0 ms                                                | 115 ms: 1.20x slower                                            |
| coverage                   | 78.8 ms                                                | 95.1 ms: 1.21x slower                                           |
| async_generators           | 374 ms                                                 | 453 ms: 1.21x slower                                            |
| mako                       | 10.7 ms                                                | 13.1 ms: 1.23x slower                                           |
| unpickle                   | 13.8 us                                                | 17.1 us: 1.23x slower                                           |
| scimark_fft                | 345 ms                                                 | 432 ms: 1.25x slower                                            |
| telco                      | 6.86 ms                                                | 8.67 ms: 1.26x slower                                           |
| spectral_norm              | 108 ms                                                 | 137 ms: 1.26x slower                                            |
| mypy2                      | 686 ms                                                 | 868 ms: 1.27x slower                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.77 ms: 1.46x slower                                           |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                    |

Benchmark hidden because not significant (8): json, scimark_lu, bench_mp_pool, logging_format, xml_etree_iterparse, sympy_expand, asyncio_websockets, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 76.14% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x