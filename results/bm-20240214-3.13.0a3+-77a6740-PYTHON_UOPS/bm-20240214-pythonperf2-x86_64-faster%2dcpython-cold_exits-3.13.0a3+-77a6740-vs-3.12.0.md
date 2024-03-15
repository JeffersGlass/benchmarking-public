
# Results vs. 3.12.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 77a6740
- commit date: 2024-02-14
- overall geometric mean: 1.13x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 0.89x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 319 ms: 1.12x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.97 ms: 1.10x slower                                                        |
| docutils       | 2.87 sec                                                     | 3.06 sec: 1.07x slower                                                       |
| tornado_http   | 121 ms                                                       | 126 ms: 1.04x slower                                                         |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 717 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 563 ms: 1.04x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 561 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.06x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 266 ms: 1.00x slower                                                         |
| float          | 76.6 ms                                                      | 102 ms: 1.33x slower                                                         |
| nbody          | 88.0 ms                                                      | 123 ms: 1.40x slower                                                         |
| Geometric mean | (ref)                                                        | 1.23x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 235 ms: 1.02x faster                                                         |
| regex_effbot   | 3.57 ms                                                      | 3.58 ms: 1.00x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 26.4 ms: 1.12x slower                                                        |
| regex_compile  | 144 ms                                                       | 192 ms: 1.33x slower                                                         |
| Geometric mean | (ref)                                                        | 1.10x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 314 us: 1.02x faster                                                         |
| unpickle_list        | 4.66 us                                                      | 4.74 us: 1.02x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.1 us: 1.03x slower                                                        |
| pickle_dict          | 32.5 us                                                      | 33.6 us: 1.03x slower                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 91.2 ms: 1.06x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 62.5 ms: 1.07x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 116 ms: 1.12x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.87 sec: 1.33x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 310 us: 1.48x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.08x slower                                                                 |

