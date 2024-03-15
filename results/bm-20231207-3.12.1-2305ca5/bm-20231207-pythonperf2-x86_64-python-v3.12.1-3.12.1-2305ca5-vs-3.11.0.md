
# Results vs. 3.11.0

- fork: python
- ref: v3.12.1
- machine: linux-x86_64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 281 ms: 1.02x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.31 ms: 1.08x faster                                        |
| docutils       | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                       |
| tornado_http   | 124 ms                                                       | 118 ms: 1.05x faster                                         |
| Geometric mean | (ref)                                                        | 1.04x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                         |
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                         |
| async_tree_io              | 1.17 sec                                                     | 1.04 sec: 1.12x faster                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 540 ms: 1.11x faster                                         |
| async_tree_none_tg         | 474 ms                                                       | 430 ms: 1.10x faster                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.05 sec: 1.10x faster                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 693 ms: 1.09x faster                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 695 ms: 1.08x faster                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 85.5 ms: 1.09x faster                                        |
| float          | 74.9 ms                                                      | 77.0 ms: 1.03x slower                                        |
| pidigits       | 251 ms                                                       | 265 ms: 1.05x slower                                         |
| Geometric mean | (ref)                                                        | 1.00x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 138 ms: 1.13x faster                                         |
| regex_v8       | 24.4 ms                                                      | 23.5 ms: 1.04x faster                                        |
| regex_effbot   | 3.34 ms                                                      | 3.54 ms: 1.06x slower                                        |
| regex_dna      | 227 ms                                                       | 244 ms: 1.07x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                        |
| json_loads           | 28.9 us                                                      | 24.6 us: 1.17x faster                                        |
| unpickle_pure_python | 238 us                                                       | 205 us: 1.16x faster                                         |
| xml_etree_parse      | 155 ms                                                       | 145 ms: 1.06x faster                                         |
| tomli_loads          | 2.25 sec                                                     | 2.14 sec: 1.05x faster                                       |
| xml_etree_iterparse  | 107 ms                                                       | 102 ms: 1.05x faster                                         |
| pickle_dict          | 32.3 us                                                      | 31.2 us: 1.04x faster                                        |
| pickle_pure_python   | 316 us                                                       | 320 us: 1.01x slower                                         |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                        |
| xml_etree_process    | 55.9 ms                                                      | 58.0 ms: 1.04x slower                                        |
| unpickle_list        | 4.60 us                                                      | 4.82 us: 1.05x slower                                        |
| xml_etree_generate   | 79.7 ms                                                      | 84.6 ms: 1.06x slower                                        |
| pickle_list          | 3.94 us                                                      | 4.46 us: 1.13x slower                                        |
| unpickle             | 13.3 us                                                      | 15.2 us: 1.15x slower                                        |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.08x slower                                        |
| python_startup_no_site | 7.73 ms                                                      | 8.53 ms: 1.10x slower                                        |
| Geometric mean         | (ref)                                                        | 1.09x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.1 ms: 1.09x faster                                        |
| django_template | 39.3 ms                                                      | 37.5 ms: 1.05x faster                                        |
| Geometric mean  | (ref)                                                        | 1.07x faster                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 122 us: 4.37x faster                                         |
| asyncio_tcp                | 747 ms                                                       | 374 ms: 2.00x faster                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.96x faster                                       |
| generators                 | 54.6 ms                                                      | 37.1 ms: 1.47x faster                                        |
| json_dumps                 | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                        |
| richards_super             | 63.6 ms                                                      | 50.7 ms: 1.25x faster                                        |
| deltablue                  | 3.97 ms                                                      | 3.24 ms: 1.22x faster                                        |
| coroutines                 | 27.8 ms                                                      | 22.7 ms: 1.22x faster                                        |
| chaos                      | 74.9 ms                                                      | 62.1 ms: 1.21x faster                                        |
| comprehensions             | 25.1 us                                                      | 20.8 us: 1.20x faster                                        |
| fannkuch                   | 416 ms                                                       | 348 ms: 1.20x faster                                         |
| hexiom                     | 6.98 ms                                                      | 5.91 ms: 1.18x faster                                        |
| sympy_sum                  | 186 ms                                                       | 158 ms: 1.18x faster                                         |
| json_loads                 | 28.9 us                                                      | 24.6 us: 1.17x faster                                        |
| scimark_lu                 | 114 ms                                                       | 97.5 ms: 1.17x faster                                        |
| unpickle_pure_python       | 238 us                                                       | 205 us: 1.16x faster                                         |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                         |
| sympy_expand               | 553 ms                                                       | 479 ms: 1.15x faster                                         |
| async_tree_none            | 518 ms                                                       | 450 ms: 1.15x faster                                         |
| nqueens                    | 103 ms                                                       | 90.0 ms: 1.14x faster                                        |
| sympy_str                  | 337 ms                                                       | 297 ms: 1.13x faster                                         |
| regex_compile              | 156 ms                                                       | 138 ms: 1.13x faster                                         |
| async_tree_io              | 1.17 sec                                                     | 1.04 sec: 1.12x faster                                       |
| richards                   | 49.7 ms                                                      | 44.5 ms: 1.12x faster                                        |
| logging_simple             | 7.24 us                                                      | 6.49 us: 1.12x faster                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 540 ms: 1.11x faster                                         |
| sympy_integrate            | 25.8 ms                                                      | 23.3 ms: 1.11x faster                                        |
| async_tree_none_tg         | 474 ms                                                       | 430 ms: 1.10x faster                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.38 ms: 1.10x faster                                        |
| mdp                        | 2.77 sec                                                     | 2.52 sec: 1.10x faster                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.05 sec: 1.10x faster                                       |
| mako                       | 11.0 ms                                                      | 10.1 ms: 1.09x faster                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 693 ms: 1.09x faster                                         |
| nbody                      | 92.9 ms                                                      | 85.5 ms: 1.09x faster                                        |
| logging_format             | 7.71 us                                                      | 7.11 us: 1.08x faster                                        |
| chameleon                  | 7.92 ms                                                      | 7.31 ms: 1.08x faster                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 695 ms: 1.08x faster                                         |
| json                       | 5.58 ms                                                      | 5.19 ms: 1.08x faster                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.78 ms: 1.08x faster                                        |
| pycparser                  | 1.31 sec                                                     | 1.22 sec: 1.07x faster                                       |
| xml_etree_parse            | 155 ms                                                       | 145 ms: 1.06x faster                                         |
| deepcopy                   | 391 us                                                       | 368 us: 1.06x faster                                         |
| go                         | 158 ms                                                       | 149 ms: 1.06x faster                                         |
| sqlalchemy_imperative      | 19.8 ms                                                      | 18.6 ms: 1.06x faster                                        |
| bench_thread_pool          | 1.00 ms                                                      | 945 us: 1.06x faster                                         |
| crypto_pyaes               | 83.3 ms                                                      | 78.7 ms: 1.06x faster                                        |
| mypy2                      | 762 ms                                                       | 720 ms: 1.06x faster                                         |
| tomli_loads                | 2.25 sec                                                     | 2.14 sec: 1.05x faster                                       |
| tornado_http               | 124 ms                                                       | 118 ms: 1.05x faster                                         |
| dask                       | 410 ms                                                       | 390 ms: 1.05x faster                                         |
| xml_etree_iterparse        | 107 ms                                                       | 102 ms: 1.05x faster                                         |
| dulwich_log                | 67.4 ms                                                      | 64.2 ms: 1.05x faster                                        |
| django_template            | 39.3 ms                                                      | 37.5 ms: 1.05x faster                                        |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                         |
| logging_silent             | 100 ns                                                       | 95.8 ns: 1.05x faster                                        |
| regex_v8                   | 24.4 ms                                                      | 23.5 ms: 1.04x faster                                        |
| pickle_dict                | 32.3 us                                                      | 31.2 us: 1.04x faster                                        |
| raytrace                   | 309 ms                                                       | 299 ms: 1.03x faster                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 67.7 ms: 1.03x faster                                        |
| spectral_norm              | 95.1 ms                                                      | 92.6 ms: 1.03x faster                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.62 sec: 1.03x faster                                       |
| sqlglot_optimize           | 59.0 ms                                                      | 57.6 ms: 1.02x faster                                        |
| 2to3                       | 287 ms                                                       | 281 ms: 1.02x faster                                         |
| pyflate                    | 449 ms                                                       | 441 ms: 1.02x faster                                         |
| pprint_safe_repr           | 805 ms                                                       | 791 ms: 1.02x faster                                         |
| gc_traversal               | 4.15 ms                                                      | 4.10 ms: 1.01x faster                                        |
| scimark_sor                | 110 ms                                                       | 108 ms: 1.01x faster                                         |
| docutils                   | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                       |
| meteor_contest             | 131 ms                                                       | 131 ms: 1.00x slower                                         |
| pickle_pure_python         | 316 us                                                       | 320 us: 1.01x slower                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.60 ms: 1.02x slower                                        |
| pickle                     | 9.89 us                                                      | 10.1 us: 1.02x slower                                        |
| coverage                   | 66.1 ms                                                      | 67.6 ms: 1.02x slower                                        |
| gunicorn                   | 966 us                                                       | 992 us: 1.03x slower                                         |
| float                      | 74.9 ms                                                      | 77.0 ms: 1.03x slower                                        |
| aiohttp                    | 986 us                                                       | 1.02 ms: 1.03x slower                                        |
| sqlalchemy_declarative     | 154 ms                                                       | 160 ms: 1.03x slower                                         |
| xml_etree_process          | 55.9 ms                                                      | 58.0 ms: 1.04x slower                                        |
| unpickle_list              | 4.60 us                                                      | 4.82 us: 1.05x slower                                        |
| pidigits                   | 251 ms                                                       | 265 ms: 1.05x slower                                         |
| scimark_fft                | 281 ms                                                       | 297 ms: 1.06x slower                                         |
| regex_effbot               | 3.34 ms                                                      | 3.54 ms: 1.06x slower                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.31 ms: 1.06x slower                                        |
| xml_etree_generate         | 79.7 ms                                                      | 84.6 ms: 1.06x slower                                        |
| sqlite_synth               | 2.52 us                                                      | 2.69 us: 1.07x slower                                        |
| regex_dna                  | 227 ms                                                       | 244 ms: 1.07x slower                                         |
| unpack_sequence            | 45.7 ns                                                      | 49.1 ns: 1.07x slower                                        |
| python_startup             | 10.7 ms                                                      | 11.5 ms: 1.08x slower                                        |
| telco                      | 6.81 ms                                                      | 7.47 ms: 1.10x slower                                        |
| python_startup_no_site     | 7.73 ms                                                      | 8.53 ms: 1.10x slower                                        |
| pickle_list                | 3.94 us                                                      | 4.46 us: 1.13x slower                                        |
| unpickle                   | 13.3 us                                                      | 15.2 us: 1.15x slower                                        |
| async_generators           | 322 ms                                                       | 379 ms: 1.18x slower                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                 |

Benchmark hidden because not significant (5): deepcopy_reduce, pathlib, deepcopy_memo, asyncio_websockets, bench_mp_pool
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 1.02x