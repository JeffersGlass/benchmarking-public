# Results vs. 3.11.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: linux-x86_64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster \*
- HPT reliability: 71.38%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 310 ms: 1.08x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.45 ms: 1.06x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.96 sec: 1.04x slower                                                       |
| tornado_http   | 124 ms                                                       | 127 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 444 ms: 1.16x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 560 ms: 1.12x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 563 ms: 1.07x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 715 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 712 ms: 1.05x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                       |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                         |
| float          | 74.9 ms                                                      | 78.8 ms: 1.05x slower                                                        |
| nbody          | 92.9 ms                                                      | 102 ms: 1.10x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 154 ms: 1.01x faster                                                         |
| regex_v8       | 24.4 ms                                                      | 25.3 ms: 1.04x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                        |
| regex_dna      | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.4 ms: 1.27x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.0 us: 1.16x faster                                                        |
| pickle_dict          | 32.3 us                                                      | 30.4 us: 1.06x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 151 ms: 1.02x faster                                                         |
| xml_etree_iterparse  | 107 ms                                                       | 106 ms: 1.01x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 319 us: 1.01x slower                                                         |
| unpickle_pure_python | 238 us                                                       | 243 us: 1.02x slower                                                         |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.39 sec: 1.06x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 59.5 ms: 1.06x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 86.8 ms: 1.09x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.51 us: 1.15x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 15.7 ms: 1.46x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 14.1 ms: 1.83x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.64x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.7 ms: 1.02x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 120 us: 4.43x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 378 ms: 1.98x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 33.4 ms: 1.64x faster                                                        |
| comprehensions             | 25.1 us                                                      | 19.2 us: 1.30x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.4 ms: 1.27x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                        |
| async_tree_none            | 518 ms                                                       | 444 ms: 1.16x faster                                                         |
| json_loads                 | 28.9 us                                                      | 25.0 us: 1.16x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 163 ms: 1.14x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 560 ms: 1.12x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.58 us: 1.10x faster                                                        |
| sympy_str                  | 337 ms                                                       | 306 ms: 1.10x faster                                                         |
| richards_super             | 63.6 ms                                                      | 58.6 ms: 1.09x faster                                                        |
| chaos                      | 74.9 ms                                                      | 69.2 ms: 1.08x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.15 us: 1.08x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 444 ms: 1.07x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 563 ms: 1.07x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.89 ms: 1.07x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 30.4 us: 1.06x faster                                                        |
| chameleon                  | 7.92 ms                                                      | 7.45 ms: 1.06x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.06x faster                                                       |
| mdp                        | 2.77 sec                                                     | 2.61 sec: 1.06x faster                                                       |
| sympy_expand               | 553 ms                                                       | 523 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 715 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 712 ms: 1.05x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                       |
| json                       | 5.58 ms                                                      | 5.33 ms: 1.05x faster                                                        |
| deltablue                  | 3.97 ms                                                      | 3.80 ms: 1.05x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.45 ms: 1.04x faster                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 80.9 ms: 1.03x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 25.1 ms: 1.03x faster                                                        |
| mako                       | 11.0 ms                                                      | 10.7 ms: 1.02x faster                                                        |
| xml_etree_parse            | 155 ms                                                       | 151 ms: 1.02x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.88 ms: 1.02x faster                                                        |
| raytrace                   | 309 ms                                                       | 304 ms: 1.02x faster                                                         |
| regex_compile              | 156 ms                                                       | 154 ms: 1.01x faster                                                         |
| asyncio_websockets         | 390 ms                                                       | 385 ms: 1.01x faster                                                         |
| xml_etree_iterparse        | 107 ms                                                       | 106 ms: 1.01x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 120 ms: 1.01x faster                                                         |
| deepcopy                   | 391 us                                                       | 388 us: 1.01x faster                                                         |
| meteor_contest             | 131 ms                                                       | 132 ms: 1.01x slower                                                         |
| nqueens                    | 103 ms                                                       | 104 ms: 1.01x slower                                                         |
| pickle_pure_python         | 316 us                                                       | 319 us: 1.01x slower                                                         |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                                       |
| tornado_http               | 124 ms                                                       | 127 ms: 1.02x slower                                                         |
| unpickle_pure_python       | 238 us                                                       | 243 us: 1.02x slower                                                         |
| deepcopy_reduce            | 3.40 us                                                      | 3.48 us: 1.02x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.5 ms: 1.03x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 25.3 ms: 1.04x slower                                                        |
| docutils                   | 2.85 sec                                                     | 2.96 sec: 1.04x slower                                                       |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                         |
| spectral_norm              | 95.1 ms                                                      | 99.6 ms: 1.05x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                        |
| richards                   | 49.7 ms                                                      | 52.2 ms: 1.05x slower                                                        |
| regex_dna                  | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| float                      | 74.9 ms                                                      | 78.8 ms: 1.05x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 71.1 ms: 1.05x slower                                                        |
| fannkuch                   | 416 ms                                                       | 440 ms: 1.06x slower                                                         |
| scimark_lu                 | 114 ms                                                       | 121 ms: 1.06x slower                                                         |
| deepcopy_memo              | 37.5 us                                                      | 39.8 us: 1.06x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.39 sec: 1.06x slower                                                       |
| xml_etree_process          | 55.9 ms                                                      | 59.5 ms: 1.06x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.70 us: 1.07x slower                                                        |
| 2to3                       | 287 ms                                                       | 310 ms: 1.08x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 86.8 ms: 1.09x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 64.3 ms: 1.09x slower                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.45 ms: 1.10x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.83 sec: 1.10x slower                                                       |
| nbody                      | 92.9 ms                                                      | 102 ms: 1.10x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 886 ms: 1.10x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 7.69 ms: 1.10x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.6 us: 1.10x slower                                                        |
| go                         | 158 ms                                                       | 176 ms: 1.12x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.51 us: 1.15x slower                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 84.3 ms: 1.21x slower                                                        |
| async_generators           | 322 ms                                                       | 388 ms: 1.21x slower                                                         |
| pyflate                    | 449 ms                                                       | 544 ms: 1.21x slower                                                         |
| mypy2                      | 762 ms                                                       | 925 ms: 1.21x slower                                                         |
| scimark_fft                | 281 ms                                                       | 341 ms: 1.22x slower                                                         |
| telco                      | 6.81 ms                                                      | 8.32 ms: 1.22x slower                                                        |
| coverage                   | 66.1 ms                                                      | 84.7 ms: 1.28x slower                                                        |
| scimark_sor                | 110 ms                                                       | 156 ms: 1.42x slower                                                         |
| python_startup             | 10.7 ms                                                      | 15.7 ms: 1.46x slower                                                        |
| bench_mp_pool              | 4.70 ms                                                      | 6.93 ms: 1.47x slower                                                        |
| unpack_sequence            | 45.7 ns                                                      | 81.5 ns: 1.78x slower                                                        |
| python_startup_no_site     | 7.73 ms                                                      | 14.1 ms: 1.83x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (4): create_gc_cycles, logging_silent, bench_thread_pool, unpickle_list
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 71.38% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.25x