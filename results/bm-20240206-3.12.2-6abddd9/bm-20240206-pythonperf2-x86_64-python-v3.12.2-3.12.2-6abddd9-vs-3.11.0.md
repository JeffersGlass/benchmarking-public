
# Results vs. 3.11.0

- fork: python
- ref: v3.12.2
- machine: linux-x86_64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 284 ms: 1.01x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.35 ms: 1.08x faster                                        |
| tornado_http   | 124 ms                                                       | 119 ms: 1.05x faster                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_memoization     | 629 ms                                                       | 550 ms: 1.14x faster                                         |
| async_tree_none            | 518 ms                                                       | 458 ms: 1.13x faster                                         |
| async_tree_io              | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 548 ms: 1.09x faster                                         |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 703 ms: 1.07x faster                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 705 ms: 1.06x faster                                         |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 87.7 ms: 1.06x faster                                        |
| float          | 74.9 ms                                                      | 77.7 ms: 1.04x slower                                        |
| pidigits       | 251 ms                                                       | 265 ms: 1.06x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 140 ms: 1.11x faster                                         |
| regex_v8       | 24.4 ms                                                      | 23.7 ms: 1.03x faster                                        |
| regex_effbot   | 3.34 ms                                                      | 3.43 ms: 1.03x slower                                        |
| regex_dna      | 227 ms                                                       | 236 ms: 1.04x slower                                         |
| Geometric mean | (ref)                                                        | 1.02x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.4 ms: 1.28x faster                                        |
| json_loads           | 28.9 us                                                      | 24.5 us: 1.18x faster                                        |
| unpickle_pure_python | 238 us                                                       | 203 us: 1.17x faster                                         |
| xml_etree_parse      | 155 ms                                                       | 149 ms: 1.04x faster                                         |
| tomli_loads          | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                       |
| xml_etree_iterparse  | 107 ms                                                       | 104 ms: 1.03x faster                                         |
| pickle_dict          | 32.3 us                                                      | 32.4 us: 1.00x slower                                        |
| pickle_pure_python   | 316 us                                                       | 321 us: 1.02x slower                                         |
| unpickle_list        | 4.60 us                                                      | 4.69 us: 1.02x slower                                        |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                        |
| xml_etree_process    | 55.9 ms                                                      | 58.9 ms: 1.05x slower                                        |
| xml_etree_generate   | 79.7 ms                                                      | 86.1 ms: 1.08x slower                                        |
| unpickle             | 13.3 us                                                      | 14.9 us: 1.12x slower                                        |
| pickle_list          | 3.94 us                                                      | 4.52 us: 1.15x slower                                        |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.6 ms: 1.08x slower                                        |
| python_startup_no_site | 7.73 ms                                                      | 8.50 ms: 1.10x slower                                        |
| Geometric mean         | (ref)                                                        | 1.09x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 9.97 ms: 1.10x faster                                        |
| django_template | 39.3 ms                                                      | 38.5 ms: 1.02x faster                                        |
| Geometric mean  | (ref)                                                        | 1.06x faster                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 124 us: 4.30x faster                                         |
| asyncio_tcp                | 747 ms                                                       | 374 ms: 2.00x faster                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.56 sec: 1.96x faster                                       |
| generators                 | 54.6 ms                                                      | 36.7 ms: 1.49x faster                                        |
| json_dumps                 | 13.3 ms                                                      | 10.4 ms: 1.28x faster                                        |
| richards_super             | 63.6 ms                                                      | 50.8 ms: 1.25x faster                                        |
| fannkuch                   | 416 ms                                                       | 339 ms: 1.23x faster                                         |
| deltablue                  | 3.97 ms                                                      | 3.24 ms: 1.22x faster                                        |
| coroutines                 | 27.8 ms                                                      | 22.9 ms: 1.21x faster                                        |
| comprehensions             | 25.1 us                                                      | 21.1 us: 1.19x faster                                        |
| chaos                      | 74.9 ms                                                      | 63.1 ms: 1.19x faster                                        |
| json_loads                 | 28.9 us                                                      | 24.5 us: 1.18x faster                                        |
| unpickle_pure_python       | 238 us                                                       | 203 us: 1.17x faster                                         |
| nqueens                    | 103 ms                                                       | 88.6 ms: 1.16x faster                                        |
| sympy_sum                  | 186 ms                                                       | 161 ms: 1.16x faster                                         |
| hexiom                     | 6.98 ms                                                      | 6.07 ms: 1.15x faster                                        |
| async_tree_memoization     | 629 ms                                                       | 550 ms: 1.14x faster                                         |
| scimark_lu                 | 114 ms                                                       | 99.7 ms: 1.14x faster                                        |
| async_tree_none            | 518 ms                                                       | 458 ms: 1.13x faster                                         |
| richards                   | 49.7 ms                                                      | 44.3 ms: 1.12x faster                                        |
| sympy_expand               | 553 ms                                                       | 496 ms: 1.12x faster                                         |
| regex_compile              | 156 ms                                                       | 140 ms: 1.11x faster                                         |
| sympy_str                  | 337 ms                                                       | 303 ms: 1.11x faster                                         |
| gc_traversal               | 4.15 ms                                                      | 3.74 ms: 1.11x faster                                        |
| async_tree_io              | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                       |
| mako                       | 11.0 ms                                                      | 9.97 ms: 1.10x faster                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 548 ms: 1.09x faster                                         |
| sympy_integrate            | 25.8 ms                                                      | 23.7 ms: 1.09x faster                                        |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                         |
| mdp                        | 2.77 sec                                                     | 2.56 sec: 1.08x faster                                       |
| sqlglot_parse              | 1.51 ms                                                      | 1.40 ms: 1.08x faster                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                       |
| logging_simple             | 7.24 us                                                      | 6.72 us: 1.08x faster                                        |
| chameleon                  | 7.92 ms                                                      | 7.35 ms: 1.08x faster                                        |
| json                       | 5.58 ms                                                      | 5.18 ms: 1.08x faster                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 703 ms: 1.07x faster                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 705 ms: 1.06x faster                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.80 ms: 1.06x faster                                        |
| sqlalchemy_imperative      | 19.8 ms                                                      | 18.6 ms: 1.06x faster                                        |
| nbody                      | 92.9 ms                                                      | 87.7 ms: 1.06x faster                                        |
| go                         | 158 ms                                                       | 149 ms: 1.06x faster                                         |
| bench_thread_pool          | 1.00 ms                                                      | 949 us: 1.05x faster                                         |
| mypy2                      | 762 ms                                                       | 723 ms: 1.05x faster                                         |
| deepcopy                   | 391 us                                                       | 371 us: 1.05x faster                                         |
| crypto_pyaes               | 83.3 ms                                                      | 79.5 ms: 1.05x faster                                        |
| tornado_http               | 124 ms                                                       | 119 ms: 1.05x faster                                         |
| dask                       | 410 ms                                                       | 392 ms: 1.05x faster                                         |
| logging_format             | 7.71 us                                                      | 7.40 us: 1.04x faster                                        |
| xml_etree_parse            | 155 ms                                                       | 149 ms: 1.04x faster                                         |
| dulwich_log                | 67.4 ms                                                      | 64.9 ms: 1.04x faster                                        |
| raytrace                   | 309 ms                                                       | 298 ms: 1.04x faster                                         |
| meteor_contest             | 131 ms                                                       | 126 ms: 1.04x faster                                         |
| tomli_loads                | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                       |
| pycparser                  | 1.31 sec                                                     | 1.27 sec: 1.03x faster                                       |
| xml_etree_iterparse        | 107 ms                                                       | 104 ms: 1.03x faster                                         |
| regex_v8                   | 24.4 ms                                                      | 23.7 ms: 1.03x faster                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 68.0 ms: 1.03x faster                                        |
| sqlglot_normalize          | 122 ms                                                       | 119 ms: 1.02x faster                                         |
| spectral_norm              | 95.1 ms                                                      | 92.8 ms: 1.02x faster                                        |
| django_template            | 39.3 ms                                                      | 38.5 ms: 1.02x faster                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 58.0 ms: 1.02x faster                                        |
| asyncio_websockets         | 390 ms                                                       | 385 ms: 1.01x faster                                         |
| deepcopy_memo              | 37.5 us                                                      | 37.1 us: 1.01x faster                                        |
| 2to3                       | 287 ms                                                       | 284 ms: 1.01x faster                                         |
| pickle_dict                | 32.3 us                                                      | 32.4 us: 1.00x slower                                        |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.68 sec: 1.01x slower                                       |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.12 ms: 1.01x slower                                        |
| pickle_pure_python         | 316 us                                                       | 321 us: 1.02x slower                                         |
| unpickle_list              | 4.60 us                                                      | 4.69 us: 1.02x slower                                        |
| pyflate                    | 449 ms                                                       | 461 ms: 1.03x slower                                         |
| regex_effbot               | 3.34 ms                                                      | 3.43 ms: 1.03x slower                                        |
| pprint_safe_repr           | 805 ms                                                       | 827 ms: 1.03x slower                                         |
| gunicorn                   | 966 us                                                       | 996 us: 1.03x slower                                         |
| scimark_fft                | 281 ms                                                       | 290 ms: 1.03x slower                                         |
| float                      | 74.9 ms                                                      | 77.7 ms: 1.04x slower                                        |
| regex_dna                  | 227 ms                                                       | 236 ms: 1.04x slower                                         |
| sqlalchemy_declarative     | 154 ms                                                       | 160 ms: 1.04x slower                                         |
| aiohttp                    | 986 us                                                       | 1.02 ms: 1.04x slower                                        |
| pickle                     | 9.89 us                                                      | 10.3 us: 1.04x slower                                        |
| xml_etree_process          | 55.9 ms                                                      | 58.9 ms: 1.05x slower                                        |
| pidigits                   | 251 ms                                                       | 265 ms: 1.06x slower                                         |
| bench_mp_pool              | 4.70 ms                                                      | 5.00 ms: 1.06x slower                                        |
| telco                      | 6.81 ms                                                      | 7.27 ms: 1.07x slower                                        |
| python_startup             | 10.7 ms                                                      | 11.6 ms: 1.08x slower                                        |
| sqlite_synth               | 2.52 us                                                      | 2.73 us: 1.08x slower                                        |
| xml_etree_generate         | 79.7 ms                                                      | 86.1 ms: 1.08x slower                                        |
| python_startup_no_site     | 7.73 ms                                                      | 8.50 ms: 1.10x slower                                        |
| unpickle                   | 13.3 us                                                      | 14.9 us: 1.12x slower                                        |
| unpack_sequence            | 45.7 ns                                                      | 52.0 ns: 1.14x slower                                        |
| pickle_list                | 3.94 us                                                      | 4.52 us: 1.15x slower                                        |
| async_generators           | 322 ms                                                       | 393 ms: 1.22x slower                                         |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                 |

Benchmark hidden because not significant (6): deepcopy_reduce, logging_silent, docutils, scimark_sor, create_gc_cycles, coverage
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x