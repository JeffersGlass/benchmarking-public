
# Results vs. 3.12.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 310 ms: 1.09x slower                                                         |
| chameleon      | 7.23 ms                                                      | 8.13 ms: 1.12x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                       |
| tornado_http   | 121 ms                                                       | 124 ms: 1.03x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 540 ms                                                       | 554 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 714 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 561 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 720 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 446 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 105 ms: 1.37x slower                                                         |
| nbody          | 88.0 ms                                                      | 128 ms: 1.46x slower                                                         |
| Geometric mean | (ref)                                                        | 1.26x slower                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 246 ms: 1.03x slower                                                         |
| regex_effbot   | 3.57 ms                                                      | 3.80 ms: 1.06x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 25.5 ms: 1.08x slower                                                        |
| regex_compile  | 144 ms                                                       | 172 ms: 1.19x slower                                                         |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 10.1 us: 1.04x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 309 us: 1.03x faster                                                         |
| pickle_dict          | 32.5 us                                                      | 31.6 us: 1.03x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.9 us: 1.01x slower                                                        |
| json_loads           | 24.4 us                                                      | 24.5 us: 1.01x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 150 ms: 1.04x slower                                                         |
| xml_etree_generate   | 86.1 ms                                                      | 91.8 ms: 1.07x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 62.3 ms: 1.07x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 229 us: 1.09x slower                                                         |
| xml_etree_iterparse  | 103 ms                                                       | 118 ms: 1.14x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.80 sec: 1.30x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                 |

Benchmark hidden because not significant (2): unpickle_list, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpack_sequence            | 53.2 ns                                                      | 43.5 ns: 1.22x faster                                                        |
| typing_runtime_protocols   | 152 us                                                       | 127 us: 1.20x faster                                                         |
| generators                 | 37.4 ms                                                      | 34.4 ms: 1.09x faster                                                        |
| pickle                     | 10.5 us                                                      | 10.1 us: 1.04x faster                                                        |
| pickle_pure_python         | 318 us                                                       | 309 us: 1.03x faster                                                         |
| pickle_dict                | 32.5 us                                                      | 31.6 us: 1.03x faster                                                        |
| async_generators           | 390 ms                                                       | 380 ms: 1.03x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                        |
| asyncio_tcp                | 378 ms                                                       | 374 ms: 1.01x faster                                                         |
| sqlite_synth               | 2.77 us                                                      | 2.76 us: 1.01x faster                                                        |
| unpickle                   | 14.8 us                                                      | 14.9 us: 1.01x slower                                                        |
| json_loads                 | 24.4 us                                                      | 24.5 us: 1.01x slower                                                        |
| deepcopy_reduce            | 3.37 us                                                      | 3.40 us: 1.01x slower                                                        |
| json                       | 5.12 ms                                                      | 5.19 ms: 1.01x slower                                                        |
| logging_simple             | 6.71 us                                                      | 6.83 us: 1.02x slower                                                        |
| deepcopy                   | 368 us                                                       | 377 us: 1.02x slower                                                         |
| tornado_http               | 121 ms                                                       | 124 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 554 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 714 ms: 1.03x slower                                                         |
| docutils                   | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                       |
| regex_dna                  | 239 ms                                                       | 246 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 561 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 720 ms: 1.03x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.5 ms: 1.03x slower                                                        |
| async_tree_none_tg         | 431 ms                                                       | 446 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| mdp                        | 2.57 sec                                                     | 2.67 sec: 1.04x slower                                                       |
| logging_silent             | 94.4 ns                                                      | 98.1 ns: 1.04x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 150 ms: 1.04x slower                                                         |
| sympy_sum                  | 162 ms                                                       | 169 ms: 1.04x slower                                                         |
| dask                       | 392 ms                                                       | 409 ms: 1.04x slower                                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.86 ms: 1.05x slower                                                        |
| sqlglot_parse              | 1.38 ms                                                      | 1.44 ms: 1.05x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                       |
| sympy_integrate            | 23.9 ms                                                      | 25.2 ms: 1.05x slower                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 85.1 ms: 1.06x slower                                                        |
| gc_traversal               | 3.48 ms                                                      | 3.69 ms: 1.06x slower                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.80 ms: 1.06x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 91.8 ms: 1.07x slower                                                        |
| xml_etree_process          | 58.4 ms                                                      | 62.3 ms: 1.07x slower                                                        |
| sqlglot_normalize          | 116 ms                                                       | 123 ms: 1.07x slower                                                         |
| sympy_str                  | 302 ms                                                       | 325 ms: 1.07x slower                                                         |
| deepcopy_memo              | 36.8 us                                                      | 39.6 us: 1.08x slower                                                        |
| mypy2                      | 830 ms                                                       | 894 ms: 1.08x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 25.5 ms: 1.08x slower                                                        |
| meteor_contest             | 128 ms                                                       | 139 ms: 1.09x slower                                                         |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| 2to3                       | 285 ms                                                       | 310 ms: 1.09x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 107 ms: 1.09x slower                                                         |
| unpickle_pure_python       | 210 us                                                       | 229 us: 1.09x slower                                                         |
| pycparser                  | 1.23 sec                                                     | 1.36 sec: 1.10x slower                                                       |
| sqlglot_optimize           | 57.5 ms                                                      | 63.6 ms: 1.11x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 72.5 ms: 1.11x slower                                                        |
| sympy_expand               | 484 ms                                                       | 540 ms: 1.11x slower                                                         |
| chameleon                  | 7.23 ms                                                      | 8.13 ms: 1.12x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 911 ms: 1.13x slower                                                         |
| comprehensions             | 21.9 us                                                      | 24.9 us: 1.14x slower                                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.88 sec: 1.14x slower                                                       |
| xml_etree_iterparse        | 103 ms                                                       | 118 ms: 1.14x slower                                                         |
| richards_super             | 51.3 ms                                                      | 60.3 ms: 1.17x slower                                                        |
| chaos                      | 64.0 ms                                                      | 76.2 ms: 1.19x slower                                                        |
| regex_compile              | 144 ms                                                       | 172 ms: 1.19x slower                                                         |
| richards                   | 45.7 ms                                                      | 54.8 ms: 1.20x slower                                                        |
| telco                      | 6.96 ms                                                      | 8.48 ms: 1.22x slower                                                        |
| go                         | 150 ms                                                       | 183 ms: 1.22x slower                                                         |
| nqueens                    | 89.9 ms                                                      | 110 ms: 1.22x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 86.8 ms: 1.26x slower                                                        |
| coverage                   | 66.7 ms                                                      | 84.5 ms: 1.27x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.80 sec: 1.30x slower                                                       |
| pyflate                    | 439 ms                                                       | 572 ms: 1.30x slower                                                         |
| scimark_sor                | 109 ms                                                       | 142 ms: 1.31x slower                                                         |
| fannkuch                   | 350 ms                                                       | 468 ms: 1.34x slower                                                         |
| float                      | 76.6 ms                                                      | 105 ms: 1.37x slower                                                         |
| scimark_fft                | 301 ms                                                       | 429 ms: 1.42x slower                                                         |
| nbody                      | 88.0 ms                                                      | 128 ms: 1.46x slower                                                         |
| mako                       | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.68 ms: 1.59x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 9.75 ms: 1.64x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 5.49 ms: 1.70x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 161 ms: 1.76x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.10x slower                                                                 |

Benchmark hidden because not significant (11): bench_mp_pool, async_tree_none, unpickle_list, asyncio_websockets, asyncio_tcp_ssl, pidigits, raytrace, pickle_list, logging_format, create_gc_cycles, bench_thread_pool
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x