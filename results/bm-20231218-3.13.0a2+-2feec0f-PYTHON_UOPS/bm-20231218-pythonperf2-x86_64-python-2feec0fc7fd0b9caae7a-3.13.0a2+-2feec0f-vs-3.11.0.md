
# Results vs. 3.11.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: linux-x86_64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.02x slower
- HPT reliability: 94.39%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 310 ms: 1.08x slower                                                         |
| chameleon      | 7.92 ms                                                      | 8.13 ms: 1.03x slower                                                        |
| docutils       | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 561 ms: 1.12x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 554 ms: 1.08x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 446 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 714 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 720 ms: 1.04x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 265 ms: 1.06x slower                                                         |
| nbody          | 92.9 ms                                                      | 128 ms: 1.38x slower                                                         |
| float          | 74.9 ms                                                      | 105 ms: 1.40x slower                                                         |
| Geometric mean | (ref)                                                        | 1.27x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 25.5 ms: 1.05x slower                                                        |
| regex_dna      | 227 ms                                                       | 246 ms: 1.08x slower                                                         |
| regex_compile  | 156 ms                                                       | 172 ms: 1.10x slower                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.80 ms: 1.14x slower                                                        |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.5 us: 1.18x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 229 us: 1.04x faster                                                         |
| xml_etree_parse      | 155 ms                                                       | 150 ms: 1.03x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 309 us: 1.02x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 31.6 us: 1.02x faster                                                        |
| unpickle_list        | 4.60 us                                                      | 4.66 us: 1.01x slower                                                        |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 118 ms: 1.10x slower                                                         |
| xml_etree_process    | 55.9 ms                                                      | 62.3 ms: 1.12x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.9 us: 1.12x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.44 us: 1.13x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 91.8 ms: 1.15x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.80 sec: 1.24x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 14.9 ms: 1.35x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf2-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 127 us: 4.20x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 374 ms: 2.00x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.4 ms: 1.59x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                        |
| json_loads                 | 28.9 us                                                      | 24.5 us: 1.18x faster                                                        |
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.69 ms: 1.12x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 561 ms: 1.12x faster                                                         |
| sympy_sum                  | 186 ms                                                       | 169 ms: 1.10x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 554 ms: 1.08x faster                                                         |
| json                       | 5.58 ms                                                      | 5.19 ms: 1.08x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 446 ms: 1.06x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 107 ms: 1.06x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.83 us: 1.06x faster                                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| richards_super             | 63.6 ms                                                      | 60.3 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 714 ms: 1.05x faster                                                         |
| unpack_sequence            | 45.7 ns                                                      | 43.5 ns: 1.05x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.44 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 720 ms: 1.04x faster                                                         |
| unpickle_pure_python       | 238 us                                                       | 229 us: 1.04x faster                                                         |
| mdp                        | 2.77 sec                                                     | 2.67 sec: 1.04x faster                                                       |
| sympy_str                  | 337 ms                                                       | 325 ms: 1.04x faster                                                         |
| bench_thread_pool          | 1.00 ms                                                      | 964 us: 1.04x faster                                                         |
| deepcopy                   | 391 us                                                       | 377 us: 1.04x faster                                                         |
| raytrace                   | 309 ms                                                       | 299 ms: 1.04x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 150 ms: 1.03x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.86 ms: 1.03x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.52 us: 1.03x faster                                                        |
| sympy_expand               | 553 ms                                                       | 540 ms: 1.02x faster                                                         |
| logging_silent             | 100 ns                                                       | 98.1 ns: 1.02x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 25.2 ms: 1.02x faster                                                        |
| pickle_pure_python         | 316 us                                                       | 309 us: 1.02x faster                                                         |
| pickle_dict                | 32.3 us                                                      | 31.6 us: 1.02x faster                                                        |
| comprehensions             | 25.1 us                                                      | 24.9 us: 1.01x faster                                                        |
| unpickle_list              | 4.60 us                                                      | 4.66 us: 1.01x slower                                                        |
| sqlglot_normalize          | 122 ms                                                       | 123 ms: 1.01x slower                                                         |
| chaos                      | 74.9 ms                                                      | 76.2 ms: 1.02x slower                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 85.1 ms: 1.02x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| chameleon                  | 7.92 ms                                                      | 8.13 ms: 1.03x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.5 ms: 1.03x slower                                                        |
| pycparser                  | 1.31 sec                                                     | 1.36 sec: 1.04x slower                                                       |
| docutils                   | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                       |
| regex_v8                   | 24.4 ms                                                      | 25.5 ms: 1.05x slower                                                        |
| deepcopy_memo              | 37.5 us                                                      | 39.6 us: 1.06x slower                                                        |
| pidigits                   | 251 ms                                                       | 265 ms: 1.06x slower                                                         |
| meteor_contest             | 131 ms                                                       | 139 ms: 1.07x slower                                                         |
| nqueens                    | 103 ms                                                       | 110 ms: 1.07x slower                                                         |
| dulwich_log                | 67.4 ms                                                      | 72.5 ms: 1.08x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 63.6 ms: 1.08x slower                                                        |
| regex_dna                  | 227 ms                                                       | 246 ms: 1.08x slower                                                         |
| 2to3                       | 287 ms                                                       | 310 ms: 1.08x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.76 us: 1.09x slower                                                        |
| regex_compile              | 156 ms                                                       | 172 ms: 1.10x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                       | 118 ms: 1.10x slower                                                         |
| richards                   | 49.7 ms                                                      | 54.8 ms: 1.10x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 62.3 ms: 1.12x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.9 us: 1.12x slower                                                        |
| fannkuch                   | 416 ms                                                       | 468 ms: 1.12x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.44 us: 1.13x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.88 sec: 1.13x slower                                                       |
| pprint_safe_repr           | 805 ms                                                       | 911 ms: 1.13x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.80 ms: 1.14x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 91.8 ms: 1.15x slower                                                        |
| go                         | 158 ms                                                       | 183 ms: 1.16x slower                                                         |
| mypy2                      | 762 ms                                                       | 894 ms: 1.17x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                        |
| async_generators           | 322 ms                                                       | 380 ms: 1.18x slower                                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 86.8 ms: 1.24x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.80 sec: 1.24x slower                                                       |
| telco                      | 6.81 ms                                                      | 8.48 ms: 1.25x slower                                                        |
| pyflate                    | 449 ms                                                       | 572 ms: 1.27x slower                                                         |
| coverage                   | 66.1 ms                                                      | 84.5 ms: 1.28x slower                                                        |
| scimark_sor                | 110 ms                                                       | 142 ms: 1.30x slower                                                         |
| mako                       | 11.0 ms                                                      | 14.9 ms: 1.35x slower                                                        |
| nbody                      | 92.9 ms                                                      | 128 ms: 1.38x slower                                                         |
| deltablue                  | 3.97 ms                                                      | 5.49 ms: 1.38x slower                                                        |
| float                      | 74.9 ms                                                      | 105 ms: 1.40x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 9.75 ms: 1.40x slower                                                        |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                        |
| scimark_fft                | 281 ms                                                       | 429 ms: 1.53x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.68 ms: 1.64x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 161 ms: 1.70x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (5): asyncio_websockets, bench_mp_pool, dask, tornado_http, deepcopy_reduce
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.39% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x