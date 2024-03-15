
# Results vs. 3.12.0

- fork: python
- ref: ca71987f4e3be56a369a
- machine: linux-x86_64
- commit hash: ca71987
- commit date: 2023-12-23
- overall geometric mean: 1.01x slower
- HPT reliability: 94.43%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 294 ms: 1.03x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.37 ms: 1.02x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.81 sec: 1.02x faster                                                       |
| tornado_http   | 121 ms                                                       | 118 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|---------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none           | 452 ms                                                       | 432 ms: 1.04x faster                                                         |
| async_tree_io_tg          | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                                       |
| async_tree_memoization_tg | 540 ms                                                       | 546 ms: 1.01x slower                                                         |
| async_tree_io             | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| Geometric mean            | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| float          | 76.6 ms                                                      | 79.4 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                        |
| regex_compile  | 144 ms                                                       | 142 ms: 1.01x faster                                                         |
| regex_dna      | 239 ms                                                       | 245 ms: 1.03x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 26.1 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.4 us: 1.07x faster                                                        |
| pickle               | 10.5 us                                                      | 10.0 us: 1.05x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.4 us: 1.03x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 310 us: 1.03x faster                                                         |
| unpickle_pure_python | 210 us                                                       | 210 us: 1.00x slower                                                         |
| xml_etree_process    | 58.4 ms                                                      | 59.4 ms: 1.02x slower                                                        |
| tomli_loads          | 2.16 sec                                                     | 2.21 sec: 1.02x slower                                                       |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.03x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| xml_etree_parse      | 144 ms                                                       | 149 ms: 1.04x slower                                                         |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (3): unpickle_list, xml_etree_generate, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.17x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                        |

All benchmarks:
===============

