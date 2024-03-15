
# Results vs. 3.12.0

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.01x slower
- HPT reliability: 93.85%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.86x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 294 ms: 1.03x slower                                                 |
| chameleon      | 7.23 ms                                                      | 7.36 ms: 1.02x slower                                                |
| docutils       | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                               |
| tornado_http   | 121 ms                                                       | 118 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                        | 1.00x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 437 ms: 1.03x faster                                                 |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 713 ms: 1.02x slower                                                 |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                 |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                               |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.05x slower                                               |
| async_tree_memoization_tg  | 540 ms                                                       | 568 ms: 1.05x slower                                                 |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 734 ms: 1.05x slower                                                 |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                         |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 84.3 ms: 1.04x faster                                                |
| pidigits       | 265 ms                                                       | 267 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                        | 1.01x faster                                                         |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                |
| regex_dna      | 239 ms                                                       | 240 ms: 1.01x slower                                                 |
| regex_compile  | 144 ms                                                       | 146 ms: 1.01x slower                                                 |
| regex_v8       | 23.6 ms                                                      | 24.7 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                        | 1.01x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 9.98 us: 1.06x faster                                                |
| pickle_pure_python   | 318 us                                                       | 308 us: 1.03x faster                                                 |
| pickle_dict          | 32.5 us                                                      | 31.6 us: 1.03x faster                                                |
| unpickle_list        | 4.66 us                                                      | 4.54 us: 1.03x faster                                                |
| pickle_list          | 4.43 us                                                      | 4.34 us: 1.02x faster                                                |
| xml_etree_generate   | 86.1 ms                                                      | 85.0 ms: 1.01x faster                                                |
| unpickle             | 14.8 us                                                      | 14.6 us: 1.01x faster                                                |
| unpickle_pure_python | 210 us                                                       | 211 us: 1.01x slower                                                 |
| xml_etree_process    | 58.4 ms                                                      | 58.7 ms: 1.01x slower                                                |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                                 |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                 |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.03x slower                                                |
| json_dumps           | 10.2 ms                                                      | 10.7 ms: 1.04x slower                                                |
| tomli_loads          | 2.16 sec                                                     | 2.35 sec: 1.09x slower                                               |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.8 ms: 1.10x slower                                                |
| python_startup_no_site | 8.64 ms                                                      | 11.3 ms: 1.30x slower                                                |
| Geometric mean         | (ref)                                                        | 1.20x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| comprehensions             | 21.9 us                                                      | 16.6 us: 1.32x faster                                                |
| typing_runtime_protocols   | 152 us                                                       | 122 us: 1.24x faster                                                 |
| raytrace                   | 298 ms                                                       | 270 ms: 1.10x faster                                                 |
| async_generators           | 390 ms                                                       | 362 ms: 1.08x faster                                                 |
| sympy_sum                  | 162 ms                                                       | 150 ms: 1.08x faster                                                 |
| generators                 | 37.4 ms                                                      | 34.8 ms: 1.08x faster                                                |
| crypto_pyaes               | 80.3 ms                                                      | 74.9 ms: 1.07x faster                                                |
| bench_mp_pool              | 4.76 ms                                                      | 4.48 ms: 1.06x faster                                                |
| chaos                      | 64.0 ms                                                      | 60.2 ms: 1.06x faster                                                |
| scimark_monte_carlo        | 69.0 ms                                                      | 65.0 ms: 1.06x faster                                                |
| pickle                     | 10.5 us                                                      | 9.98 us: 1.06x faster                                                |
| coroutines                 | 23.0 ms                                                      | 22.0 ms: 1.04x faster                                                |
| nbody                      | 88.0 ms                                                      | 84.3 ms: 1.04x faster                                                |
| sympy_integrate            | 23.9 ms                                                      | 23.0 ms: 1.04x faster                                                |
| regex_effbot               | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                |
| sympy_str                  | 302 ms                                                       | 291 ms: 1.04x faster                                                 |
| sqlite_synth               | 2.77 us                                                      | 2.68 us: 1.03x faster                                                |
| async_tree_none            | 452 ms                                                       | 437 ms: 1.03x faster                                                 |
| pickle_pure_python         | 318 us                                                       | 308 us: 1.03x faster                                                 |
| logging_format             | 7.48 us                                                      | 7.27 us: 1.03x faster                                                |
| unpack_sequence            | 53.2 ns                                                      | 51.7 ns: 1.03x faster                                                |
| pickle_dict                | 32.5 us                                                      | 31.6 us: 1.03x faster                                                |
| unpickle_list              | 4.66 us                                                      | 4.54 us: 1.03x faster                                                |
| logging_simple             | 6.71 us                                                      | 6.54 us: 1.03x faster                                                |
| tornado_http               | 121 ms                                                       | 118 ms: 1.02x faster                                                 |
| asyncio_tcp                | 378 ms                                                       | 369 ms: 1.02x faster                                                 |
| nqueens                    | 89.9 ms                                                      | 87.9 ms: 1.02x faster                                                |
| pickle_list                | 4.43 us                                                      | 4.34 us: 1.02x faster                                                |
| mdp                        | 2.57 sec                                                     | 2.53 sec: 1.01x faster                                               |
| docutils                   | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                               |
| xml_etree_generate         | 86.1 ms                                                      | 85.0 ms: 1.01x faster                                                |
| unpickle                   | 14.8 us                                                      | 14.6 us: 1.01x faster                                                |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.16 ms: 1.01x faster                                                |
| deepcopy_reduce            | 3.37 us                                                      | 3.33 us: 1.01x faster                                                |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                               |
| pprint_pformat             | 1.65 sec                                                     | 1.64 sec: 1.01x faster                                               |
| scimark_fft                | 301 ms                                                       | 299 ms: 1.01x faster                                                 |
| pprint_safe_repr           | 807 ms                                                       | 804 ms: 1.00x faster                                                 |
| sqlglot_optimize           | 57.5 ms                                                      | 57.7 ms: 1.00x slower                                                |
| unpickle_pure_python       | 210 us                                                       | 211 us: 1.01x slower                                                 |
| xml_etree_process          | 58.4 ms                                                      | 58.7 ms: 1.01x slower                                                |
| sqlglot_parse              | 1.38 ms                                                      | 1.39 ms: 1.01x slower                                                |
| regex_dna                  | 239 ms                                                       | 240 ms: 1.01x slower                                                 |
| scimark_lu                 | 98.8 ms                                                      | 99.5 ms: 1.01x slower                                                |
| sqlglot_transpile          | 1.78 ms                                                      | 1.79 ms: 1.01x slower                                                |
| pidigits                   | 265 ms                                                       | 267 ms: 1.01x slower                                                 |
| regex_compile              | 144 ms                                                       | 146 ms: 1.01x slower                                                 |
| logging_silent             | 94.4 ns                                                      | 95.6 ns: 1.01x slower                                                |
| deepcopy_memo              | 36.8 us                                                      | 37.3 us: 1.01x slower                                                |
| meteor_contest             | 128 ms                                                       | 130 ms: 1.02x slower                                                 |
| xml_etree_iterparse        | 103 ms                                                       | 105 ms: 1.02x slower                                                 |
| chameleon                  | 7.23 ms                                                      | 7.36 ms: 1.02x slower                                                |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                 |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 713 ms: 1.02x slower                                                 |
| sympy_expand               | 484 ms                                                       | 496 ms: 1.03x slower                                                 |
| gc_traversal               | 3.48 ms                                                      | 3.57 ms: 1.03x slower                                                |
| mako                       | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                |
| json                       | 5.12 ms                                                      | 5.27 ms: 1.03x slower                                                |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                 |
| 2to3                       | 285 ms                                                       | 294 ms: 1.03x slower                                                 |
| json_loads                 | 24.4 us                                                      | 25.2 us: 1.03x slower                                                |
| dulwich_log                | 65.4 ms                                                      | 68.0 ms: 1.04x slower                                                |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                               |
| json_dumps                 | 10.2 ms                                                      | 10.7 ms: 1.04x slower                                                |
| regex_v8                   | 23.6 ms                                                      | 24.7 ms: 1.04x slower                                                |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.05x slower                                               |
| async_tree_memoization_tg  | 540 ms                                                       | 568 ms: 1.05x slower                                                 |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 734 ms: 1.05x slower                                                 |
| pycparser                  | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                               |
| hexiom                     | 5.96 ms                                                      | 6.41 ms: 1.08x slower                                                |
| fannkuch                   | 350 ms                                                       | 380 ms: 1.09x slower                                                 |
| tomli_loads                | 2.16 sec                                                     | 2.35 sec: 1.09x slower                                               |
| python_startup             | 11.6 ms                                                      | 12.8 ms: 1.10x slower                                                |
| deltablue                  | 3.24 ms                                                      | 3.64 ms: 1.12x slower                                                |
| go                         | 150 ms                                                       | 169 ms: 1.13x slower                                                 |
| pyflate                    | 439 ms                                                       | 507 ms: 1.16x slower                                                 |
| telco                      | 6.96 ms                                                      | 8.11 ms: 1.16x slower                                                |
| richards_super             | 51.3 ms                                                      | 60.3 ms: 1.17x slower                                                |
| coverage                   | 66.7 ms                                                      | 79.4 ms: 1.19x slower                                                |
| richards                   | 45.7 ms                                                      | 54.6 ms: 1.19x slower                                                |
| python_startup_no_site     | 8.64 ms                                                      | 11.3 ms: 1.30x slower                                                |
| scimark_sor                | 109 ms                                                       | 144 ms: 1.32x slower                                                 |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                         |

Benchmark hidden because not significant (9): bench_thread_pool, asyncio_websockets, sqlglot_normalize, spectral_norm, deepcopy, create_gc_cycles, float, async_tree_memoization, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 93.85% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.86x