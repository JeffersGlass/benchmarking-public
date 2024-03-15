# Results vs. 3.11.0

- fork: mdboom
- ref: dont_getenv
- machine: linux-x86_64
- commit hash: cb999fb
- commit date: 2024-03-13
- overall geometric mean: 1.02x faster
- HPT reliability: 66.60%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 283 ms: 1.07x slower                                          |
| chameleon      | 6.70 ms                                                | 6.83 ms: 1.02x slower                                         |
| docutils       | 2.66 sec                                               | 2.78 sec: 1.04x slower                                        |
| html5lib       | 64.8 ms                                                | 68.8 ms: 1.06x slower                                         |
| Geometric mean | (ref)                                                  | 1.04x slower                                                  |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                          |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                          |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.06x faster                                        |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.05x faster                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 599 ms: 1.05x faster                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                          |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 741 ms: 1.03x faster                                          |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.8 ms: 1.03x faster                                         |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                          |
| float          | 78.9 ms                                                | 80.0 ms: 1.01x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 143 ms: 1.01x slower                                          |
| regex_dna      | 205 ms                                                 | 225 ms: 1.10x slower                                          |
| regex_effbot   | 3.51 ms                                                | 3.90 ms: 1.11x slower                                         |
| regex_v8       | 22.9 ms                                                | 25.4 ms: 1.11x slower                                         |
| Geometric mean | (ref)                                                  | 1.08x slower                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                         |
| tomli_loads          | 2.30 sec                                               | 2.08 sec: 1.11x faster                                        |
| unpickle_list        | 5.21 us                                                | 4.80 us: 1.09x faster                                         |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                          |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                         |
| pickle_pure_python   | 320 us                                                 | 312 us: 1.03x faster                                          |
| pickle_dict          | 34.6 us                                                | 34.1 us: 1.02x faster                                         |
| unpickle_pure_python | 242 us                                                 | 239 us: 1.01x faster                                          |
| xml_etree_process    | 56.9 ms                                                | 59.7 ms: 1.05x slower                                         |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                         |
| unpickle             | 13.8 us                                                | 14.5 us: 1.05x slower                                         |
| xml_etree_generate   | 81.1 ms                                                | 86.7 ms: 1.07x slower                                         |
| pickle_list          | 4.59 us                                                | 5.00 us: 1.09x slower                                         |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                  |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.6 ms: 1.47x slower                                         |
| python_startup_no_site | 6.01 ms                                                | 11.1 ms: 1.85x slower                                         |
| Geometric mean         | (ref)                                                  | 1.65x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.8 ms: 1.01x slower                                         |
| django_template | 33.5 ms                                                | 34.7 ms: 1.03x slower                                         |
| genshi_xml      | 53.4 ms                                                | 55.3 ms: 1.03x slower                                         |
| genshi_text     | 22.5 ms                                                | 24.3 ms: 1.08x slower                                         |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.72x faster                                          |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.54x faster                                         |
| asyncio_tcp                | 875 ms                                                 | 505 ms: 1.73x faster                                          |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                        |
| pylint                     | 476 ms                                                 | 324 ms: 1.47x faster                                          |
| comprehensions             | 23.6 us                                                | 17.3 us: 1.36x faster                                         |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                         |
| coroutines                 | 27.0 ms                                                | 22.4 ms: 1.21x faster                                         |
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                          |
| richards_super             | 61.9 ms                                                | 53.7 ms: 1.15x faster                                         |
| deltablue                  | 3.92 ms                                                | 3.43 ms: 1.14x faster                                         |
| chaos                      | 71.9 ms                                                | 64.5 ms: 1.11x faster                                         |
| tomli_loads                | 2.30 sec                                               | 2.08 sec: 1.11x faster                                        |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                          |
| sqlglot_parse              | 1.43 ms                                                | 1.31 ms: 1.10x faster                                         |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                          |
| unpickle_list              | 5.21 us                                                | 4.80 us: 1.09x faster                                         |
| djangocms                  | 33.5 us                                                | 31.0 us: 1.08x faster                                         |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                          |
| richards                   | 49.8 ms                                                | 47.0 ms: 1.06x faster                                         |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                         |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.06x faster                                        |
| logging_simple             | 6.22 us                                                | 5.90 us: 1.05x faster                                         |
| mdp                        | 2.77 sec                                               | 2.63 sec: 1.05x faster                                        |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.05x faster                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 599 ms: 1.05x faster                                          |
| deepcopy_reduce            | 3.22 us                                                | 3.08 us: 1.04x faster                                         |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                          |
| logging_format             | 6.81 us                                                | 6.53 us: 1.04x faster                                         |
| raytrace                   | 309 ms                                                 | 297 ms: 1.04x faster                                          |
| sympy_str                  | 297 ms                                                 | 287 ms: 1.04x faster                                          |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.03x faster                                          |
| nbody                      | 96.0 ms                                                | 92.8 ms: 1.03x faster                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                          |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                          |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                         |
| deepcopy                   | 365 us                                                 | 355 us: 1.03x faster                                          |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 741 ms: 1.03x faster                                          |
| pickle_pure_python         | 320 us                                                 | 312 us: 1.03x faster                                          |
| pidigits                   | 194 ms                                                 | 190 ms: 1.02x faster                                          |
| scimark_fft                | 345 ms                                                 | 339 ms: 1.02x faster                                          |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.94 ms: 1.02x faster                                         |
| fannkuch                   | 405 ms                                                 | 398 ms: 1.02x faster                                          |
| pickle_dict                | 34.6 us                                                | 34.1 us: 1.02x faster                                         |
| json                       | 5.24 ms                                                | 5.17 ms: 1.01x faster                                         |
| unpickle_pure_python       | 242 us                                                 | 239 us: 1.01x faster                                          |
| deepcopy_memo              | 40.2 us                                                | 39.7 us: 1.01x faster                                         |
| crypto_pyaes               | 76.7 ms                                                | 76.1 ms: 1.01x faster                                         |
| sympy_integrate            | 21.5 ms                                                | 21.3 ms: 1.01x faster                                         |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.00x slower                                          |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                         |
| pprint_safe_repr           | 747 ms                                                 | 756 ms: 1.01x slower                                          |
| regex_compile              | 141 ms                                                 | 143 ms: 1.01x slower                                          |
| mako                       | 10.7 ms                                                | 10.8 ms: 1.01x slower                                         |
| float                      | 78.9 ms                                                | 80.0 ms: 1.01x slower                                         |
| thrift                     | 784 us                                                 | 795 us: 1.01x slower                                          |
| gc_traversal               | 4.01 ms                                                | 4.09 ms: 1.02x slower                                         |
| chameleon                  | 6.70 ms                                                | 6.83 ms: 1.02x slower                                         |
| nqueens                    | 87.9 ms                                                | 89.6 ms: 1.02x slower                                         |
| hexiom                     | 6.89 ms                                                | 7.03 ms: 1.02x slower                                         |
| dask                       | 365 ms                                                 | 374 ms: 1.02x slower                                          |
| asyncio_websockets         | 550 ms                                                 | 563 ms: 1.02x slower                                          |
| sqlglot_optimize           | 55.3 ms                                                | 56.8 ms: 1.03x slower                                         |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                        |
| django_template            | 33.5 ms                                                | 34.7 ms: 1.03x slower                                         |
| bench_thread_pool          | 834 us                                                 | 863 us: 1.03x slower                                          |
| genshi_xml                 | 53.4 ms                                                | 55.3 ms: 1.03x slower                                         |
| docutils                   | 2.66 sec                                               | 2.78 sec: 1.04x slower                                        |
| spectral_norm              | 108 ms                                                 | 113 ms: 1.05x slower                                          |
| xml_etree_process          | 56.9 ms                                                | 59.7 ms: 1.05x slower                                         |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                         |
| unpickle                   | 13.8 us                                                | 14.5 us: 1.05x slower                                         |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                          |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.06x slower                                          |
| create_gc_cycles           | 1.43 ms                                                | 1.52 ms: 1.06x slower                                         |
| html5lib                   | 64.8 ms                                                | 68.8 ms: 1.06x slower                                         |
| 2to3                       | 264 ms                                                 | 283 ms: 1.07x slower                                          |
| xml_etree_generate         | 81.1 ms                                                | 86.7 ms: 1.07x slower                                         |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.07x slower                                         |
| genshi_text                | 22.5 ms                                                | 24.3 ms: 1.08x slower                                         |
| gunicorn                   | 1.20 ms                                                | 1.29 ms: 1.08x slower                                         |
| dulwich_log                | 64.6 ms                                                | 70.0 ms: 1.08x slower                                         |
| pickle_list                | 4.59 us                                                | 5.00 us: 1.09x slower                                         |
| regex_dna                  | 205 ms                                                 | 225 ms: 1.10x slower                                          |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                         |
| pyflate                    | 434 ms                                                 | 480 ms: 1.11x slower                                          |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                         |
| regex_effbot               | 3.51 ms                                                | 3.90 ms: 1.11x slower                                         |
| regex_v8                   | 22.9 ms                                                | 25.4 ms: 1.11x slower                                         |
| scimark_lu                 | 116 ms                                                 | 130 ms: 1.11x slower                                          |
| telco                      | 6.86 ms                                                | 8.42 ms: 1.23x slower                                         |
| coverage                   | 78.8 ms                                                | 97.8 ms: 1.24x slower                                         |
| async_generators           | 374 ms                                                 | 469 ms: 1.26x slower                                          |
| mypy2                      | 686 ms                                                 | 904 ms: 1.32x slower                                          |
| python_startup             | 8.56 ms                                                | 12.6 ms: 1.47x slower                                         |
| python_startup_no_site     | 6.01 ms                                                | 11.1 ms: 1.85x slower                                         |
| unpack_sequence            | 43.5 ns                                                | 88.3 ns: 2.03x slower                                         |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                  |

Benchmark hidden because not significant (5): pprint_pformat, scimark_monte_carlo, xml_etree_iterparse, meteor_contest, tornado_http
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 66.60% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x