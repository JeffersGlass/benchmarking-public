# Results vs. 3.12.0

- fork: mdboom
- ref: too_short_7
- machine: linux-x86_64
- commit hash: 61ce027
- commit date: 2024-03-13
- overall geometric mean: 1.00x slower
- HPT reliability: 67.87%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 281 ms: 1.02x slower                                          |
| chameleon      | 7.41 ms                                                | 7.01 ms: 1.06x faster                                         |
| tornado_http   | 103 ms                                                 | 98.8 ms: 1.04x faster                                         |
| Geometric mean | (ref)                                                  | 1.02x faster                                                  |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 446 ms: 1.06x faster                                          |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 743 ms: 1.02x slower                                          |
| async_tree_memoization_tg  | 575 ms                                                 | 594 ms: 1.03x slower                                          |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                        |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                        |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                  |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.6 ms: 1.05x faster                                         |
| nbody          | 97.0 ms                                                | 93.5 ms: 1.04x faster                                         |
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                          |
| Geometric mean | (ref)                                                  | 1.03x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 143 ms: 1.04x faster                                          |
| regex_effbot   | 3.61 ms                                                | 3.83 ms: 1.06x slower                                         |
| regex_dna      | 212 ms                                                 | 232 ms: 1.09x slower                                          |
| regex_v8       | 23.1 ms                                                | 26.1 ms: 1.13x slower                                         |
| Geometric mean | (ref)                                                  | 1.06x slower                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.07 sec: 1.12x faster                                        |
| pickle_pure_python   | 324 us                                                 | 298 us: 1.09x faster                                          |
| unpickle_list        | 5.29 us                                                | 4.89 us: 1.08x faster                                         |
| unpickle             | 15.9 us                                                | 14.8 us: 1.07x faster                                         |
| pickle_dict          | 35.5 us                                                | 33.7 us: 1.05x faster                                         |
| xml_etree_process    | 61.7 ms                                                | 59.7 ms: 1.03x faster                                         |
| pickle_list          | 5.08 us                                                | 4.95 us: 1.03x faster                                         |
| xml_etree_generate   | 89.2 ms                                                | 87.4 ms: 1.02x faster                                         |
| json_loads           | 28.5 us                                                | 28.0 us: 1.02x faster                                         |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                         |
| unpickle_pure_python | 230 us                                                 | 238 us: 1.04x slower                                          |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                  |