| Benchmark                 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231223-pythonperf2-x86_64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|---------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| comprehensions            | 21.9 us                                                      | 16.4 us: 1.34x faster                                                        |
| typing_runtime_protocols  | 152 us                                                       | 120 us: 1.27x faster                                                         |
| unpack_sequence           | 53.2 ns                                                      | 44.8 ns: 1.19x faster                                                        |
| raytrace                  | 298 ms                                                       | 257 ms: 1.16x faster                                                         |
| crypto_pyaes              | 80.3 ms                                                      | 69.6 ms: 1.15x faster                                                        |
| generators                | 37.4 ms                                                      | 34.0 ms: 1.10x faster                                                        |
| async_generators          | 390 ms                                                       | 357 ms: 1.09x faster                                                         |
| chaos                     | 64.0 ms                                                      | 58.8 ms: 1.09x faster                                                        |
| pickle_dict               | 32.5 us                                                      | 30.4 us: 1.07x faster                                                        |
| sympy_sum                 | 162 ms                                                       | 152 ms: 1.06x faster                                                         |
| logging_format            | 7.48 us                                                      | 7.06 us: 1.06x faster                                                        |
| scimark_monte_carlo       | 69.0 ms                                                      | 65.3 ms: 1.06x faster                                                        |
| pickle                    | 10.5 us                                                      | 10.0 us: 1.05x faster                                                        |
| async_tree_none           | 452 ms                                                       | 432 ms: 1.04x faster                                                         |
| logging_simple            | 6.71 us                                                      | 6.45 us: 1.04x faster                                                        |
| coroutines                | 23.0 ms                                                      | 22.1 ms: 1.04x faster                                                        |
| regex_effbot              | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                        |
| sympy_integrate           | 23.9 ms                                                      | 23.1 ms: 1.04x faster                                                        |
| sympy_str                 | 302 ms                                                       | 292 ms: 1.03x faster                                                         |
| asyncio_tcp               | 378 ms                                                       | 366 ms: 1.03x faster                                                         |
| nqueens                   | 89.9 ms                                                      | 87.0 ms: 1.03x faster                                                        |
| tornado_http              | 121 ms                                                       | 118 ms: 1.03x faster                                                         |
| sqlite_synth              | 2.77 us                                                      | 2.70 us: 1.03x faster                                                        |
| mdp                       | 2.57 sec                                                     | 2.50 sec: 1.03x faster                                                       |
| unpickle                  | 14.8 us                                                      | 14.4 us: 1.03x faster                                                        |
| pickle_pure_python        | 318 us                                                       | 310 us: 1.03x faster                                                         |
| docutils                  | 2.87 sec                                                     | 2.81 sec: 1.02x faster                                                       |
| scimark_fft               | 301 ms                                                       | 296 ms: 1.02x faster                                                         |
| regex_compile             | 144 ms                                                       | 142 ms: 1.01x faster                                                         |
| deepcopy_reduce           | 3.37 us                                                      | 3.33 us: 1.01x faster                                                        |
| asyncio_tcp_ssl           | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| spectral_norm             | 91.6 ms                                                      | 90.9 ms: 1.01x faster                                                        |
| pprint_pformat            | 1.65 sec                                                     | 1.64 sec: 1.01x faster                                                       |
| pathlib                   | 18.9 ms                                                      | 18.8 ms: 1.01x faster                                                        |
| pidigits                  | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| unpickle_pure_python      | 210 us                                                       | 210 us: 1.00x slower                                                         |
| sqlglot_normalize         | 116 ms                                                       | 116 ms: 1.01x slower                                                         |
| async_tree_io_tg          | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                                       |
| dask                      | 392 ms                                                       | 396 ms: 1.01x slower                                                         |
| async_tree_memoization_tg | 540 ms                                                       | 546 ms: 1.01x slower                                                         |
| deepcopy                  | 368 us                                                       | 374 us: 1.01x slower                                                         |
| xml_etree_process         | 58.4 ms                                                      | 59.4 ms: 1.02x slower                                                        |
| sqlglot_optimize          | 57.5 ms                                                      | 58.5 ms: 1.02x slower                                                        |
| chameleon                 | 7.23 ms                                                      | 7.37 ms: 1.02x slower                                                        |
| logging_silent            | 94.4 ns                                                      | 96.3 ns: 1.02x slower                                                        |
| tomli_loads               | 2.16 sec                                                     | 2.21 sec: 1.02x slower                                                       |
| async_tree_io             | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| regex_dna                 | 239 ms                                                       | 245 ms: 1.03x slower                                                         |
| json                      | 5.12 ms                                                      | 5.26 ms: 1.03x slower                                                        |
| sympy_expand              | 484 ms                                                       | 498 ms: 1.03x slower                                                         |
| 2to3                      | 285 ms                                                       | 294 ms: 1.03x slower                                                         |
| json_loads                | 24.4 us                                                      | 25.2 us: 1.03x slower                                                        |
| float                     | 76.6 ms                                                      | 79.4 ms: 1.04x slower                                                        |
| dulwich_log               | 65.4 ms                                                      | 67.7 ms: 1.04x slower                                                        |
| xml_etree_iterparse       | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| xml_etree_parse           | 144 ms                                                       | 149 ms: 1.04x slower                                                         |
| mako                      | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                        |
| deepcopy_memo             | 36.8 us                                                      | 38.7 us: 1.05x slower                                                        |
| json_dumps                | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                        |
| hexiom                    | 5.96 ms                                                      | 6.33 ms: 1.06x slower                                                        |
| pycparser                 | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                                       |
| gc_traversal              | 3.48 ms                                                      | 3.74 ms: 1.08x slower                                                        |
| python_startup            | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| deltablue                 | 3.24 ms                                                      | 3.53 ms: 1.09x slower                                                        |
| regex_v8                  | 23.6 ms                                                      | 26.1 ms: 1.10x slower                                                        |
| go                        | 150 ms                                                       | 167 ms: 1.12x slower                                                         |
| fannkuch                  | 350 ms                                                       | 392 ms: 1.12x slower                                                         |
| pyflate                   | 439 ms                                                       | 500 ms: 1.14x slower                                                         |
| richards_super            | 51.3 ms                                                      | 59.0 ms: 1.15x slower                                                        |
| richards                  | 45.7 ms                                                      | 53.3 ms: 1.17x slower                                                        |
| telco                     | 6.96 ms                                                      | 8.16 ms: 1.17x slower                                                        |
| coverage                  | 66.7 ms                                                      | 78.4 ms: 1.18x slower                                                        |
| python_startup_no_site    | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| scimark_sor               | 109 ms                                                       | 143 ms: 1.32x slower                                                         |
| Geometric mean            | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (19): bench_mp_pool, async_tree_cpu_io_mixed, nbody, scimark_sparse_mat_mult, sqlglot_parse, meteor_contest, unpickle_list, async_tree_none_tg, sqlglot_transpile, async_tree_memoization, pprint_safe_repr, xml_etree_generate, asyncio_websockets, async_tree_cpu_io_mixed_tg, scimark_lu, pickle_list, create_gc_cycles, bench_thread_pool, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 94.43% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.88x