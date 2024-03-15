
# Results vs. 3.12.0

- fork: python
- ref: ae460d450ab854ca66d5
- machine: linux-x86_64
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 301 ms: 1.06x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.18 ms: 1.01x faster                                                        |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.01x slower                                                       |
| tornado_http   | 121 ms                                                       | 123 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 436 ms: 1.04x faster                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 709 ms: 1.02x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 553 ms: 1.02x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 81.7 ms: 1.07x slower                                                        |
| nbody          | 88.0 ms                                                      | 106 ms: 1.21x slower                                                         |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                        |
| regex_compile  | 144 ms                                                       | 146 ms: 1.02x slower                                                         |
| regex_dna      | 239 ms                                                       | 249 ms: 1.04x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 26.1 ms: 1.11x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.8 us: 1.06x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 305 us: 1.04x faster                                                         |
| pickle               | 10.5 us                                                      | 10.3 us: 1.03x faster                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 84.7 ms: 1.02x faster                                                        |
| pickle_list          | 4.43 us                                                      | 4.47 us: 1.01x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 104 ms: 1.01x slower                                                         |
| unpickle_list        | 4.66 us                                                      | 4.76 us: 1.02x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| json_dumps           | 10.2 ms                                                      | 10.5 ms: 1.03x slower                                                        |
| unpickle             | 14.8 us                                                      | 15.3 us: 1.03x slower                                                        |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.04x slower                                                        |
| tomli_loads          | 2.16 sec                                                     | 2.30 sec: 1.06x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 228 us: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.19x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 11.9 ms: 1.19x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 120 us: 1.27x faster                                                         |
| unpack_sequence            | 53.2 ns                                                      | 44.8 ns: 1.19x faster                                                        |
| comprehensions             | 21.9 us                                                      | 19.2 us: 1.14x faster                                                        |
| generators                 | 37.4 ms                                                      | 33.6 ms: 1.12x faster                                                        |
| raytrace                   | 298 ms                                                       | 278 ms: 1.07x faster                                                         |
| pickle_dict                | 32.5 us                                                      | 30.8 us: 1.06x faster                                                        |
| pickle_pure_python         | 318 us                                                       | 305 us: 1.04x faster                                                         |
| async_tree_none            | 452 ms                                                       | 436 ms: 1.04x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                                        |
| create_gc_cycles           | 1.59 ms                                                      | 1.54 ms: 1.03x faster                                                        |
| sympy_sum                  | 162 ms                                                       | 158 ms: 1.03x faster                                                         |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.03x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                        |
| async_generators           | 390 ms                                                       | 382 ms: 1.02x faster                                                         |
| deepcopy_reduce            | 3.37 us                                                      | 3.31 us: 1.02x faster                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 84.7 ms: 1.02x faster                                                        |
| sympy_str                  | 302 ms                                                       | 298 ms: 1.01x faster                                                         |
| mdp                        | 2.57 sec                                                     | 2.54 sec: 1.01x faster                                                       |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| logging_simple             | 6.71 us                                                      | 6.66 us: 1.01x faster                                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                                       |
| logging_format             | 7.48 us                                                      | 7.43 us: 1.01x faster                                                        |
| chameleon                  | 7.23 ms                                                      | 7.18 ms: 1.01x faster                                                        |
| asyncio_tcp                | 378 ms                                                       | 376 ms: 1.01x faster                                                         |
| sympy_integrate            | 23.9 ms                                                      | 23.8 ms: 1.00x faster                                                        |
| pathlib                    | 18.9 ms                                                      | 18.8 ms: 1.00x faster                                                        |
| docutils                   | 2.87 sec                                                     | 2.88 sec: 1.01x slower                                                       |
| scimark_lu                 | 98.8 ms                                                      | 99.4 ms: 1.01x slower                                                        |
| pickle_list                | 4.43 us                                                      | 4.47 us: 1.01x slower                                                        |
| xml_etree_iterparse        | 103 ms                                                       | 104 ms: 1.01x slower                                                         |
| regex_compile              | 144 ms                                                       | 146 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 709 ms: 1.02x slower                                                         |
| tornado_http               | 121 ms                                                       | 123 ms: 1.02x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.40 ms: 1.02x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 96.2 ns: 1.02x slower                                                        |
| unpickle_list              | 4.66 us                                                      | 4.76 us: 1.02x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 553 ms: 1.02x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 119 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| bench_thread_pool          | 950 us                                                       | 976 us: 1.03x slower                                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.83 ms: 1.03x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 10.5 ms: 1.03x slower                                                        |
| dask                       | 392 ms                                                       | 404 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| unpickle                   | 14.8 us                                                      | 15.3 us: 1.03x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| json_loads                 | 24.4 us                                                      | 25.2 us: 1.04x slower                                                        |
| meteor_contest             | 128 ms                                                       | 133 ms: 1.04x slower                                                         |
| json                       | 5.12 ms                                                      | 5.31 ms: 1.04x slower                                                        |
| sympy_expand               | 484 ms                                                       | 505 ms: 1.04x slower                                                         |
| regex_dna                  | 239 ms                                                       | 249 ms: 1.04x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.74 sec: 1.05x slower                                                       |
| dulwich_log                | 65.4 ms                                                      | 69.0 ms: 1.06x slower                                                        |
| 2to3                       | 285 ms                                                       | 301 ms: 1.06x slower                                                         |
| pprint_safe_repr           | 807 ms                                                       | 856 ms: 1.06x slower                                                         |
| tomli_loads                | 2.16 sec                                                     | 2.30 sec: 1.06x slower                                                       |
| gc_traversal               | 3.48 ms                                                      | 3.71 ms: 1.07x slower                                                        |
| float                      | 76.6 ms                                                      | 81.7 ms: 1.07x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                                       |
| sqlglot_optimize           | 57.5 ms                                                      | 61.5 ms: 1.07x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 96.7 ms: 1.08x slower                                                        |
| chaos                      | 64.0 ms                                                      | 69.4 ms: 1.08x slower                                                        |
| unpickle_pure_python       | 210 us                                                       | 228 us: 1.09x slower                                                         |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                        |
| richards_super             | 51.3 ms                                                      | 56.4 ms: 1.10x slower                                                        |
| regex_v8                   | 23.6 ms                                                      | 26.1 ms: 1.11x slower                                                        |
| richards                   | 45.7 ms                                                      | 50.6 ms: 1.11x slower                                                        |
| go                         | 150 ms                                                       | 167 ms: 1.11x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 77.6 ms: 1.13x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 3.69 ms: 1.14x slower                                                        |
| scimark_fft                | 301 ms                                                       | 345 ms: 1.15x slower                                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.95 ms: 1.18x slower                                                        |
| fannkuch                   | 350 ms                                                       | 412 ms: 1.18x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.24 ms: 1.18x slower                                                        |
| mako                       | 10.0 ms                                                      | 11.9 ms: 1.19x slower                                                        |
| coverage                   | 66.7 ms                                                      | 79.5 ms: 1.19x slower                                                        |
| nbody                      | 88.0 ms                                                      | 106 ms: 1.21x slower                                                         |
| spectral_norm              | 91.6 ms                                                      | 111 ms: 1.21x slower                                                         |
| pyflate                    | 439 ms                                                       | 538 ms: 1.23x slower                                                         |
| hexiom                     | 5.96 ms                                                      | 7.60 ms: 1.28x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                        |
| scimark_sor                | 109 ms                                                       | 141 ms: 1.29x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.04x slower                                                                 |

Benchmark hidden because not significant (10): deepcopy, bench_mp_pool, asyncio_websockets, sqlite_synth, xml_etree_process, async_tree_memoization, deepcopy_memo, async_tree_cpu_io_mixed, crypto_pyaes, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.92x