
# Results vs. 3.12.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.01x slower
- HPT reliability: 95.13%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 292 ms: 1.02x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.48 ms: 1.03x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.84 sec: 1.01x faster                                                       |
| tornado_http   | 121 ms                                                       | 119 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none    | 452 ms                                                       | 430 ms: 1.05x faster                                                         |
| async_tree_none_tg | 431 ms                                                       | 425 ms: 1.01x faster                                                         |
| async_tree_io_tg   | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                                       |
| async_tree_io      | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| Geometric mean     | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 86.7 ms: 1.02x faster                                                        |
| pidigits       | 265 ms                                                       | 263 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 78.0 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 141 ms: 1.02x faster                                                         |
| regex_effbot   | 3.57 ms                                                      | 3.53 ms: 1.01x faster                                                        |
| regex_dna      | 239 ms                                                       | 247 ms: 1.04x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 26.8 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 305 us: 1.04x faster                                                         |
| pickle               | 10.5 us                                                      | 10.1 us: 1.04x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.6 us: 1.02x faster                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 85.1 ms: 1.01x faster                                                        |
| json_loads           | 24.4 us                                                      | 24.6 us: 1.01x slower                                                        |
| pickle_dict          | 32.5 us                                                      | 33.0 us: 1.01x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 212 us: 1.01x slower                                                         |
| xml_etree_iterparse  | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| xml_etree_parse      | 144 ms                                                       | 149 ms: 1.04x slower                                                         |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| tomli_loads          | 2.16 sec                                                     | 2.35 sec: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (3): xml_etree_process, unpickle_list, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.17x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| comprehensions           | 21.9 us                                                      | 16.4 us: 1.34x faster                                                        |
| typing_runtime_protocols | 152 us                                                       | 116 us: 1.31x faster                                                         |
| unpack_sequence          | 53.2 ns                                                      | 46.4 ns: 1.15x faster                                                        |
| raytrace                 | 298 ms                                                       | 264 ms: 1.13x faster                                                         |
| crypto_pyaes             | 80.3 ms                                                      | 71.1 ms: 1.13x faster                                                        |
| generators               | 37.4 ms                                                      | 33.6 ms: 1.11x faster                                                        |
| sympy_sum                | 162 ms                                                       | 152 ms: 1.07x faster                                                         |
| async_generators         | 390 ms                                                       | 366 ms: 1.07x faster                                                         |
| async_tree_none          | 452 ms                                                       | 430 ms: 1.05x faster                                                         |
| chaos                    | 64.0 ms                                                      | 61.0 ms: 1.05x faster                                                        |
| logging_format           | 7.48 us                                                      | 7.16 us: 1.05x faster                                                        |
| pickle_pure_python       | 318 us                                                       | 305 us: 1.04x faster                                                         |
| scimark_monte_carlo      | 69.0 ms                                                      | 66.4 ms: 1.04x faster                                                        |
| pickle                   | 10.5 us                                                      | 10.1 us: 1.04x faster                                                        |
| sympy_integrate          | 23.9 ms                                                      | 23.1 ms: 1.04x faster                                                        |
| sympy_str                | 302 ms                                                       | 292 ms: 1.04x faster                                                         |
| mdp                      | 2.57 sec                                                     | 2.49 sec: 1.03x faster                                                       |
| logging_simple           | 6.71 us                                                      | 6.53 us: 1.03x faster                                                        |
| coroutines               | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                        |
| asyncio_tcp              | 378 ms                                                       | 369 ms: 1.02x faster                                                         |
| sqlite_synth             | 2.77 us                                                      | 2.71 us: 1.02x faster                                                        |
| regex_compile            | 144 ms                                                       | 141 ms: 1.02x faster                                                         |
| tornado_http             | 121 ms                                                       | 119 ms: 1.02x faster                                                         |
| deepcopy_reduce          | 3.37 us                                                      | 3.30 us: 1.02x faster                                                        |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.13 ms: 1.02x faster                                                        |
| unpickle                 | 14.8 us                                                      | 14.6 us: 1.02x faster                                                        |
| nbody                    | 88.0 ms                                                      | 86.7 ms: 1.02x faster                                                        |
| async_tree_none_tg       | 431 ms                                                       | 425 ms: 1.01x faster                                                         |
| scimark_fft              | 301 ms                                                       | 297 ms: 1.01x faster                                                         |
| regex_effbot             | 3.57 ms                                                      | 3.53 ms: 1.01x faster                                                        |
| deepcopy                 | 368 us                                                       | 364 us: 1.01x faster                                                         |
| xml_etree_generate       | 86.1 ms                                                      | 85.1 ms: 1.01x faster                                                        |
| nqueens                  | 89.9 ms                                                      | 88.9 ms: 1.01x faster                                                        |
| docutils                 | 2.87 sec                                                     | 2.84 sec: 1.01x faster                                                       |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| pidigits                 | 265 ms                                                       | 263 ms: 1.01x faster                                                         |
| pprint_safe_repr         | 807 ms                                                       | 812 ms: 1.01x slower                                                         |
| meteor_contest           | 128 ms                                                       | 129 ms: 1.01x slower                                                         |
| json_loads               | 24.4 us                                                      | 24.6 us: 1.01x slower                                                        |
| spectral_norm            | 91.6 ms                                                      | 92.6 ms: 1.01x slower                                                        |
| asyncio_websockets       | 387 ms                                                       | 391 ms: 1.01x slower                                                         |
| async_tree_io_tg         | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                                       |
| pickle_dict              | 32.5 us                                                      | 33.0 us: 1.01x slower                                                        |
| create_gc_cycles         | 1.59 ms                                                      | 1.61 ms: 1.01x slower                                                        |
| unpickle_pure_python     | 210 us                                                       | 212 us: 1.01x slower                                                         |
| float                    | 76.6 ms                                                      | 78.0 ms: 1.02x slower                                                        |
| deepcopy_memo            | 36.8 us                                                      | 37.5 us: 1.02x slower                                                        |
| 2to3                     | 285 ms                                                       | 292 ms: 1.02x slower                                                         |
| gc_traversal             | 3.48 ms                                                      | 3.56 ms: 1.02x slower                                                        |
| async_tree_io            | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| json                     | 5.12 ms                                                      | 5.26 ms: 1.03x slower                                                        |
| sympy_expand             | 484 ms                                                       | 498 ms: 1.03x slower                                                         |
| sqlglot_optimize         | 57.5 ms                                                      | 59.2 ms: 1.03x slower                                                        |
| mako                     | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                        |
| dulwich_log              | 65.4 ms                                                      | 67.6 ms: 1.03x slower                                                        |
| chameleon                | 7.23 ms                                                      | 7.48 ms: 1.03x slower                                                        |
| xml_etree_iterparse      | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| regex_dna                | 239 ms                                                       | 247 ms: 1.04x slower                                                         |
| xml_etree_parse          | 144 ms                                                       | 149 ms: 1.04x slower                                                         |
| json_dumps               | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| logging_silent           | 94.4 ns                                                      | 98.4 ns: 1.04x slower                                                        |
| pycparser                | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                                       |
| hexiom                   | 5.96 ms                                                      | 6.37 ms: 1.07x slower                                                        |
| python_startup           | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| tomli_loads              | 2.16 sec                                                     | 2.35 sec: 1.09x slower                                                       |
| deltablue                | 3.24 ms                                                      | 3.55 ms: 1.10x slower                                                        |
| fannkuch                 | 350 ms                                                       | 387 ms: 1.11x slower                                                         |
| go                       | 150 ms                                                       | 169 ms: 1.13x slower                                                         |
| regex_v8                 | 23.6 ms                                                      | 26.8 ms: 1.13x slower                                                        |
| pyflate                  | 439 ms                                                       | 505 ms: 1.15x slower                                                         |
| telco                    | 6.96 ms                                                      | 8.04 ms: 1.15x slower                                                        |
| richards_super           | 51.3 ms                                                      | 60.6 ms: 1.18x slower                                                        |
| richards                 | 45.7 ms                                                      | 54.4 ms: 1.19x slower                                                        |
| coverage                 | 66.7 ms                                                      | 80.8 ms: 1.21x slower                                                        |
| python_startup_no_site   | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| scimark_sor              | 109 ms                                                       | 143 ms: 1.31x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (17): bench_mp_pool, xml_etree_process, pathlib, async_tree_memoization, scimark_lu, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, pprint_pformat, sqlglot_transpile, unpickle_list, sqlglot_parse, sqlglot_normalize, pickle_list, async_tree_memoization_tg, bench_thread_pool, dask, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 95.13% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.88x