Benchmark hidden because not significant (3): xml_etree_parse, pickle, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.6 ms: 1.32x slower                                         |
| python_startup_no_site | 6.94 ms                                                | 11.1 ms: 1.61x slower                                         |
| Geometric mean         | (ref)                                                  | 1.45x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.9 ms: 1.09x faster                                         |
| django_template | 34.6 ms                                                | 34.8 ms: 1.00x slower                                         |
| Geometric mean  | (ref)                                                  | 1.04x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 111 us: 1.42x faster                                          |
| comprehensions             | 21.8 us                                                | 17.3 us: 1.26x faster                                         |
| tomli_loads                | 2.33 sec                                               | 2.07 sec: 1.12x faster                                        |
| scimark_fft                | 382 ms                                                 | 345 ms: 1.11x faster                                          |
| logging_format             | 7.23 us                                                | 6.56 us: 1.10x faster                                         |
| mako                       | 11.9 ms                                                | 10.9 ms: 1.09x faster                                         |
| logging_simple             | 6.46 us                                                | 5.92 us: 1.09x faster                                         |
| pickle_pure_python         | 324 us                                                 | 298 us: 1.09x faster                                          |
| deltablue                  | 3.72 ms                                                | 3.43 ms: 1.08x faster                                         |
| unpickle_list              | 5.29 us                                                | 4.89 us: 1.08x faster                                         |
| crypto_pyaes               | 81.9 ms                                                | 75.8 ms: 1.08x faster                                         |
| deepcopy_reduce            | 3.35 us                                                | 3.11 us: 1.08x faster                                         |
| raytrace                   | 312 ms                                                 | 291 ms: 1.07x faster                                          |
| unpickle                   | 15.9 us                                                | 14.8 us: 1.07x faster                                         |
| fannkuch                   | 417 ms                                                 | 394 ms: 1.06x faster                                          |
| scimark_monte_carlo        | 75.1 ms                                                | 71.0 ms: 1.06x faster                                         |
| async_tree_none            | 472 ms                                                 | 446 ms: 1.06x faster                                          |
| chameleon                  | 7.41 ms                                                | 7.01 ms: 1.06x faster                                         |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.06x faster                                         |
| pickle_dict                | 35.5 us                                                | 33.7 us: 1.05x faster                                         |
| float                      | 84.7 ms                                                | 80.6 ms: 1.05x faster                                         |
| sympy_str                  | 300 ms                                                 | 287 ms: 1.04x faster                                          |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                          |
| deepcopy                   | 371 us                                                 | 356 us: 1.04x faster                                          |
| tornado_http               | 103 ms                                                 | 98.8 ms: 1.04x faster                                         |
| chaos                      | 67.0 ms                                                | 64.5 ms: 1.04x faster                                         |
| nbody                      | 97.0 ms                                                | 93.5 ms: 1.04x faster                                         |
| regex_compile              | 148 ms                                                 | 143 ms: 1.04x faster                                          |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.88 ms: 1.04x faster                                         |
| logging_silent             | 104 ns                                                 | 101 ns: 1.04x faster                                          |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                          |
| sqlglot_parse              | 1.36 ms                                                | 1.32 ms: 1.03x faster                                         |
| xml_etree_process          | 61.7 ms                                                | 59.7 ms: 1.03x faster                                         |
| coroutines                 | 23.2 ms                                                | 22.4 ms: 1.03x faster                                         |
| pathlib                    | 19.3 ms                                                | 18.8 ms: 1.03x faster                                         |
| pprint_safe_repr           | 776 ms                                                 | 755 ms: 1.03x faster                                          |
| gc_traversal               | 3.79 ms                                                | 3.69 ms: 1.03x faster                                         |
| json                       | 5.26 ms                                                | 5.12 ms: 1.03x faster                                         |
| deepcopy_memo              | 40.7 us                                                | 39.7 us: 1.03x faster                                         |
| pickle_list                | 5.08 us                                                | 4.95 us: 1.03x faster                                         |
| async_generators           | 463 ms                                                 | 453 ms: 1.02x faster                                          |
| xml_etree_generate         | 89.2 ms                                                | 87.4 ms: 1.02x faster                                         |
| sqlglot_normalize          | 110 ms                                                 | 108 ms: 1.02x faster                                          |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.02x faster                                         |
| json_loads                 | 28.5 us                                                | 28.0 us: 1.02x faster                                         |
| sympy_integrate            | 21.4 ms                                                | 21.2 ms: 1.01x faster                                         |
| pprint_pformat             | 1.57 sec                                               | 1.56 sec: 1.01x faster                                        |
| scimark_sor                | 129 ms                                                 | 128 ms: 1.01x faster                                          |
| django_template            | 34.6 ms                                                | 34.8 ms: 1.00x slower                                         |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                          |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                         |
| richards                   | 45.8 ms                                                | 46.5 ms: 1.01x slower                                         |
| sympy_expand               | 478 ms                                                 | 485 ms: 1.01x slower                                          |
| create_gc_cycles           | 1.48 ms                                                | 1.50 ms: 1.02x slower                                         |
| dulwich_log                | 68.5 ms                                                | 69.7 ms: 1.02x slower                                         |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                          |
| richards_super             | 51.5 ms                                                | 52.5 ms: 1.02x slower                                         |
| asyncio_websockets         | 551 ms                                                 | 563 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 743 ms: 1.02x slower                                          |
| 2to3                       | 274 ms                                                 | 281 ms: 1.02x slower                                          |
| bench_thread_pool          | 842 us                                                 | 863 us: 1.03x slower                                          |
| asyncio_tcp                | 491 ms                                                 | 504 ms: 1.03x slower                                          |
| sqlglot_optimize           | 54.8 ms                                                | 56.4 ms: 1.03x slower                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 594 ms: 1.03x slower                                          |
| unpickle_pure_python       | 230 us                                                 | 238 us: 1.04x slower                                          |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.85 sec: 1.04x slower                                        |
| aiohttp                    | 1.15 ms                                                | 1.20 ms: 1.05x slower                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.24 sec: 1.05x slower                                        |
| gunicorn                   | 1.24 ms                                                | 1.30 ms: 1.05x slower                                         |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                        |
| regex_effbot               | 3.61 ms                                                | 3.83 ms: 1.06x slower                                         |
| go                         | 139 ms                                                 | 149 ms: 1.07x slower                                          |
| pycparser                  | 1.18 sec                                               | 1.27 sec: 1.07x slower                                        |
| nqueens                    | 83.3 ms                                                | 90.0 ms: 1.08x slower                                         |
| scimark_lu                 | 118 ms                                                 | 129 ms: 1.09x slower                                          |
| regex_dna                  | 212 ms                                                 | 232 ms: 1.09x slower                                          |
| bench_mp_pool              | 24.0 ms                                                | 26.3 ms: 1.09x slower                                         |
| hexiom                     | 6.41 ms                                                | 7.04 ms: 1.10x slower                                         |
| regex_v8                   | 23.1 ms                                                | 26.1 ms: 1.13x slower                                         |
| telco                      | 7.10 ms                                                | 8.56 ms: 1.21x slower                                         |
| python_startup             | 9.55 ms                                                | 12.6 ms: 1.32x slower                                         |
| coverage                   | 72.7 ms                                                | 98.0 ms: 1.35x slower                                         |
| python_startup_no_site     | 6.94 ms                                                | 11.1 ms: 1.61x slower                                         |
| unpack_sequence            | 54.0 ns                                                | 87.8 ns: 1.63x slower                                         |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                  |

Benchmark hidden because not significant (12): spectral_norm, async_tree_memoization, pyflate, xml_etree_parse, mdp, pickle, async_tree_cpu_io_mixed, docutils, xml_etree_iterparse, sqlite_synth, dask, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240313-3.13.0a5+-61ce027-JIT/bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 67.87% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x