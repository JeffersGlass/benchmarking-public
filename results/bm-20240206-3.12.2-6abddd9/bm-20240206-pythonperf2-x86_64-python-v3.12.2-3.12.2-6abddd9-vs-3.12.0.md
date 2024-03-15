
# Results vs. 3.12.0

- fork: python
- ref: v3.12.2
- machine: linux-x86_64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.00x faster \*
- HPT reliability: 74.91%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 284 ms: 1.01x faster                                         |
| chameleon      | 7.23 ms                                                      | 7.35 ms: 1.02x slower                                        |
| docutils       | 2.87 sec                                                     | 2.85 sec: 1.01x faster                                       |
| tornado_http   | 121 ms                                                       | 119 ms: 1.02x faster                                         |
| Geometric mean | (ref)                                                        | 1.00x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_memoization     | 544 ms                                                       | 550 ms: 1.01x slower                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 705 ms: 1.01x slower                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 548 ms: 1.01x slower                                         |
| async_tree_none            | 452 ms                                                       | 458 ms: 1.01x slower                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.01x slower                                       |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                         |
| async_tree_io              | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                       |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                 |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 77.7 ms: 1.01x slower                                        |
| Geometric mean | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (2): nbody, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.43 ms: 1.04x faster                                        |
| regex_compile  | 144 ms                                                       | 140 ms: 1.03x faster                                         |
| regex_dna      | 239 ms                                                       | 236 ms: 1.01x faster                                         |
| regex_v8       | 23.6 ms                                                      | 23.7 ms: 1.00x slower                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                       | 203 us: 1.03x faster                                         |
| pickle               | 10.5 us                                                      | 10.3 us: 1.02x faster                                        |
| pickle_dict          | 32.5 us                                                      | 32.4 us: 1.00x faster                                        |
| unpickle             | 14.8 us                                                      | 14.9 us: 1.01x slower                                        |
| unpickle_list        | 4.66 us                                                      | 4.69 us: 1.01x slower                                        |
| tomli_loads          | 2.16 sec                                                     | 2.17 sec: 1.01x slower                                       |
| pickle_pure_python   | 318 us                                                       | 321 us: 1.01x slower                                         |
| xml_etree_process    | 58.4 ms                                                      | 58.9 ms: 1.01x slower                                        |
| json_dumps           | 10.2 ms                                                      | 10.4 ms: 1.01x slower                                        |
| pickle_list          | 4.43 us                                                      | 4.52 us: 1.02x slower                                        |
| xml_etree_parse      | 144 ms                                                       | 149 ms: 1.03x slower                                         |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (3): xml_etree_generate, json_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.50 ms: 1.02x faster                                        |
| python_startup         | 11.6 ms                                                      | 11.6 ms: 1.01x faster                                        |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 38.5 ms: 1.01x slower                                        |
| Geometric mean  | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 124 us: 1.23x faster                                         |
| mypy2                      | 830 ms                                                       | 723 ms: 1.15x faster                                         |
| regex_effbot               | 3.57 ms                                                      | 3.43 ms: 1.04x faster                                        |
| scimark_fft                | 301 ms                                                       | 290 ms: 1.04x faster                                         |
| comprehensions             | 21.9 us                                                      | 21.1 us: 1.04x faster                                        |
| richards                   | 45.7 ms                                                      | 44.3 ms: 1.03x faster                                        |
| fannkuch                   | 350 ms                                                       | 339 ms: 1.03x faster                                         |
| unpickle_pure_python       | 210 us                                                       | 203 us: 1.03x faster                                         |
| regex_compile              | 144 ms                                                       | 140 ms: 1.03x faster                                         |
| unpack_sequence            | 53.2 ns                                                      | 52.0 ns: 1.02x faster                                        |
| generators                 | 37.4 ms                                                      | 36.7 ms: 1.02x faster                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.12 ms: 1.02x faster                                        |
| tornado_http               | 121 ms                                                       | 119 ms: 1.02x faster                                         |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.02x faster                                        |
| meteor_contest             | 128 ms                                                       | 126 ms: 1.02x faster                                         |
| sqlite_synth               | 2.77 us                                                      | 2.73 us: 1.02x faster                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.56 sec: 1.02x faster                                       |
| python_startup_no_site     | 8.64 ms                                                      | 8.50 ms: 1.02x faster                                        |
| nqueens                    | 89.9 ms                                                      | 88.6 ms: 1.01x faster                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 68.0 ms: 1.01x faster                                        |
| chaos                      | 64.0 ms                                                      | 63.1 ms: 1.01x faster                                        |
| logging_format             | 7.48 us                                                      | 7.40 us: 1.01x faster                                        |
| sympy_integrate            | 23.9 ms                                                      | 23.7 ms: 1.01x faster                                        |
| regex_dna                  | 239 ms                                                       | 236 ms: 1.01x faster                                         |
| crypto_pyaes               | 80.3 ms                                                      | 79.5 ms: 1.01x faster                                        |
| richards_super             | 51.3 ms                                                      | 50.8 ms: 1.01x faster                                        |
| asyncio_tcp                | 378 ms                                                       | 374 ms: 1.01x faster                                         |
| sympy_sum                  | 162 ms                                                       | 161 ms: 1.01x faster                                         |
| dulwich_log                | 65.4 ms                                                      | 64.9 ms: 1.01x faster                                        |
| asyncio_websockets         | 387 ms                                                       | 385 ms: 1.01x faster                                         |
| docutils                   | 2.87 sec                                                     | 2.85 sec: 1.01x faster                                       |
| 2to3                       | 285 ms                                                       | 284 ms: 1.01x faster                                         |
| python_startup             | 11.6 ms                                                      | 11.6 ms: 1.01x faster                                        |
| pickle_dict                | 32.5 us                                                      | 32.4 us: 1.00x faster                                        |
| go                         | 150 ms                                                       | 149 ms: 1.00x faster                                         |
| mdp                        | 2.57 sec                                                     | 2.56 sec: 1.00x faster                                       |
| regex_v8                   | 23.6 ms                                                      | 23.7 ms: 1.00x slower                                        |
| aiohttp                    | 1.02 ms                                                      | 1.02 ms: 1.01x slower                                        |
| unpickle                   | 14.8 us                                                      | 14.9 us: 1.01x slower                                        |
| unpickle_list              | 4.66 us                                                      | 4.69 us: 1.01x slower                                        |
| deepcopy_reduce            | 3.37 us                                                      | 3.39 us: 1.01x slower                                        |
| tomli_loads                | 2.16 sec                                                     | 2.17 sec: 1.01x slower                                       |
| async_generators           | 390 ms                                                       | 393 ms: 1.01x slower                                         |
| deepcopy                   | 368 us                                                       | 371 us: 1.01x slower                                         |
| pickle_pure_python         | 318 us                                                       | 321 us: 1.01x slower                                         |
| scimark_sor                | 109 ms                                                       | 110 ms: 1.01x slower                                         |
| deepcopy_memo              | 36.8 us                                                      | 37.1 us: 1.01x slower                                        |
| sqlglot_optimize           | 57.5 ms                                                      | 58.0 ms: 1.01x slower                                        |
| xml_etree_process          | 58.4 ms                                                      | 58.9 ms: 1.01x slower                                        |
| django_template            | 38.2 ms                                                      | 38.5 ms: 1.01x slower                                        |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                        |
| async_tree_memoization     | 544 ms                                                       | 550 ms: 1.01x slower                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 705 ms: 1.01x slower                                         |
| json                       | 5.12 ms                                                      | 5.18 ms: 1.01x slower                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.80 ms: 1.01x slower                                        |
| spectral_norm              | 91.6 ms                                                      | 92.8 ms: 1.01x slower                                        |
| float                      | 76.6 ms                                                      | 77.7 ms: 1.01x slower                                        |
| async_tree_memoization_tg  | 540 ms                                                       | 548 ms: 1.01x slower                                         |
| json_dumps                 | 10.2 ms                                                      | 10.4 ms: 1.01x slower                                        |
| async_tree_none            | 452 ms                                                       | 458 ms: 1.01x slower                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.01x slower                                       |
| pprint_pformat             | 1.65 sec                                                     | 1.68 sec: 1.02x slower                                       |
| chameleon                  | 7.23 ms                                                      | 7.35 ms: 1.02x slower                                        |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                         |
| async_tree_io              | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                       |
| sqlglot_parse              | 1.38 ms                                                      | 1.40 ms: 1.02x slower                                        |
| hexiom                     | 5.96 ms                                                      | 6.07 ms: 1.02x slower                                        |
| pickle_list                | 4.43 us                                                      | 4.52 us: 1.02x slower                                        |
| pprint_safe_repr           | 807 ms                                                       | 827 ms: 1.02x slower                                         |
| sympy_expand               | 484 ms                                                       | 496 ms: 1.02x slower                                         |
| pycparser                  | 1.23 sec                                                     | 1.27 sec: 1.03x slower                                       |
| sqlglot_normalize          | 116 ms                                                       | 119 ms: 1.03x slower                                         |
| xml_etree_parse            | 144 ms                                                       | 149 ms: 1.03x slower                                         |
| telco                      | 6.96 ms                                                      | 7.27 ms: 1.04x slower                                        |
| pyflate                    | 439 ms                                                       | 461 ms: 1.05x slower                                         |
| logging_silent             | 94.4 ns                                                      | 100 ns: 1.06x slower                                         |
| gc_traversal               | 3.48 ms                                                      | 3.74 ms: 1.08x slower                                        |
| Geometric mean             | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (21): sqlalchemy_imperative, gunicorn, create_gc_cycles, coverage, nbody, mako, coroutines, dask, bench_thread_pool, raytrace, xml_etree_generate, logging_simple, pidigits, deltablue, sympy_str, json_loads, sqlalchemy_declarative, xml_etree_iterparse, scimark_lu, async_tree_cpu_io_mixed, bench_mp_pool


# HPT report

- Reliability score: 74.91% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.91x