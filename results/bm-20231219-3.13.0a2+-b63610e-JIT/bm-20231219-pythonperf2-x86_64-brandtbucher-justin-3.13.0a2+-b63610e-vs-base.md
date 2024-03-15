# Results vs. base

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 292 ms                                                                       | 302 ms: 1.04x slower                                                 |
| chameleon      | 7.48 ms                                                                      | 7.78 ms: 1.04x slower                                                |
| docutils       | 2.84 sec                                                                     | 2.88 sec: 1.01x slower                                               |
| tornado_http   | 119 ms                                                                       | 121 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.03x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 696 ms                                                                       | 711 ms: 1.02x slower                                                 |
| async_tree_io              | 1.07 sec                                                                     | 1.10 sec: 1.02x slower                                               |
| async_tree_io_tg           | 1.06 sec                                                                     | 1.09 sec: 1.03x slower                                               |
| async_tree_memoization     | 543 ms                                                                       | 559 ms: 1.03x slower                                                 |
| async_tree_cpu_io_mixed_tg | 698 ms                                                                       | 718 ms: 1.03x slower                                                 |
| async_tree_none            | 430 ms                                                                       | 447 ms: 1.04x slower                                                 |
| async_tree_none_tg         | 425 ms                                                                       | 446 ms: 1.05x slower                                                 |
| async_tree_memoization_tg  | 543 ms                                                                       | 570 ms: 1.05x slower                                                 |
| Geometric mean             | (ref)                                                                        | 1.03x slower                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 263 ms                                                                       | 263 ms: 1.00x faster                                                 |
| float          | 78.0 ms                                                                      | 82.2 ms: 1.05x slower                                                |
| nbody          | 86.7 ms                                                                      | 108 ms: 1.24x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.09x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_v8       | 26.8 ms                                                                      | 25.3 ms: 1.06x faster                                                |
| regex_dna      | 247 ms                                                                       | 244 ms: 1.01x faster                                                 |
| regex_effbot   | 3.53 ms                                                                      | 3.60 ms: 1.02x slower                                                |
| regex_compile  | 141 ms                                                                       | 150 ms: 1.06x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_list          | 4.45 us                                                                      | 4.23 us: 1.05x faster                                                |
| pickle               | 10.1 us                                                                      | 9.88 us: 1.03x faster                                                |
| pickle_dict          | 33.0 us                                                                      | 32.4 us: 1.02x faster                                                |
| xml_etree_parse      | 149 ms                                                                       | 148 ms: 1.01x faster                                                 |
| json_loads           | 24.6 us                                                                      | 24.5 us: 1.00x faster                                                |
| tomli_loads          | 2.35 sec                                                                     | 2.36 sec: 1.01x slower                                               |
| xml_etree_iterparse  | 106 ms                                                                       | 107 ms: 1.01x slower                                                 |
| unpickle_list        | 4.67 us                                                                      | 4.71 us: 1.01x slower                                                |
| unpickle             | 14.6 us                                                                      | 14.8 us: 1.01x slower                                                |
| xml_etree_process    | 58.2 ms                                                                      | 59.5 ms: 1.02x slower                                                |
| pickle_pure_python   | 305 us                                                                       | 313 us: 1.03x slower                                                 |
| xml_etree_generate   | 85.1 ms                                                                      | 88.0 ms: 1.03x slower                                                |
| unpickle_pure_python | 212 us                                                                       | 221 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                                        | 1.00x slower                                                         |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 12.5 ms                                                                      | 12.6 ms: 1.01x slower                                                |
| python_startup_no_site | 11.0 ms                                                                      | 11.1 ms: 1.02x slower                                                |
| Geometric mean         | (ref)                                                                        | 1.01x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.3 ms                                                                      | 12.0 ms: 1.16x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-pythonperf2-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_v8                   | 26.8 ms                                                                      | 25.3 ms: 1.06x faster                                                |
| unpack_sequence            | 46.4 ns                                                                      | 44.0 ns: 1.05x faster                                                |
| richards                   | 54.4 ms                                                                      | 51.7 ms: 1.05x faster                                                |
| pickle_list                | 4.45 us                                                                      | 4.23 us: 1.05x faster                                                |
| richards_super             | 60.6 ms                                                                      | 57.8 ms: 1.05x faster                                                |
| create_gc_cycles           | 1.61 ms                                                                      | 1.56 ms: 1.03x faster                                                |
| pickle                     | 10.1 us                                                                      | 9.88 us: 1.03x faster                                                |
| pycparser                  | 1.32 sec                                                                     | 1.28 sec: 1.03x faster                                               |
| pickle_dict                | 33.0 us                                                                      | 32.4 us: 1.02x faster                                                |
| asyncio_websockets         | 391 ms                                                                       | 385 ms: 1.02x faster                                                 |
| regex_dna                  | 247 ms                                                                       | 244 ms: 1.01x faster                                                 |
| xml_etree_parse            | 149 ms                                                                       | 148 ms: 1.01x faster                                                 |
| deepcopy_memo              | 37.5 us                                                                      | 37.4 us: 1.00x faster                                                |
| json_loads                 | 24.6 us                                                                      | 24.5 us: 1.00x faster                                                |
| pidigits                   | 263 ms                                                                       | 263 ms: 1.00x faster                                                 |
| asyncio_tcp_ssl            | 1.57 sec                                                                     | 1.58 sec: 1.00x slower                                               |
| tomli_loads                | 2.35 sec                                                                     | 2.36 sec: 1.01x slower                                               |
| coroutines                 | 22.4 ms                                                                      | 22.5 ms: 1.01x slower                                                |
| dulwich_log                | 67.6 ms                                                                      | 68.2 ms: 1.01x slower                                                |
| xml_etree_iterparse        | 106 ms                                                                       | 107 ms: 1.01x slower                                                 |
| unpickle_list              | 4.67 us                                                                      | 4.71 us: 1.01x slower                                                |
| python_startup             | 12.5 ms                                                                      | 12.6 ms: 1.01x slower                                                |
| logging_format             | 7.16 us                                                                      | 7.24 us: 1.01x slower                                                |
| logging_simple             | 6.53 us                                                                      | 6.61 us: 1.01x slower                                                |
| unpickle                   | 14.6 us                                                                      | 14.8 us: 1.01x slower                                                |
| docutils                   | 2.84 sec                                                                     | 2.88 sec: 1.01x slower                                               |
| python_startup_no_site     | 11.0 ms                                                                      | 11.1 ms: 1.02x slower                                                |
| pathlib                    | 18.8 ms                                                                      | 19.2 ms: 1.02x slower                                                |
| regex_effbot               | 3.53 ms                                                                      | 3.60 ms: 1.02x slower                                                |
| sqlglot_parse              | 1.38 ms                                                                      | 1.41 ms: 1.02x slower                                                |
| tornado_http               | 119 ms                                                                       | 121 ms: 1.02x slower                                                 |
| deepcopy                   | 364 us                                                                       | 371 us: 1.02x slower                                                 |
| deepcopy_reduce            | 3.30 us                                                                      | 3.37 us: 1.02x slower                                                |
| async_tree_cpu_io_mixed    | 696 ms                                                                       | 711 ms: 1.02x slower                                                 |
| sympy_expand               | 498 ms                                                                       | 509 ms: 1.02x slower                                                 |
| xml_etree_process          | 58.2 ms                                                                      | 59.5 ms: 1.02x slower                                                |
| pyflate                    | 505 ms                                                                       | 517 ms: 1.02x slower                                                 |
| async_tree_io              | 1.07 sec                                                                     | 1.10 sec: 1.02x slower                                               |
| sqlglot_transpile          | 1.78 ms                                                                      | 1.82 ms: 1.03x slower                                                |
| meteor_contest             | 129 ms                                                                       | 133 ms: 1.03x slower                                                 |
| pickle_pure_python         | 305 us                                                                       | 313 us: 1.03x slower                                                 |
| telco                      | 8.04 ms                                                                      | 8.25 ms: 1.03x slower                                                |
| go                         | 169 ms                                                                       | 174 ms: 1.03x slower                                                 |
| async_tree_io_tg           | 1.06 sec                                                                     | 1.09 sec: 1.03x slower                                               |
| coverage                   | 80.8 ms                                                                      | 83.1 ms: 1.03x slower                                                |
| async_tree_memoization     | 543 ms                                                                       | 559 ms: 1.03x slower                                                 |
| dask                       | 395 ms                                                                       | 406 ms: 1.03x slower                                                 |
| async_tree_cpu_io_mixed_tg | 698 ms                                                                       | 718 ms: 1.03x slower                                                 |
| xml_etree_generate         | 85.1 ms                                                                      | 88.0 ms: 1.03x slower                                                |
| typing_runtime_protocols   | 116 us                                                                       | 120 us: 1.04x slower                                                 |
| async_generators           | 366 ms                                                                       | 380 ms: 1.04x slower                                                 |
| sqlglot_normalize          | 116 ms                                                                       | 120 ms: 1.04x slower                                                 |
| 2to3                       | 292 ms                                                                       | 302 ms: 1.04x slower                                                 |
| generators                 | 33.6 ms                                                                      | 34.9 ms: 1.04x slower                                                |
| unpickle_pure_python       | 212 us                                                                       | 221 us: 1.04x slower                                                 |
| chameleon                  | 7.48 ms                                                                      | 7.78 ms: 1.04x slower                                                |
| async_tree_none            | 430 ms                                                                       | 447 ms: 1.04x slower                                                 |
| scimark_lu                 | 98.6 ms                                                                      | 103 ms: 1.04x slower                                                 |
| sympy_str                  | 292 ms                                                                       | 304 ms: 1.04x slower                                                 |
| sqlglot_optimize           | 59.2 ms                                                                      | 62.0 ms: 1.05x slower                                                |
| raytrace                   | 264 ms                                                                       | 277 ms: 1.05x slower                                                 |
| mdp                        | 2.49 sec                                                                     | 2.62 sec: 1.05x slower                                               |
| async_tree_none_tg         | 425 ms                                                                       | 446 ms: 1.05x slower                                                 |
| async_tree_memoization_tg  | 543 ms                                                                       | 570 ms: 1.05x slower                                                 |
| float                      | 78.0 ms                                                                      | 82.2 ms: 1.05x slower                                                |
| sympy_integrate            | 23.1 ms                                                                      | 24.4 ms: 1.06x slower                                                |
| sympy_sum                  | 152 ms                                                                       | 161 ms: 1.06x slower                                                 |
| pprint_safe_repr           | 812 ms                                                                       | 861 ms: 1.06x slower                                                 |
| regex_compile              | 141 ms                                                                       | 150 ms: 1.06x slower                                                 |
| pprint_pformat             | 1.66 sec                                                                     | 1.77 sec: 1.07x slower                                               |
| bench_mp_pool              | 4.58 ms                                                                      | 4.90 ms: 1.07x slower                                                |
| fannkuch                   | 387 ms                                                                       | 439 ms: 1.13x slower                                                 |
| deltablue                  | 3.55 ms                                                                      | 4.06 ms: 1.15x slower                                                |
| nqueens                    | 88.9 ms                                                                      | 102 ms: 1.15x slower                                                 |
| gc_traversal               | 3.56 ms                                                                      | 4.10 ms: 1.15x slower                                                |
| mako                       | 10.3 ms                                                                      | 12.0 ms: 1.16x slower                                                |
| chaos                      | 61.0 ms                                                                      | 71.2 ms: 1.17x slower                                                |
| crypto_pyaes               | 71.1 ms                                                                      | 83.6 ms: 1.18x slower                                                |
| scimark_monte_carlo        | 66.4 ms                                                                      | 79.1 ms: 1.19x slower                                                |
| scimark_sparse_mat_mult    | 4.13 ms                                                                      | 5.11 ms: 1.24x slower                                                |
| nbody                      | 86.7 ms                                                                      | 108 ms: 1.24x slower                                                 |
| scimark_fft                | 297 ms                                                                       | 371 ms: 1.25x slower                                                 |
| hexiom                     | 6.37 ms                                                                      | 7.96 ms: 1.25x slower                                                |
| comprehensions             | 16.4 us                                                                      | 21.0 us: 1.28x slower                                                |
| spectral_norm              | 92.6 ms                                                                      | 121 ms: 1.31x slower                                                 |
| Geometric mean             | (ref)                                                                        | 1.04x slower                                                         |

Benchmark hidden because not significant (8): json, asyncio_tcp, json_dumps, scimark_sor, bench_thread_pool, sqlite_synth, logging_silent, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.04x