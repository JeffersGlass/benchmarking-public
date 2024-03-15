
# Results vs. 3.12.0

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: linux-x86_64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.01x slower
- HPT reliability: 94.60%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.86x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 293 ms: 1.03x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.34 ms: 1.02x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                                       |
| tornado_http   | 121 ms                                                       | 119 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 432 ms: 1.04x faster                                                         |
| async_tree_none_tg         | 431 ms                                                       | 436 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 564 ms: 1.04x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 85.9 ms: 1.02x faster                                                        |
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| float          | 76.6 ms                                                      | 79.4 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                        |
| regex_dna      | 239 ms                                                       | 236 ms: 1.01x faster                                                         |
| regex_compile  | 144 ms                                                       | 145 ms: 1.01x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 24.8 ms: 1.05x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 10.3 us: 1.02x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.5 us: 1.02x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 312 us: 1.02x faster                                                         |
| xml_etree_generate   | 86.1 ms                                                      | 85.1 ms: 1.01x faster                                                        |
| pickle_dict          | 32.5 us                                                      | 32.8 us: 1.01x slower                                                        |
| pickle_list          | 4.43 us                                                      | 4.46 us: 1.01x slower                                                        |
| unpickle_list        | 4.66 us                                                      | 4.71 us: 1.01x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 213 us: 1.02x slower                                                         |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.23 sec: 1.03x slower                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| json_loads           | 24.4 us                                                      | 25.5 us: 1.05x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.8 ms: 1.10x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.2 ms: 1.30x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.20x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| comprehensions             | 21.9 us                                                      | 16.9 us: 1.30x faster                                                        |
| typing_runtime_protocols   | 152 us                                                       | 126 us: 1.20x faster                                                         |
| crypto_pyaes               | 80.3 ms                                                      | 69.6 ms: 1.15x faster                                                        |
| unpack_sequence            | 53.2 ns                                                      | 48.3 ns: 1.10x faster                                                        |
| generators                 | 37.4 ms                                                      | 34.3 ms: 1.09x faster                                                        |
| sympy_sum                  | 162 ms                                                       | 150 ms: 1.08x faster                                                         |
| async_generators           | 390 ms                                                       | 362 ms: 1.08x faster                                                         |
| raytrace                   | 298 ms                                                       | 278 ms: 1.07x faster                                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.58 sec: 1.05x faster                                                       |
| pprint_safe_repr           | 807 ms                                                       | 773 ms: 1.04x faster                                                         |
| async_tree_none            | 452 ms                                                       | 432 ms: 1.04x faster                                                         |
| sympy_integrate            | 23.9 ms                                                      | 23.0 ms: 1.04x faster                                                        |
| sympy_str                  | 302 ms                                                       | 290 ms: 1.04x faster                                                         |
| chaos                      | 64.0 ms                                                      | 62.0 ms: 1.03x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.70 us: 1.03x faster                                                        |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.02x faster                                                        |
| nbody                      | 88.0 ms                                                      | 85.9 ms: 1.02x faster                                                        |
| asyncio_tcp                | 378 ms                                                       | 369 ms: 1.02x faster                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 67.4 ms: 1.02x faster                                                        |
| unpickle                   | 14.8 us                                                      | 14.5 us: 1.02x faster                                                        |
| tornado_http               | 121 ms                                                       | 119 ms: 1.02x faster                                                         |
| pickle_pure_python         | 318 us                                                       | 312 us: 1.02x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.5 ms: 1.02x faster                                                        |
| mdp                        | 2.57 sec                                                     | 2.52 sec: 1.02x faster                                                       |
| nqueens                    | 89.9 ms                                                      | 88.3 ms: 1.02x faster                                                        |
| deepcopy_reduce            | 3.37 us                                                      | 3.32 us: 1.02x faster                                                        |
| docutils                   | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                                       |
| spectral_norm              | 91.6 ms                                                      | 90.5 ms: 1.01x faster                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 85.1 ms: 1.01x faster                                                        |
| regex_dna                  | 239 ms                                                       | 236 ms: 1.01x faster                                                         |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| pidigits                   | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| meteor_contest             | 128 ms                                                       | 129 ms: 1.00x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 116 ms: 1.01x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.0 ms: 1.01x slower                                                        |
| pickle_dict                | 32.5 us                                                      | 32.8 us: 1.01x slower                                                        |
| pickle_list                | 4.43 us                                                      | 4.46 us: 1.01x slower                                                        |
| regex_compile              | 144 ms                                                       | 145 ms: 1.01x slower                                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.25 ms: 1.01x slower                                                        |
| dask                       | 392 ms                                                       | 396 ms: 1.01x slower                                                         |
| deepcopy                   | 368 us                                                       | 373 us: 1.01x slower                                                         |
| sympy_expand               | 484 ms                                                       | 490 ms: 1.01x slower                                                         |
| unpickle_list              | 4.66 us                                                      | 4.71 us: 1.01x slower                                                        |
| async_tree_none_tg         | 431 ms                                                       | 436 ms: 1.01x slower                                                         |
| mako                       | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                        |
| chameleon                  | 7.23 ms                                                      | 7.34 ms: 1.02x slower                                                        |
| unpickle_pure_python       | 210 us                                                       | 213 us: 1.02x slower                                                         |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| json                       | 5.12 ms                                                      | 5.22 ms: 1.02x slower                                                        |
| sqlglot_optimize           | 57.5 ms                                                      | 58.6 ms: 1.02x slower                                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.82 ms: 1.02x slower                                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.03x slower                                                         |
| 2to3                       | 285 ms                                                       | 293 ms: 1.03x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.41 ms: 1.03x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 97.0 ns: 1.03x slower                                                        |
| deepcopy_memo              | 36.8 us                                                      | 37.8 us: 1.03x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.23 sec: 1.03x slower                                                       |
| scimark_lu                 | 98.8 ms                                                      | 102 ms: 1.03x slower                                                         |
| dulwich_log                | 65.4 ms                                                      | 67.7 ms: 1.04x slower                                                        |
| float                      | 76.6 ms                                                      | 79.4 ms: 1.04x slower                                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| xml_etree_iterparse        | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| scimark_fft                | 301 ms                                                       | 314 ms: 1.04x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 564 ms: 1.04x slower                                                         |
| json_loads                 | 24.4 us                                                      | 25.5 us: 1.05x slower                                                        |
| regex_v8                   | 23.6 ms                                                      | 24.8 ms: 1.05x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.07x slower                                                       |
| gc_traversal               | 3.48 ms                                                      | 3.75 ms: 1.08x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 6.47 ms: 1.09x slower                                                        |
| python_startup             | 11.6 ms                                                      | 12.8 ms: 1.10x slower                                                        |
| fannkuch                   | 350 ms                                                       | 390 ms: 1.11x slower                                                         |
| go                         | 150 ms                                                       | 167 ms: 1.11x slower                                                         |
| deltablue                  | 3.24 ms                                                      | 3.64 ms: 1.13x slower                                                        |
| pyflate                    | 439 ms                                                       | 505 ms: 1.15x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.06 ms: 1.16x slower                                                        |
| richards_super             | 51.3 ms                                                      | 60.4 ms: 1.18x slower                                                        |
| richards                   | 45.7 ms                                                      | 53.9 ms: 1.18x slower                                                        |
| coverage                   | 66.7 ms                                                      | 80.6 ms: 1.21x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.2 ms: 1.30x slower                                                        |
| scimark_sor                | 109 ms                                                       | 149 ms: 1.36x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (10): bench_mp_pool, bench_thread_pool, logging_simple, asyncio_websockets, create_gc_cycles, xml_etree_process, async_tree_memoization, logging_format, async_tree_cpu_io_mixed, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 94.60% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.86x