
# Results vs. 3.12.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: linux-x86_64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 309 ms: 1.08x slower                                                         |
| chameleon      | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.94 sec: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.02x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 561 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 562 ms: 1.04x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 448 ms: 1.04x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 266 ms: 1.00x slower                                                         |
| float          | 76.6 ms                                                      | 104 ms: 1.36x slower                                                         |
| nbody          | 88.0 ms                                                      | 130 ms: 1.48x slower                                                         |
| Geometric mean | (ref)                                                        | 1.27x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.64 ms: 1.02x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 25.1 ms: 1.06x slower                                                        |
| regex_compile  | 144 ms                                                       | 172 ms: 1.19x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.7 us: 1.03x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 313 us: 1.02x faster                                                         |
| pickle_list          | 4.43 us                                                      | 4.46 us: 1.01x slower                                                        |
| json_loads           | 24.4 us                                                      | 24.7 us: 1.01x slower                                                        |
| pickle               | 10.5 us                                                      | 10.8 us: 1.02x slower                                                        |
| unpickle             | 14.8 us                                                      | 15.2 us: 1.02x slower                                                        |
| unpickle_list        | 4.66 us                                                      | 4.84 us: 1.04x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 150 ms: 1.04x slower                                                         |
| json_dumps           | 10.2 ms                                                      | 10.9 ms: 1.07x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 62.8 ms: 1.08x slower                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 94.3 ms: 1.09x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| unpickle_pure_python | 210 us                                                       | 243 us: 1.16x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.83 sec: 1.31x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 15.3 ms: 1.53x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 125 us: 1.21x faster                                                         |
| unpack_sequence            | 53.2 ns                                                      | 44.4 ns: 1.20x faster                                                        |
| generators                 | 37.4 ms                                                      | 34.5 ms: 1.09x faster                                                        |
| async_generators           | 390 ms                                                       | 370 ms: 1.05x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.1 ms: 1.04x faster                                                        |
| pickle_dict                | 32.5 us                                                      | 31.7 us: 1.03x faster                                                        |
| pickle_pure_python         | 318 us                                                       | 313 us: 1.02x faster                                                         |
| pidigits                   | 265 ms                                                       | 266 ms: 1.00x slower                                                         |
| pickle_list                | 4.43 us                                                      | 4.46 us: 1.01x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.81 us: 1.01x slower                                                        |
| json_loads                 | 24.4 us                                                      | 24.7 us: 1.01x slower                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.64 ms: 1.02x slower                                                        |
| deepcopy                   | 368 us                                                       | 376 us: 1.02x slower                                                         |
| pickle                     | 10.5 us                                                      | 10.8 us: 1.02x slower                                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                         |
| mdp                        | 2.57 sec                                                     | 2.63 sec: 1.02x slower                                                       |
| unpickle                   | 14.8 us                                                      | 15.2 us: 1.02x slower                                                        |
| logging_simple             | 6.71 us                                                      | 6.87 us: 1.02x slower                                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.02x slower                                                         |
| docutils                   | 2.87 sec                                                     | 2.94 sec: 1.03x slower                                                       |
| json                       | 5.12 ms                                                      | 5.25 ms: 1.03x slower                                                        |
| sympy_sum                  | 162 ms                                                       | 167 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 561 ms: 1.03x slower                                                         |
| bench_thread_pool          | 950 us                                                       | 982 us: 1.03x slower                                                         |
| raytrace                   | 298 ms                                                       | 308 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| dask                       | 392 ms                                                       | 407 ms: 1.04x slower                                                         |
| unpickle_list              | 4.66 us                                                      | 4.84 us: 1.04x slower                                                        |
| async_tree_memoization_tg  | 540 ms                                                       | 562 ms: 1.04x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 448 ms: 1.04x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 24.9 ms: 1.04x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 150 ms: 1.04x slower                                                         |
| logging_silent             | 94.4 ns                                                      | 98.5 ns: 1.04x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                       |
| sqlglot_transpile          | 1.78 ms                                                      | 1.87 ms: 1.05x slower                                                        |
| sqlglot_parse              | 1.38 ms                                                      | 1.45 ms: 1.06x slower                                                        |
| scimark_lu                 | 98.8 ms                                                      | 104 ms: 1.06x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 25.1 ms: 1.06x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 10.9 ms: 1.07x slower                                                        |
| gc_traversal               | 3.48 ms                                                      | 3.72 ms: 1.07x slower                                                        |
| sympy_str                  | 302 ms                                                       | 324 ms: 1.07x slower                                                         |
| pycparser                  | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                                       |
| sqlglot_normalize          | 116 ms                                                       | 124 ms: 1.07x slower                                                         |
| xml_etree_process          | 58.4 ms                                                      | 62.8 ms: 1.08x slower                                                        |
| mypy2                      | 830 ms                                                       | 893 ms: 1.08x slower                                                         |
| meteor_contest             | 128 ms                                                       | 138 ms: 1.08x slower                                                         |
| crypto_pyaes               | 80.3 ms                                                      | 87.0 ms: 1.08x slower                                                        |
| 2to3                       | 285 ms                                                       | 309 ms: 1.08x slower                                                         |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 71.3 ms: 1.09x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 94.3 ms: 1.09x slower                                                        |
| deepcopy_memo              | 36.8 us                                                      | 40.7 us: 1.11x slower                                                        |
| sympy_expand               | 484 ms                                                       | 537 ms: 1.11x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 63.9 ms: 1.11x slower                                                        |
| chameleon                  | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                        |
| xml_etree_iterparse        | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| comprehensions             | 21.9 us                                                      | 25.1 us: 1.15x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 927 ms: 1.15x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.91 sec: 1.15x slower                                                       |
| unpickle_pure_python       | 210 us                                                       | 243 us: 1.16x slower                                                         |
| richards_super             | 51.3 ms                                                      | 60.0 ms: 1.17x slower                                                        |
| richards                   | 45.7 ms                                                      | 54.0 ms: 1.18x slower                                                        |
| regex_compile              | 144 ms                                                       | 172 ms: 1.19x slower                                                         |
| go                         | 150 ms                                                       | 179 ms: 1.19x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.36 ms: 1.20x slower                                                        |
| coverage                   | 66.7 ms                                                      | 80.2 ms: 1.20x slower                                                        |
| chaos                      | 64.0 ms                                                      | 77.8 ms: 1.22x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 109 ms: 1.22x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 87.8 ms: 1.27x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.83 sec: 1.31x slower                                                       |
| pyflate                    | 439 ms                                                       | 581 ms: 1.33x slower                                                         |
| scimark_sor                | 109 ms                                                       | 146 ms: 1.34x slower                                                         |
| fannkuch                   | 350 ms                                                       | 474 ms: 1.35x slower                                                         |
| float                      | 76.6 ms                                                      | 104 ms: 1.36x slower                                                         |
| scimark_fft                | 301 ms                                                       | 436 ms: 1.45x slower                                                         |
| nbody                      | 88.0 ms                                                      | 130 ms: 1.48x slower                                                         |
| mako                       | 10.0 ms                                                      | 15.3 ms: 1.53x slower                                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.63 ms: 1.58x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 9.78 ms: 1.64x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 5.42 ms: 1.67x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 163 ms: 1.77x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.10x slower                                                                 |

Benchmark hidden because not significant (10): async_tree_none, logging_format, asyncio_tcp, deepcopy_reduce, asyncio_websockets, asyncio_tcp_ssl, regex_dna, create_gc_cycles, tornado_http, bench_mp_pool
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x