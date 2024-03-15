
# Results vs. 3.11.0

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 4d59a84
- commit date: 2024-02-09
- overall geometric mean: 1.01x faster \*
- HPT reliability: 95.68%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.34 ms: 1.10x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 591 ms: 1.06x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 737 ms: 1.03x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 91.8 ms: 1.16x slower                                                            |
| nbody          | 96.0 ms                                                | 114 ms: 1.18x slower                                                             |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                            |
| regex_compile  | 141 ms                                                 | 151 ms: 1.07x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                            |
| regex_dna      | 205 ms                                                 | 227 ms: 1.11x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.25x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 303 us: 1.05x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 233 us: 1.04x faster                                                             |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| unpickle_list        | 5.21 us                                                | 5.17 us: 1.01x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| tomli_loads          | 2.30 sec                                               | 2.37 sec: 1.03x slower                                                           |
| pickle_dict          | 34.6 us                                                | 35.8 us: 1.04x slower                                                            |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                            |
| unpickle             | 13.8 us                                                | 14.7 us: 1.06x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.5 ms: 1.06x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 88.8 ms: 1.10x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.26 us: 1.15x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.74 ms: 1.45x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.6 ms: 1.28x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.44x faster                                                             |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.54x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 494 ms: 1.77x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.25x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.4 ms: 1.20x faster                                                            |
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                             |
| comprehensions             | 23.6 us                                                | 20.6 us: 1.15x faster                                                            |
| richards_super             | 61.9 ms                                                | 55.7 ms: 1.11x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.70 ms: 1.08x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 591 ms: 1.06x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                           |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| pickle_pure_python         | 320 us                                                 | 303 us: 1.05x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                            |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.67 sec: 1.04x faster                                                           |
| unpickle_pure_python       | 242 us                                                 | 233 us: 1.04x faster                                                             |
| raytrace                   | 309 ms                                                 | 297 ms: 1.04x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                            |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                             |
| logging_silent             | 111 ns                                                 | 107 ns: 1.03x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.02 us: 1.03x faster                                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 737 ms: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| deepcopy                   | 365 us                                                 | 357 us: 1.02x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                            |
| sympy_str                  | 297 ms                                                 | 292 ms: 1.02x faster                                                             |
| unpack_sequence            | 43.5 ns                                                | 42.7 ns: 1.02x faster                                                            |
| richards                   | 49.8 ms                                                | 48.9 ms: 1.02x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                            |
| unpickle_list              | 5.21 us                                                | 5.17 us: 1.01x faster                                                            |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                             |
| chaos                      | 71.9 ms                                                | 72.2 ms: 1.00x slower                                                            |
| deepcopy_memo              | 40.2 us                                                | 40.3 us: 1.00x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                           |
| sympy_expand               | 484 ms                                                 | 490 ms: 1.01x slower                                                             |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.01x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 850 us: 1.02x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.02x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.37 sec: 1.03x slower                                                           |
| scimark_sor                | 121 ms                                                 | 126 ms: 1.04x slower                                                             |
| pickle_dict                | 34.6 us                                                | 35.8 us: 1.04x slower                                                            |
| meteor_contest             | 109 ms                                                 | 113 ms: 1.04x slower                                                             |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 57.7 ms: 1.04x slower                                                            |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                             |
| unpickle                   | 13.8 us                                                | 14.7 us: 1.06x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.5 ms: 1.06x slower                                                            |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 68.9 ms: 1.07x slower                                                            |
| regex_compile              | 141 ms                                                 | 151 ms: 1.07x slower                                                             |
| fannkuch                   | 405 ms                                                 | 437 ms: 1.08x slower                                                             |
| nqueens                    | 87.9 ms                                                | 95.0 ms: 1.08x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 811 ms: 1.08x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.69 sec: 1.09x slower                                                           |
| crypto_pyaes               | 76.7 ms                                                | 83.2 ms: 1.09x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.34 ms: 1.10x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 88.8 ms: 1.10x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                            |
| regex_dna                  | 205 ms                                                 | 227 ms: 1.11x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.90 us: 1.13x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 79.9 ms: 1.13x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.26 us: 1.15x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.53 ms: 1.16x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.84 ms: 1.16x slower                                                            |
| float                      | 78.9 ms                                                | 91.8 ms: 1.16x slower                                                            |
| pyflate                    | 434 ms                                                 | 508 ms: 1.17x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| nbody                      | 96.0 ms                                                | 114 ms: 1.18x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.24 ms: 1.20x slower                                                            |
| async_generators           | 374 ms                                                 | 450 ms: 1.20x slower                                                             |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                                            |
| telco                      | 6.86 ms                                                | 8.57 ms: 1.25x slower                                                            |
| mypy2                      | 686 ms                                                 | 867 ms: 1.26x slower                                                             |
| scimark_fft                | 345 ms                                                 | 441 ms: 1.28x slower                                                             |
| mako                       | 10.7 ms                                                | 13.6 ms: 1.28x slower                                                            |
| spectral_norm              | 108 ms                                                 | 143 ms: 1.32x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.74 ms: 1.45x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (6): logging_format, bench_mp_pool, pathlib, json, tornado_http, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 95.68% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x