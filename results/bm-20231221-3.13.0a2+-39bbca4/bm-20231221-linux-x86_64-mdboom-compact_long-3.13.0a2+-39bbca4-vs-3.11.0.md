
# Results vs. 3.11.0

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.06x faster
- HPT reliability: 99.98%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| chameleon      | 6.70 ms                                                | 7.06 ms: 1.05x slower                                          |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                         |
| tornado_http   | 98.1 ms                                                | 95.0 ms: 1.03x faster                                          |
| Geometric mean | (ref)                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none           | 528 ms                                                 | 438 ms: 1.20x faster                                           |
| async_tree_memoization    | 639 ms                                                 | 565 ms: 1.13x faster                                           |
| async_tree_io             | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| async_tree_none_tg        | 491 ms                                                 | 455 ms: 1.08x faster                                           |
| async_tree_io_tg          | 1.29 sec                                               | 1.22 sec: 1.06x faster                                         |
| async_tree_memoization_tg | 626 ms                                                 | 597 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 727 ms: 1.03x faster                                           |
| Geometric mean            | (ref)                                                  | 1.08x faster                                                   |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 91.2 ms: 1.05x faster                                          |
| float          | 78.9 ms                                                | 81.9 ms: 1.04x slower                                          |
| pidigits       | 194 ms                                                 | 222 ms: 1.15x slower                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 134 ms: 1.05x faster                                           |
| regex_dna      | 205 ms                                                 | 217 ms: 1.06x slower                                           |
| regex_v8       | 22.9 ms                                                | 24.4 ms: 1.06x slower                                          |
| Geometric mean | (ref)                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                          |
| unpickle_pure_python | 242 us                                                 | 220 us: 1.10x faster                                           |
| tomli_loads          | 2.30 sec                                               | 2.17 sec: 1.06x faster                                         |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                           |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                          |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                           |
| unpickle_list        | 5.21 us                                                | 5.07 us: 1.03x faster                                          |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                           |
| pickle_dict          | 34.6 us                                                | 34.3 us: 1.01x faster                                          |
| pickle               | 11.0 us                                                | 11.1 us: 1.01x slower                                          |
| xml_etree_process    | 56.9 ms                                                | 59.0 ms: 1.04x slower                                          |
| xml_etree_generate   | 81.1 ms                                                | 85.9 ms: 1.06x slower                                          |
| unpickle             | 13.8 us                                                | 15.0 us: 1.08x slower                                          |
| pickle_list          | 4.59 us                                                | 5.05 us: 1.10x slower                                          |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.21x slower                                          |
| python_startup_no_site | 6.01 ms                                                | 8.99 ms: 1.50x slower                                          |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                          |