Benchmark hidden because not significant (3): unpickle, pickle, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.10x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.2 ms: 1.29x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.19x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 14.1 ms: 1.41x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a3+-77a6740 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 124 us: 1.22x faster                                                         |
| generators                 | 37.4 ms                                                      | 34.0 ms: 1.10x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                                        |
| async_generators           | 390 ms                                                       | 381 ms: 1.02x faster                                                         |
| regex_dna                  | 239 ms                                                       | 235 ms: 1.02x faster                                                         |
| pickle_pure_python         | 318 us                                                       | 314 us: 1.02x faster                                                         |
| asyncio_tcp                | 378 ms                                                       | 374 ms: 1.01x faster                                                         |
| regex_effbot               | 3.57 ms                                                      | 3.58 ms: 1.00x slower                                                        |
| pidigits                   | 265 ms                                                       | 266 ms: 1.00x slower                                                         |
| logging_format             | 7.48 us                                                      | 7.56 us: 1.01x slower                                                        |
| unpickle_list              | 4.66 us                                                      | 4.74 us: 1.02x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| gc_traversal               | 3.48 ms                                                      | 3.57 ms: 1.03x slower                                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.03x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.4 ms: 1.03x slower                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.85 us: 1.03x slower                                                        |
| mdp                        | 2.57 sec                                                     | 2.64 sec: 1.03x slower                                                       |
| json_loads                 | 24.4 us                                                      | 25.1 us: 1.03x slower                                                        |
| logging_simple             | 6.71 us                                                      | 6.91 us: 1.03x slower                                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 717 ms: 1.03x slower                                                         |
| pickle_dict                | 32.5 us                                                      | 33.6 us: 1.03x slower                                                        |
| deepcopy_reduce            | 3.37 us                                                      | 3.48 us: 1.03x slower                                                        |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 563 ms: 1.04x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 561 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                       |
| tornado_http               | 121 ms                                                       | 126 ms: 1.04x slower                                                         |
| json                       | 5.12 ms                                                      | 5.34 ms: 1.04x slower                                                        |
| dask                       | 392 ms                                                       | 411 ms: 1.05x slower                                                         |
| bench_thread_pool          | 950 us                                                       | 996 us: 1.05x slower                                                         |
| deepcopy                   | 368 us                                                       | 387 us: 1.05x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 25.3 ms: 1.06x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.06x slower                                                       |
| logging_silent             | 94.4 ns                                                      | 99.8 ns: 1.06x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 91.2 ms: 1.06x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                        |
| sympy_sum                  | 162 ms                                                       | 172 ms: 1.06x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 123 ms: 1.06x slower                                                         |
| docutils                   | 2.87 sec                                                     | 3.06 sec: 1.07x slower                                                       |
| xml_etree_process          | 58.4 ms                                                      | 62.5 ms: 1.07x slower                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 86.8 ms: 1.08x slower                                                        |
| meteor_contest             | 128 ms                                                       | 139 ms: 1.09x slower                                                         |
| sympy_str                  | 302 ms                                                       | 330 ms: 1.09x slower                                                         |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.10x slower                                                        |
| chameleon                  | 7.23 ms                                                      | 7.97 ms: 1.10x slower                                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.96 ms: 1.10x slower                                                        |
| mypy2                      | 830 ms                                                       | 920 ms: 1.11x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.53 ms: 1.11x slower                                                        |
| regex_v8                   | 23.6 ms                                                      | 26.4 ms: 1.12x slower                                                        |
| 2to3                       | 285 ms                                                       | 319 ms: 1.12x slower                                                         |
| comprehensions             | 21.9 us                                                      | 24.5 us: 1.12x slower                                                        |
| xml_etree_iterparse        | 103 ms                                                       | 116 ms: 1.12x slower                                                         |
| deepcopy_memo              | 36.8 us                                                      | 41.7 us: 1.13x slower                                                        |
| raytrace                   | 298 ms                                                       | 339 ms: 1.14x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 66.0 ms: 1.15x slower                                                        |
| sympy_expand               | 484 ms                                                       | 559 ms: 1.15x slower                                                         |
| pycparser                  | 1.23 sec                                                     | 1.43 sec: 1.16x slower                                                       |
| dulwich_log                | 65.4 ms                                                      | 76.0 ms: 1.16x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 952 ms: 1.18x slower                                                         |
| chaos                      | 64.0 ms                                                      | 75.5 ms: 1.18x slower                                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.96 sec: 1.18x slower                                                       |
| coverage                   | 66.7 ms                                                      | 80.0 ms: 1.20x slower                                                        |
| telco                      | 6.96 ms                                                      | 8.38 ms: 1.20x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 4.05 ms: 1.25x slower                                                        |
| unpack_sequence            | 53.2 ns                                                      | 66.9 ns: 1.26x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 114 ms: 1.27x slower                                                         |
| python_startup_no_site     | 8.64 ms                                                      | 11.2 ms: 1.29x slower                                                        |
| go                         | 150 ms                                                       | 197 ms: 1.32x slower                                                         |
| tomli_loads                | 2.16 sec                                                     | 2.87 sec: 1.33x slower                                                       |
| regex_compile              | 144 ms                                                       | 192 ms: 1.33x slower                                                         |
| float                      | 76.6 ms                                                      | 102 ms: 1.33x slower                                                         |
| richards_super             | 51.3 ms                                                      | 68.5 ms: 1.33x slower                                                        |
| richards                   | 45.7 ms                                                      | 62.0 ms: 1.35x slower                                                        |
| scimark_fft                | 301 ms                                                       | 420 ms: 1.40x slower                                                         |
| nbody                      | 88.0 ms                                                      | 123 ms: 1.40x slower                                                         |
| mako                       | 10.0 ms                                                      | 14.1 ms: 1.41x slower                                                        |
| scimark_lu                 | 98.8 ms                                                      | 140 ms: 1.42x slower                                                         |
| fannkuch                   | 350 ms                                                       | 512 ms: 1.46x slower                                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.22 ms: 1.48x slower                                                        |
| unpickle_pure_python       | 210 us                                                       | 310 us: 1.48x slower                                                         |
| scimark_sor                | 109 ms                                                       | 163 ms: 1.49x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 104 ms: 1.51x slower                                                         |
| pyflate                    | 439 ms                                                       | 676 ms: 1.54x slower                                                         |
| spectral_norm              | 91.6 ms                                                      | 149 ms: 1.63x slower                                                         |
| hexiom                     | 5.96 ms                                                      | 10.5 ms: 1.76x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.13x slower                                                                 |

Benchmark hidden because not significant (8): bench_mp_pool, async_tree_none, asyncio_websockets, unpickle, asyncio_tcp_ssl, pickle, pickle_list, create_gc_cycles
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 0.89x