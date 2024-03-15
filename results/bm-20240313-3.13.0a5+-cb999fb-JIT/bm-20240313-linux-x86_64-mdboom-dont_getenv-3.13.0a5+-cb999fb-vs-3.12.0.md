# Results vs. 3.12.0

- fork: mdboom
- ref: dont_getenv
- machine: linux-x86_64
- commit hash: cb999fb
- commit date: 2024-03-13
- overall geometric mean: 1.01x slower
- HPT reliability: 81.76%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 283 ms: 1.03x slower                                          |
| chameleon      | 7.41 ms                                                | 6.83 ms: 1.08x faster                                         |
| docutils       | 2.77 sec                                               | 2.78 sec: 1.00x slower                                        |
| tornado_http   | 103 ms                                                 | 98.6 ms: 1.04x faster                                         |
| Geometric mean | (ref)                                                  | 1.02x faster                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 447 ms: 1.06x faster                                          |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 741 ms: 1.02x slower                                          |
| async_tree_memoization_tg  | 575 ms                                                 | 599 ms: 1.04x slower                                          |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                        |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.05x slower                                        |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                  |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.0 ms: 1.06x faster                                         |
| nbody          | 97.0 ms                                                | 92.8 ms: 1.04x faster                                         |
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                          |
| Geometric mean | (ref)                                                  | 1.03x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 143 ms: 1.04x faster                                          |
| regex_dna      | 212 ms                                                 | 225 ms: 1.06x slower                                          |
| regex_effbot   | 3.61 ms                                                | 3.90 ms: 1.08x slower                                         |
| regex_v8       | 23.1 ms                                                | 25.4 ms: 1.10x slower                                         |
| Geometric mean | (ref)                                                  | 1.05x slower                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.08 sec: 1.12x faster                                        |
| unpickle_list        | 5.29 us                                                | 4.80 us: 1.10x faster                                         |
| unpickle             | 15.9 us                                                | 14.5 us: 1.09x faster                                         |
| pickle_dict          | 35.5 us                                                | 34.1 us: 1.04x faster                                         |
| pickle_pure_python   | 324 us                                                 | 312 us: 1.04x faster                                          |
| xml_etree_process    | 61.7 ms                                                | 59.7 ms: 1.03x faster                                         |
| xml_etree_generate   | 89.2 ms                                                | 86.7 ms: 1.03x faster                                         |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.02x faster                                         |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                         |
| pickle               | 11.6 us                                                | 11.5 us: 1.00x faster                                         |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.01x slower                                          |
| unpickle_pure_python | 230 us                                                 | 239 us: 1.04x slower                                          |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                  |