All benchmarks:
===============

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols  | 520 us                                                 | 118 us: 4.41x faster                                           |
| generators                | 74.9 ms                                                | 29.1 ms: 2.57x faster                                          |
| asyncio_tcp               | 875 ms                                                 | 485 ms: 1.81x faster                                           |
| asyncio_tcp_ssl           | 3.11 sec                                               | 1.79 sec: 1.74x faster                                         |
| comprehensions            | 23.6 us                                                | 16.3 us: 1.44x faster                                          |
| json_dumps                | 13.3 ms                                                | 10.4 ms: 1.28x faster                                          |
| async_tree_none           | 528 ms                                                 | 438 ms: 1.20x faster                                           |
| coroutines                | 27.0 ms                                                | 22.5 ms: 1.20x faster                                          |
| chaos                     | 71.9 ms                                                | 60.9 ms: 1.18x faster                                          |
| deltablue                 | 3.92 ms                                                | 3.32 ms: 1.18x faster                                          |
| richards_super            | 61.9 ms                                                | 53.7 ms: 1.15x faster                                          |
| sympy_sum                 | 169 ms                                                 | 148 ms: 1.14x faster                                           |
| async_tree_memoization    | 639 ms                                                 | 565 ms: 1.13x faster                                           |
| sqlglot_parse             | 1.43 ms                                                | 1.27 ms: 1.13x faster                                          |
| raytrace                  | 309 ms                                                 | 275 ms: 1.12x faster                                           |
| hexiom                    | 6.89 ms                                                | 6.15 ms: 1.12x faster                                          |
| sympy_str                 | 297 ms                                                 | 269 ms: 1.11x faster                                           |
| sqlglot_transpile         | 1.75 ms                                                | 1.59 ms: 1.10x faster                                          |
| sympy_integrate           | 21.5 ms                                                | 19.5 ms: 1.10x faster                                          |
| unpickle_pure_python      | 242 us                                                 | 220 us: 1.10x faster                                           |
| nqueens                   | 87.9 ms                                                | 79.9 ms: 1.10x faster                                          |
| logging_simple            | 6.22 us                                                | 5.68 us: 1.10x faster                                          |
| logging_format            | 6.81 us                                                | 6.24 us: 1.09x faster                                          |
| async_tree_io             | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| async_tree_none_tg        | 491 ms                                                 | 455 ms: 1.08x faster                                           |
| logging_silent            | 111 ns                                                 | 103 ns: 1.07x faster                                           |
| go                        | 149 ms                                                 | 139 ms: 1.07x faster                                           |
| mdp                       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                         |
| tomli_loads               | 2.30 sec                                               | 2.17 sec: 1.06x faster                                         |
| pickle_pure_python        | 320 us                                                 | 301 us: 1.06x faster                                           |
| sqlglot_normalize         | 113 ms                                                 | 106 ms: 1.06x faster                                           |
| sympy_expand              | 484 ms                                                 | 457 ms: 1.06x faster                                           |
| async_tree_io_tg          | 1.29 sec                                               | 1.22 sec: 1.06x faster                                         |
| nbody                     | 96.0 ms                                                | 91.2 ms: 1.05x faster                                          |
| regex_compile             | 141 ms                                                 | 134 ms: 1.05x faster                                           |
| async_tree_memoization_tg | 626 ms                                                 | 597 ms: 1.05x faster                                           |
| deepcopy_reduce           | 3.22 us                                                | 3.07 us: 1.05x faster                                          |
| richards                  | 49.8 ms                                                | 47.7 ms: 1.04x faster                                          |
| deepcopy                  | 365 us                                                 | 351 us: 1.04x faster                                           |
| scimark_sparse_mat_mult   | 5.03 ms                                                | 4.85 ms: 1.04x faster                                          |
| json_loads                | 29.2 us                                                | 28.2 us: 1.04x faster                                          |
| tornado_http              | 98.1 ms                                                | 95.0 ms: 1.03x faster                                          |
| pycparser                 | 1.19 sec                                               | 1.15 sec: 1.03x faster                                         |
| xml_etree_parse           | 164 ms                                                 | 159 ms: 1.03x faster                                           |
| scimark_monte_carlo       | 70.7 ms                                                | 68.5 ms: 1.03x faster                                          |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 727 ms: 1.03x faster                                           |
| unpickle_list             | 5.21 us                                                | 5.07 us: 1.03x faster                                          |
| docutils                  | 2.66 sec                                               | 2.59 sec: 1.03x faster                                         |
| sqlglot_optimize          | 55.3 ms                                                | 53.8 ms: 1.03x faster                                          |
| pprint_pformat            | 1.55 sec                                               | 1.51 sec: 1.03x faster                                         |
| deepcopy_memo             | 40.2 us                                                | 39.2 us: 1.02x faster                                          |
| crypto_pyaes              | 76.7 ms                                                | 75.0 ms: 1.02x faster                                          |
| fannkuch                  | 405 ms                                                 | 397 ms: 1.02x faster                                           |
| xml_etree_iterparse       | 108 ms                                                 | 106 ms: 1.02x faster                                           |
| json                      | 5.24 ms                                                | 5.16 ms: 1.02x faster                                          |
| pickle_dict               | 34.6 us                                                | 34.3 us: 1.01x faster                                          |
| bench_thread_pool         | 834 us                                                 | 827 us: 1.01x faster                                           |
| pathlib                   | 18.5 ms                                                | 18.4 ms: 1.01x faster                                          |
| meteor_contest            | 109 ms                                                 | 109 ms: 1.00x slower                                           |
| asyncio_websockets        | 550 ms                                                 | 552 ms: 1.00x slower                                           |
| pickle                    | 11.0 us                                                | 11.1 us: 1.01x slower                                          |
| scimark_sor               | 121 ms                                                 | 124 ms: 1.02x slower                                           |
| dulwich_log               | 64.6 ms                                                | 65.8 ms: 1.02x slower                                          |
| spectral_norm             | 108 ms                                                 | 111 ms: 1.02x slower                                           |
| create_gc_cycles          | 1.43 ms                                                | 1.48 ms: 1.03x slower                                          |
| float                     | 78.9 ms                                                | 81.9 ms: 1.04x slower                                          |
| xml_etree_process         | 56.9 ms                                                | 59.0 ms: 1.04x slower                                          |
| chameleon                 | 6.70 ms                                                | 7.06 ms: 1.05x slower                                          |
| regex_dna                 | 205 ms                                                 | 217 ms: 1.06x slower                                           |
| xml_etree_generate        | 81.1 ms                                                | 85.9 ms: 1.06x slower                                          |
| regex_v8                  | 22.9 ms                                                | 24.4 ms: 1.06x slower                                          |
| scimark_fft               | 345 ms                                                 | 369 ms: 1.07x slower                                           |
| mako                      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                          |
| gc_traversal              | 4.01 ms                                                | 4.30 ms: 1.07x slower                                          |
| unpickle                  | 13.8 us                                                | 15.0 us: 1.08x slower                                          |
| pyflate                   | 434 ms                                                 | 472 ms: 1.09x slower                                           |
| sqlite_synth              | 2.57 us                                                | 2.82 us: 1.10x slower                                          |
| pickle_list               | 4.59 us                                                | 5.05 us: 1.10x slower                                          |
| pidigits                  | 194 ms                                                 | 222 ms: 1.15x slower                                           |
| coverage                  | 78.8 ms                                                | 93.0 ms: 1.18x slower                                          |
| async_generators          | 374 ms                                                 | 442 ms: 1.18x slower                                           |
| python_startup            | 8.56 ms                                                | 10.4 ms: 1.21x slower                                          |
| mypy2                     | 686 ms                                                 | 838 ms: 1.22x slower                                           |
| telco                     | 6.86 ms                                                | 8.55 ms: 1.25x slower                                          |
| unpack_sequence           | 43.5 ns                                                | 54.7 ns: 1.26x slower                                          |
| python_startup_no_site    | 6.01 ms                                                | 8.99 ms: 1.50x slower                                          |
| Geometric mean            | (ref)                                                  | 1.06x faster                                                   |

Benchmark hidden because not significant (6): async_tree_cpu_io_mixed_tg, pprint_safe_repr, regex_effbot, bench_mp_pool, 2to3, scimark_lu
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.97x