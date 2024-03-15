
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 302 ms: 1.06x slower                                                 |
| chameleon      | 7.23 ms                                                      | 7.78 ms: 1.08x slower                                                |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                               |
| Geometric mean | (ref)                                                        | 1.03x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                 |
| async_tree_memoization     | 544 ms                                                       | 559 ms: 1.03x slower                                                 |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                 |
| async_tree_none_tg         | 431 ms                                                       | 446 ms: 1.04x slower                                                 |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                               |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                               |
| async_tree_memoization_tg  | 540 ms                                                       | 570 ms: 1.06x slower                                                 |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                         |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 263 ms: 1.01x faster                                                 |
| float          | 76.6 ms                                                      | 82.2 ms: 1.07x slower                                                |
| nbody          | 88.0 ms                                                      | 108 ms: 1.23x slower                                                 |
| Geometric mean | (ref)                                                        | 1.09x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 244 ms: 1.02x slower                                                 |
| regex_compile  | 144 ms                                                       | 150 ms: 1.04x slower                                                 |
| regex_v8       | 23.6 ms                                                      | 25.3 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                        | 1.04x slower                                                         |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 9.88 us: 1.07x faster                                                |
| pickle_list          | 4.43 us                                                      | 4.23 us: 1.05x faster                                                |
| pickle_pure_python   | 318 us                                                       | 313 us: 1.02x faster                                                 |
| pickle_dict          | 32.5 us                                                      | 32.4 us: 1.00x faster                                                |
| json_loads           | 24.4 us                                                      | 24.5 us: 1.01x slower                                                |
| unpickle_list        | 4.66 us                                                      | 4.71 us: 1.01x slower                                                |
| xml_etree_process    | 58.4 ms                                                      | 59.5 ms: 1.02x slower                                                |
| xml_etree_generate   | 86.1 ms                                                      | 88.0 ms: 1.02x slower                                                |
| xml_etree_parse      | 144 ms                                                       | 148 ms: 1.03x slower                                                 |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                                 |
| unpickle_pure_python | 210 us                                                       | 221 us: 1.06x slower                                                 |
| tomli_loads          | 2.16 sec                                                     | 2.36 sec: 1.09x slower                                               |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                         |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 12.0 ms: 1.20x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 120 us: 1.26x faster                                                 |
| unpack_sequence            | 53.2 ns                                                      | 44.0 ns: 1.21x faster                                                |
| raytrace                   | 298 ms                                                       | 277 ms: 1.08x faster                                                 |
| generators                 | 37.4 ms                                                      | 34.9 ms: 1.07x faster                                                |
| pickle                     | 10.5 us                                                      | 9.88 us: 1.07x faster                                                |
| pickle_list                | 4.43 us                                                      | 4.23 us: 1.05x faster                                                |
| comprehensions             | 21.9 us                                                      | 21.0 us: 1.04x faster                                                |
| logging_format             | 7.48 us                                                      | 7.24 us: 1.03x faster                                                |
| async_generators           | 390 ms                                                       | 380 ms: 1.03x faster                                                 |
| asyncio_tcp                | 378 ms                                                       | 369 ms: 1.02x faster                                                 |
| coroutines                 | 23.0 ms                                                      | 22.5 ms: 1.02x faster                                                |
| create_gc_cycles           | 1.59 ms                                                      | 1.56 ms: 1.02x faster                                                |
| pickle_pure_python         | 318 us                                                       | 313 us: 1.02x faster                                                 |
| logging_simple             | 6.71 us                                                      | 6.61 us: 1.02x faster                                                |
| sqlite_synth               | 2.77 us                                                      | 2.73 us: 1.02x faster                                                |
| pidigits                   | 265 ms                                                       | 263 ms: 1.01x faster                                                 |
| sympy_sum                  | 162 ms                                                       | 161 ms: 1.01x faster                                                 |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                               |
| pickle_dict                | 32.5 us                                                      | 32.4 us: 1.00x faster                                                |
| docutils                   | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                               |
| json_loads                 | 24.4 us                                                      | 24.5 us: 1.01x slower                                                |
| sympy_str                  | 302 ms                                                       | 304 ms: 1.01x slower                                                 |
| deepcopy                   | 368 us                                                       | 371 us: 1.01x slower                                                 |
| unpickle_list              | 4.66 us                                                      | 4.71 us: 1.01x slower                                                |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.02x slower                                                |
| deepcopy_memo              | 36.8 us                                                      | 37.4 us: 1.02x slower                                                |
| mdp                        | 2.57 sec                                                     | 2.62 sec: 1.02x slower                                               |
| xml_etree_process          | 58.4 ms                                                      | 59.5 ms: 1.02x slower                                                |
| xml_etree_generate         | 86.1 ms                                                      | 88.0 ms: 1.02x slower                                                |
| sympy_integrate            | 23.9 ms                                                      | 24.4 ms: 1.02x slower                                                |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                 |
| regex_dna                  | 239 ms                                                       | 244 ms: 1.02x slower                                                 |
| sqlglot_parse              | 1.38 ms                                                      | 1.41 ms: 1.02x slower                                                |
| json                       | 5.12 ms                                                      | 5.25 ms: 1.03x slower                                                |
| async_tree_memoization     | 544 ms                                                       | 559 ms: 1.03x slower                                                 |
| sqlglot_transpile          | 1.78 ms                                                      | 1.82 ms: 1.03x slower                                                |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                 |
| xml_etree_parse            | 144 ms                                                       | 148 ms: 1.03x slower                                                 |
| meteor_contest             | 128 ms                                                       | 133 ms: 1.03x slower                                                 |
| async_tree_none_tg         | 431 ms                                                       | 446 ms: 1.04x slower                                                 |
| dask                       | 392 ms                                                       | 406 ms: 1.04x slower                                                 |
| pycparser                  | 1.23 sec                                                     | 1.28 sec: 1.04x slower                                               |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                               |
| sqlglot_normalize          | 116 ms                                                       | 120 ms: 1.04x slower                                                 |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                |
| regex_compile              | 144 ms                                                       | 150 ms: 1.04x slower                                                 |
| scimark_lu                 | 98.8 ms                                                      | 103 ms: 1.04x slower                                                 |
| crypto_pyaes               | 80.3 ms                                                      | 83.6 ms: 1.04x slower                                                |
| dulwich_log                | 65.4 ms                                                      | 68.2 ms: 1.04x slower                                                |
| xml_etree_iterparse        | 103 ms                                                       | 107 ms: 1.04x slower                                                 |
| sympy_expand               | 484 ms                                                       | 509 ms: 1.05x slower                                                 |
| logging_silent             | 94.4 ns                                                      | 99.2 ns: 1.05x slower                                                |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                               |
| async_tree_memoization_tg  | 540 ms                                                       | 570 ms: 1.06x slower                                                 |
| unpickle_pure_python       | 210 us                                                       | 221 us: 1.06x slower                                                 |
| 2to3                       | 285 ms                                                       | 302 ms: 1.06x slower                                                 |
| pprint_safe_repr           | 807 ms                                                       | 861 ms: 1.07x slower                                                 |
| pprint_pformat             | 1.65 sec                                                     | 1.77 sec: 1.07x slower                                               |
| regex_v8                   | 23.6 ms                                                      | 25.3 ms: 1.07x slower                                                |
| float                      | 76.6 ms                                                      | 82.2 ms: 1.07x slower                                                |
| chameleon                  | 7.23 ms                                                      | 7.78 ms: 1.08x slower                                                |
| sqlglot_optimize           | 57.5 ms                                                      | 62.0 ms: 1.08x slower                                                |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                |
| tomli_loads                | 2.16 sec                                                     | 2.36 sec: 1.09x slower                                               |
| chaos                      | 64.0 ms                                                      | 71.2 ms: 1.11x slower                                                |
| richards_super             | 51.3 ms                                                      | 57.8 ms: 1.13x slower                                                |
| richards                   | 45.7 ms                                                      | 51.7 ms: 1.13x slower                                                |
| nqueens                    | 89.9 ms                                                      | 102 ms: 1.14x slower                                                 |
| scimark_monte_carlo        | 69.0 ms                                                      | 79.1 ms: 1.15x slower                                                |
| go                         | 150 ms                                                       | 174 ms: 1.16x slower                                                 |
| gc_traversal               | 3.48 ms                                                      | 4.10 ms: 1.18x slower                                                |
| pyflate                    | 439 ms                                                       | 517 ms: 1.18x slower                                                 |
| telco                      | 6.96 ms                                                      | 8.25 ms: 1.19x slower                                                |
| mako                       | 10.0 ms                                                      | 12.0 ms: 1.20x slower                                                |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 5.11 ms: 1.21x slower                                                |
| nbody                      | 88.0 ms                                                      | 108 ms: 1.23x slower                                                 |
| scimark_fft                | 301 ms                                                       | 371 ms: 1.23x slower                                                 |
| coverage                   | 66.7 ms                                                      | 83.1 ms: 1.25x slower                                                |
| fannkuch                   | 350 ms                                                       | 439 ms: 1.25x slower                                                 |
| deltablue                  | 3.24 ms                                                      | 4.06 ms: 1.26x slower                                                |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                |
| scimark_sor                | 109 ms                                                       | 144 ms: 1.32x slower                                                 |
| spectral_norm              | 91.6 ms                                                      | 121 ms: 1.32x slower                                                 |
| hexiom                     | 5.96 ms                                                      | 7.96 ms: 1.34x slower                                                |
| Geometric mean             | (ref)                                                        | 1.05x slower                                                         |

Benchmark hidden because not significant (9): async_tree_none, asyncio_websockets, unpickle, tornado_http, deepcopy_reduce, regex_effbot, bench_thread_pool, bench_mp_pool, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 0.92x