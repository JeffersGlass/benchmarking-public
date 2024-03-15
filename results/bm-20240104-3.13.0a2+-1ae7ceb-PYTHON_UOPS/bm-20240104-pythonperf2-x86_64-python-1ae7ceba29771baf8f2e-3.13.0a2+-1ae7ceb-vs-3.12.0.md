
# Results vs. 3.12.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 310 ms: 1.09x slower                                                         |
| chameleon      | 7.23 ms                                                      | 8.01 ms: 1.11x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                       |
| tornado_http   | 121 ms                                                       | 123 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 696 ms                                                       | 714 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 562 ms: 1.03x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 567 ms: 1.05x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 103 ms: 1.35x slower                                                         |
| nbody          | 88.0 ms                                                      | 128 ms: 1.45x slower                                                         |
| Geometric mean | (ref)                                                        | 1.25x slower                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.51 ms: 1.02x faster                                                        |
| regex_v8       | 23.6 ms                                                      | 25.9 ms: 1.09x slower                                                        |
| regex_compile  | 144 ms                                                       | 173 ms: 1.20x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.2 us: 1.04x faster                                                        |
| pickle               | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.6 us: 1.02x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 314 us: 1.01x faster                                                         |
| unpickle_list        | 4.66 us                                                      | 4.68 us: 1.00x slower                                                        |
| json_loads           | 24.4 us                                                      | 24.7 us: 1.01x slower                                                        |
| pickle_list          | 4.43 us                                                      | 4.57 us: 1.03x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 150 ms: 1.04x slower                                                         |
| xml_etree_generate   | 86.1 ms                                                      | 92.1 ms: 1.07x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 11.0 ms: 1.07x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 62.7 ms: 1.07x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| unpickle_pure_python | 210 us                                                       | 241 us: 1.15x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.77 sec: 1.28x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 15.0 ms: 1.50x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpack_sequence            | 53.2 ns                                                      | 44.0 ns: 1.21x faster                                                        |
| typing_runtime_protocols   | 152 us                                                       | 129 us: 1.17x faster                                                         |
| generators                 | 37.4 ms                                                      | 34.1 ms: 1.10x faster                                                        |
| async_generators           | 390 ms                                                       | 374 ms: 1.04x faster                                                         |
| pickle_dict                | 32.5 us                                                      | 31.2 us: 1.04x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.2 ms: 1.04x faster                                                        |
| pickle                     | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.51 ms: 1.02x faster                                                        |
| unpickle                   | 14.8 us                                                      | 14.6 us: 1.02x faster                                                        |
| pickle_pure_python         | 318 us                                                       | 314 us: 1.01x faster                                                         |
| asyncio_tcp                | 378 ms                                                       | 375 ms: 1.01x faster                                                         |
| logging_format             | 7.48 us                                                      | 7.44 us: 1.01x faster                                                        |
| unpickle_list              | 4.66 us                                                      | 4.68 us: 1.00x slower                                                        |
| raytrace                   | 298 ms                                                       | 301 ms: 1.01x slower                                                         |
| json_loads                 | 24.4 us                                                      | 24.7 us: 1.01x slower                                                        |
| tornado_http               | 121 ms                                                       | 123 ms: 1.02x slower                                                         |
| sqlite_synth               | 2.77 us                                                      | 2.82 us: 1.02x slower                                                        |
| json                       | 5.12 ms                                                      | 5.20 ms: 1.02x slower                                                        |
| deepcopy                   | 368 us                                                       | 375 us: 1.02x slower                                                         |
| logging_simple             | 6.71 us                                                      | 6.85 us: 1.02x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                        |
| mdp                        | 2.57 sec                                                     | 2.63 sec: 1.02x slower                                                       |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 714 ms: 1.03x slower                                                         |
| docutils                   | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                       |
| bench_thread_pool          | 950 us                                                       | 977 us: 1.03x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                         |
| pickle_list                | 4.43 us                                                      | 4.57 us: 1.03x slower                                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 562 ms: 1.03x slower                                                         |
| xml_etree_parse            | 144 ms                                                       | 150 ms: 1.04x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                       |
| sympy_sum                  | 162 ms                                                       | 170 ms: 1.05x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 567 ms: 1.05x slower                                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.87 ms: 1.05x slower                                                        |
| dask                       | 392 ms                                                       | 414 ms: 1.06x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.45 ms: 1.06x slower                                                        |
| sympy_integrate            | 23.9 ms                                                      | 25.3 ms: 1.06x slower                                                        |
| scimark_lu                 | 98.8 ms                                                      | 105 ms: 1.06x slower                                                         |
| xml_etree_generate         | 86.1 ms                                                      | 92.1 ms: 1.07x slower                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 86.1 ms: 1.07x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 11.0 ms: 1.07x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                                       |
| xml_etree_process          | 58.4 ms                                                      | 62.7 ms: 1.07x slower                                                        |
| gc_traversal               | 3.48 ms                                                      | 3.74 ms: 1.08x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 102 ns: 1.08x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 125 ms: 1.08x slower                                                         |
| mypy2                      | 830 ms                                                       | 895 ms: 1.08x slower                                                         |
| sympy_str                  | 302 ms                                                       | 326 ms: 1.08x slower                                                         |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| meteor_contest             | 128 ms                                                       | 139 ms: 1.08x slower                                                         |
| 2to3                       | 285 ms                                                       | 310 ms: 1.09x slower                                                         |
| deepcopy_memo              | 36.8 us                                                      | 40.1 us: 1.09x slower                                                        |
| regex_v8                   | 23.6 ms                                                      | 25.9 ms: 1.09x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 72.4 ms: 1.11x slower                                                        |
| chameleon                  | 7.23 ms                                                      | 8.01 ms: 1.11x slower                                                        |
| sqlglot_optimize           | 57.5 ms                                                      | 63.8 ms: 1.11x slower                                                        |
| sympy_expand               | 484 ms                                                       | 543 ms: 1.12x slower                                                         |
| xml_etree_iterparse        | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| pprint_safe_repr           | 807 ms                                                       | 915 ms: 1.13x slower                                                         |
| comprehensions             | 21.9 us                                                      | 24.9 us: 1.14x slower                                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.89 sec: 1.14x slower                                                       |
| richards_super             | 51.3 ms                                                      | 58.7 ms: 1.14x slower                                                        |
| unpickle_pure_python       | 210 us                                                       | 241 us: 1.15x slower                                                         |
| richards                   | 45.7 ms                                                      | 52.9 ms: 1.16x slower                                                        |
| chaos                      | 64.0 ms                                                      | 76.0 ms: 1.19x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 107 ms: 1.20x slower                                                         |
| regex_compile              | 144 ms                                                       | 173 ms: 1.20x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.41 ms: 1.21x slower                                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 85.8 ms: 1.24x slower                                                        |
| go                         | 150 ms                                                       | 187 ms: 1.25x slower                                                         |
| python_startup_no_site     | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.77 sec: 1.28x slower                                                       |
| coverage                   | 66.7 ms                                                      | 85.7 ms: 1.29x slower                                                        |
| pyflate                    | 439 ms                                                       | 574 ms: 1.31x slower                                                         |
| float                      | 76.6 ms                                                      | 103 ms: 1.35x slower                                                         |
| fannkuch                   | 350 ms                                                       | 473 ms: 1.35x slower                                                         |
| scimark_sor                | 109 ms                                                       | 148 ms: 1.36x slower                                                         |
| scimark_fft                | 301 ms                                                       | 423 ms: 1.40x slower                                                         |
| nbody                      | 88.0 ms                                                      | 128 ms: 1.45x slower                                                         |
| mako                       | 10.0 ms                                                      | 15.0 ms: 1.50x slower                                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.37 ms: 1.51x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 9.85 ms: 1.65x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 5.49 ms: 1.70x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 164 ms: 1.79x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.10x slower                                                                 |

Benchmark hidden because not significant (8): bench_mp_pool, async_tree_none, asyncio_tcp_ssl, asyncio_websockets, regex_dna, pidigits, deepcopy_reduce, create_gc_cycles
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x