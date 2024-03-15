
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b00e021
- commit date: 2024-01-28
- overall geometric mean: 1.03x faster \*
- HPT reliability: 71.53%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 276 ms: 1.04x slower                                           |
| chameleon      | 6.70 ms                                                | 7.07 ms: 1.06x slower                                          |
| docutils       | 2.66 sec                                               | 2.66 sec: 1.00x faster                                         |
| Geometric mean | (ref)                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 442 ms: 1.19x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                           |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 575 ms: 1.09x faster                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 717 ms: 1.06x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                           |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| nbody          | 96.0 ms                                                | 104 ms: 1.08x slower                                           |
| float          | 78.9 ms                                                | 86.2 ms: 1.09x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 140 ms: 1.01x faster                                           |
| regex_effbot   | 3.51 ms                                                | 3.53 ms: 1.01x slower                                          |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                           |
| regex_v8       | 22.9 ms                                                | 24.5 ms: 1.07x slower                                          |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.30x faster                                          |
| pickle_pure_python   | 320 us                                                 | 292 us: 1.10x faster                                           |
| xml_etree_parse      | 164 ms                                                 | 155 ms: 1.06x faster                                           |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.06x faster                                           |
| tomli_loads          | 2.30 sec                                               | 2.21 sec: 1.04x faster                                         |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                          |
| pickle_dict          | 34.6 us                                                | 34.3 us: 1.01x faster                                          |
| unpickle_list        | 5.21 us                                                | 5.18 us: 1.01x faster                                          |
| pickle               | 11.0 us                                                | 11.5 us: 1.04x slower                                          |
| xml_etree_process    | 56.9 ms                                                | 59.5 ms: 1.05x slower                                          |
| unpickle             | 13.8 us                                                | 14.9 us: 1.07x slower                                          |
| xml_etree_generate   | 81.1 ms                                                | 87.4 ms: 1.08x slower                                          |
| pickle_list          | 4.59 us                                                | 5.14 us: 1.12x slower                                          |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                   |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                          |
| python_startup_no_site | 6.01 ms                                                | 8.84 ms: 1.47x slower                                          |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.7 ms: 1.19x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.66x faster                                           |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                          |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                         |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.30x faster                                          |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                          |
| comprehensions             | 23.6 us                                                | 19.4 us: 1.21x faster                                          |
| async_tree_none            | 528 ms                                                 | 442 ms: 1.19x faster                                           |
| richards_super             | 61.9 ms                                                | 53.0 ms: 1.17x faster                                          |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                           |
| pickle_pure_python         | 320 us                                                 | 292 us: 1.10x faster                                           |
| raytrace                   | 309 ms                                                 | 282 ms: 1.09x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 575 ms: 1.09x faster                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                         |
| sqlglot_transpile          | 1.75 ms                                                | 1.61 ms: 1.09x faster                                          |
| logging_silent             | 111 ns                                                 | 102 ns: 1.08x faster                                           |
| gc_traversal               | 4.01 ms                                                | 3.71 ms: 1.08x faster                                          |
| logging_simple             | 6.22 us                                                | 5.77 us: 1.08x faster                                          |
| deepcopy_memo              | 40.2 us                                                | 37.6 us: 1.07x faster                                          |
| richards                   | 49.8 ms                                                | 46.8 ms: 1.06x faster                                          |
| deepcopy                   | 365 us                                                 | 344 us: 1.06x faster                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 717 ms: 1.06x faster                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.03 us: 1.06x faster                                          |
| logging_format             | 6.81 us                                                | 6.44 us: 1.06x faster                                          |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                           |
| xml_etree_parse            | 164 ms                                                 | 155 ms: 1.06x faster                                           |
| unpickle_pure_python       | 242 us                                                 | 229 us: 1.06x faster                                           |
| sympy_str                  | 297 ms                                                 | 284 ms: 1.05x faster                                           |
| tomli_loads                | 2.30 sec                                               | 2.21 sec: 1.04x faster                                         |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                          |
| unpack_sequence            | 43.5 ns                                                | 42.1 ns: 1.03x faster                                          |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                          |
| sqlglot_normalize          | 113 ms                                                 | 110 ms: 1.02x faster                                           |
| mdp                        | 2.77 sec                                               | 2.71 sec: 1.02x faster                                         |
| sympy_expand               | 484 ms                                                 | 478 ms: 1.01x faster                                           |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                          |
| regex_compile              | 141 ms                                                 | 140 ms: 1.01x faster                                           |
| pickle_dict                | 34.6 us                                                | 34.3 us: 1.01x faster                                          |
| unpickle_list              | 5.21 us                                                | 5.18 us: 1.01x faster                                          |
| docutils                   | 2.66 sec                                               | 2.66 sec: 1.00x faster                                         |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                           |
| bench_thread_pool          | 834 us                                                 | 839 us: 1.01x slower                                           |
| go                         | 149 ms                                                 | 150 ms: 1.01x slower                                           |
| regex_effbot               | 3.51 ms                                                | 3.53 ms: 1.01x slower                                          |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                           |
| crypto_pyaes               | 76.7 ms                                                | 77.5 ms: 1.01x slower                                          |
| sqlglot_optimize           | 55.3 ms                                                | 56.1 ms: 1.01x slower                                          |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.02x slower                                           |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                         |
| deltablue                  | 3.92 ms                                                | 4.06 ms: 1.04x slower                                          |
| nqueens                    | 87.9 ms                                                | 91.4 ms: 1.04x slower                                          |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                          |
| 2to3                       | 264 ms                                                 | 276 ms: 1.04x slower                                           |
| pickle                     | 11.0 us                                                | 11.5 us: 1.04x slower                                          |
| xml_etree_process          | 56.9 ms                                                | 59.5 ms: 1.05x slower                                          |
| chameleon                  | 6.70 ms                                                | 7.07 ms: 1.06x slower                                          |
| dulwich_log                | 64.6 ms                                                | 68.4 ms: 1.06x slower                                          |
| pprint_pformat             | 1.55 sec                                               | 1.65 sec: 1.06x slower                                         |
| fannkuch                   | 405 ms                                                 | 432 ms: 1.07x slower                                           |
| pprint_safe_repr           | 747 ms                                                 | 798 ms: 1.07x slower                                           |
| scimark_monte_carlo        | 70.7 ms                                                | 75.6 ms: 1.07x slower                                          |
| regex_dna                  | 205 ms                                                 | 219 ms: 1.07x slower                                           |
| regex_v8                   | 22.9 ms                                                | 24.5 ms: 1.07x slower                                          |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.07x slower                                          |
| xml_etree_generate         | 81.1 ms                                                | 87.4 ms: 1.08x slower                                          |
| nbody                      | 96.0 ms                                                | 104 ms: 1.08x slower                                           |
| sqlite_synth               | 2.57 us                                                | 2.80 us: 1.09x slower                                          |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.49 ms: 1.09x slower                                          |
| float                      | 78.9 ms                                                | 86.2 ms: 1.09x slower                                          |
| scimark_fft                | 345 ms                                                 | 381 ms: 1.10x slower                                           |
| pickle_list                | 4.59 us                                                | 5.14 us: 1.12x slower                                          |
| hexiom                     | 6.89 ms                                                | 8.05 ms: 1.17x slower                                          |
| coverage                   | 78.8 ms                                                | 93.4 ms: 1.19x slower                                          |
| pyflate                    | 434 ms                                                 | 517 ms: 1.19x slower                                           |
| mako                       | 10.7 ms                                                | 12.7 ms: 1.19x slower                                          |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                          |
| async_generators           | 374 ms                                                 | 454 ms: 1.22x slower                                           |
| telco                      | 6.86 ms                                                | 8.65 ms: 1.26x slower                                          |
| mypy2                      | 686 ms                                                 | 867 ms: 1.26x slower                                           |
| spectral_norm              | 108 ms                                                 | 139 ms: 1.28x slower                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.84 ms: 1.47x slower                                          |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                   |

Benchmark hidden because not significant (7): scimark_lu, tornado_http, chaos, dask, bench_mp_pool, xml_etree_iterparse, json
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 71.53% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x