Benchmark hidden because not significant (2): xml_etree_parse, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.6 ms: 1.32x slower                                         |
| python_startup_no_site | 6.94 ms                                                | 11.1 ms: 1.60x slower                                         |
| Geometric mean         | (ref)                                                  | 1.45x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako           | 11.9 ms                                                | 10.8 ms: 1.10x faster                                         |
| Geometric mean | (ref)                                                  | 1.05x faster                                                  |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.43x faster                                          |
| comprehensions             | 21.8 us                                                | 17.3 us: 1.26x faster                                         |
| scimark_fft                | 382 ms                                                 | 339 ms: 1.13x faster                                          |
| tomli_loads                | 2.33 sec                                               | 2.08 sec: 1.12x faster                                        |
| logging_format             | 7.23 us                                                | 6.53 us: 1.11x faster                                         |
| mako                       | 11.9 ms                                                | 10.8 ms: 1.10x faster                                         |
| unpickle_list              | 5.29 us                                                | 4.80 us: 1.10x faster                                         |
| logging_simple             | 6.46 us                                                | 5.90 us: 1.10x faster                                         |
| unpickle                   | 15.9 us                                                | 14.5 us: 1.09x faster                                         |
| deepcopy_reduce            | 3.35 us                                                | 3.08 us: 1.09x faster                                         |
| chameleon                  | 7.41 ms                                                | 6.83 ms: 1.08x faster                                         |
| deltablue                  | 3.72 ms                                                | 3.43 ms: 1.08x faster                                         |
| crypto_pyaes               | 81.9 ms                                                | 76.1 ms: 1.08x faster                                         |
| scimark_monte_carlo        | 75.1 ms                                                | 70.5 ms: 1.07x faster                                         |
| float                      | 84.7 ms                                                | 80.0 ms: 1.06x faster                                         |
| generators                 | 31.2 ms                                                | 29.5 ms: 1.06x faster                                         |
| async_tree_none            | 472 ms                                                 | 447 ms: 1.06x faster                                          |
| raytrace                   | 312 ms                                                 | 297 ms: 1.05x faster                                          |
| fannkuch                   | 417 ms                                                 | 398 ms: 1.05x faster                                          |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                          |
| deepcopy                   | 371 us                                                 | 355 us: 1.04x faster                                          |
| nbody                      | 97.0 ms                                                | 92.8 ms: 1.04x faster                                         |
| sympy_str                  | 300 ms                                                 | 287 ms: 1.04x faster                                          |
| pickle_dict                | 35.5 us                                                | 34.1 us: 1.04x faster                                         |
| tornado_http               | 103 ms                                                 | 98.6 ms: 1.04x faster                                         |
| sqlglot_parse              | 1.36 ms                                                | 1.31 ms: 1.04x faster                                         |
| pickle_pure_python         | 324 us                                                 | 312 us: 1.04x faster                                          |
| regex_compile              | 148 ms                                                 | 143 ms: 1.04x faster                                          |
| chaos                      | 67.0 ms                                                | 64.5 ms: 1.04x faster                                         |
| coroutines                 | 23.2 ms                                                | 22.4 ms: 1.04x faster                                         |
| xml_etree_process          | 61.7 ms                                                | 59.7 ms: 1.03x faster                                         |
| pathlib                    | 19.3 ms                                                | 18.7 ms: 1.03x faster                                         |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                          |
| xml_etree_generate         | 89.2 ms                                                | 86.7 ms: 1.03x faster                                         |
| logging_silent             | 104 ns                                                 | 102 ns: 1.03x faster                                          |
| pprint_safe_repr           | 776 ms                                                 | 756 ms: 1.03x faster                                          |
| deepcopy_memo              | 40.7 us                                                | 39.7 us: 1.03x faster                                         |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.94 ms: 1.02x faster                                         |
| sqlglot_transpile          | 1.68 ms                                                | 1.65 ms: 1.02x faster                                         |
| pickle_list                | 5.08 us                                                | 5.00 us: 1.02x faster                                         |
| json                       | 5.26 ms                                                | 5.17 ms: 1.02x faster                                         |
| pprint_pformat             | 1.57 sec                                               | 1.55 sec: 1.01x faster                                        |
| spectral_norm              | 115 ms                                                 | 113 ms: 1.01x faster                                          |
| sqlglot_normalize          | 110 ms                                                 | 109 ms: 1.01x faster                                          |
| scimark_sor                | 129 ms                                                 | 128 ms: 1.01x faster                                          |
| sympy_integrate            | 21.4 ms                                                | 21.3 ms: 1.01x faster                                         |
| json_loads                 | 28.5 us                                                | 28.3 us: 1.01x faster                                         |
| pickle                     | 11.6 us                                                | 11.5 us: 1.00x faster                                         |
| docutils                   | 2.77 sec                                               | 2.78 sec: 1.00x slower                                        |
| sqlite_synth               | 2.83 us                                                | 2.85 us: 1.01x slower                                         |
| xml_etree_iterparse        | 107 ms                                                 | 108 ms: 1.01x slower                                          |
| pidigits                   | 187 ms                                                 | 190 ms: 1.01x slower                                          |
| async_generators           | 463 ms                                                 | 469 ms: 1.01x slower                                          |
| sympy_expand               | 478 ms                                                 | 487 ms: 1.02x slower                                          |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 741 ms: 1.02x slower                                          |
| asyncio_websockets         | 551 ms                                                 | 563 ms: 1.02x slower                                          |
| dulwich_log                | 68.5 ms                                                | 70.0 ms: 1.02x slower                                         |
| bench_thread_pool          | 842 us                                                 | 863 us: 1.02x slower                                          |
| richards                   | 45.8 ms                                                | 47.0 ms: 1.03x slower                                         |
| create_gc_cycles           | 1.48 ms                                                | 1.52 ms: 1.03x slower                                         |
| asyncio_tcp                | 491 ms                                                 | 505 ms: 1.03x slower                                          |
| 2to3                       | 274 ms                                                 | 283 ms: 1.03x slower                                          |
| pycparser                  | 1.18 sec                                               | 1.22 sec: 1.03x slower                                        |
| sqlglot_optimize           | 54.8 ms                                                | 56.8 ms: 1.04x slower                                         |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.04x slower                                        |
| unpickle_pure_python       | 230 us                                                 | 239 us: 1.04x slower                                          |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.04x slower                                         |
| gunicorn                   | 1.24 ms                                                | 1.29 ms: 1.04x slower                                         |
| richards_super             | 51.5 ms                                                | 53.7 ms: 1.04x slower                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 599 ms: 1.04x slower                                          |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                        |
| async_tree_io              | 1.16 sec                                               | 1.22 sec: 1.05x slower                                        |
| regex_dna                  | 212 ms                                                 | 225 ms: 1.06x slower                                          |
| nqueens                    | 83.3 ms                                                | 89.6 ms: 1.08x slower                                         |
| gc_traversal               | 3.79 ms                                                | 4.09 ms: 1.08x slower                                         |
| regex_effbot               | 3.61 ms                                                | 3.90 ms: 1.08x slower                                         |
| hexiom                     | 6.41 ms                                                | 7.03 ms: 1.10x slower                                         |
| scimark_lu                 | 118 ms                                                 | 130 ms: 1.10x slower                                          |
| regex_v8                   | 23.1 ms                                                | 25.4 ms: 1.10x slower                                         |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                         |
| go                         | 139 ms                                                 | 156 ms: 1.12x slower                                          |
| telco                      | 7.10 ms                                                | 8.42 ms: 1.19x slower                                         |
| python_startup             | 9.55 ms                                                | 12.6 ms: 1.32x slower                                         |
| coverage                   | 72.7 ms                                                | 97.8 ms: 1.35x slower                                         |
| python_startup_no_site     | 6.94 ms                                                | 11.1 ms: 1.60x slower                                         |
| unpack_sequence            | 54.0 ns                                                | 88.3 ns: 1.64x slower                                         |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (9): pyflate, async_tree_memoization, xml_etree_parse, async_tree_cpu_io_mixed, mdp, django_template, json_dumps, dask, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240313-3.13.0a5+-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 81.76% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x