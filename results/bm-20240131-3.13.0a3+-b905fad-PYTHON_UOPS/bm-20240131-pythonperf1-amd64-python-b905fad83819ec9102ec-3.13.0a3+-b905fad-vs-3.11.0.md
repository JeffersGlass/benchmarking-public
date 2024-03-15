
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.04x faster
- HPT reliability: 99.42%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 225 ms: 1.05x slower                                                        |
| tornado_http   | 92.8 ms                                                     | 88.0 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (2): chameleon, docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 275 ms: 1.21x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 354 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 471 ms: 1.13x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 371 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 487 ms: 1.07x faster                                                        |
| async_tree_io              | 808 ms                                                      | 754 ms: 1.07x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 289 ms: 1.07x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 787 ms: 1.05x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 149 ms: 1.01x faster                                                        |
| float          | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                                       |
| nbody          | 70.3 ms                                                     | 83.0 ms: 1.18x slower                                                       |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 85.3 ms: 1.07x faster                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.63 ms: 1.09x slower                                                       |
| regex_dna      | 116 ms                                                      | 129 ms: 1.11x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 18.5 ms: 1.31x slower                                                       |
| Geometric mean | (ref)                                                       | 1.10x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.78 ms: 1.40x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 185 us: 1.13x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 143 us: 1.09x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 93.5 ms: 1.04x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.42 sec: 1.03x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.7 us: 1.01x slower                                                       |
| xml_etree_process    | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 67.7 ms: 1.03x slower                                                       |
| pickle               | 6.64 us                                                     | 7.09 us: 1.07x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.9 us: 1.07x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 56.7 ms: 1.08x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.93 us: 1.09x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.82 us: 1.09x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.60 us: 1.14x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.4 ms: 1.09x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.44 ms: 1.02x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 74.2 us: 4.39x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.7 ms: 1.56x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 478 ms: 1.52x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.78 ms: 1.40x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 56.8 ns: 1.26x faster                                                       |
| richards_super             | 38.7 ms                                                     | 31.7 ms: 1.22x faster                                                       |
| raytrace                   | 213 ms                                                      | 176 ms: 1.22x faster                                                        |
| async_tree_none            | 332 ms                                                      | 275 ms: 1.21x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 797 us: 1.20x faster                                                        |
| comprehensions             | 15.6 us                                                     | 13.1 us: 1.19x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.02 ms: 1.15x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 88.2 ms: 1.13x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 185 us: 1.13x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 354 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 471 ms: 1.13x faster                                                        |
| richards                   | 31.4 ms                                                     | 28.1 ms: 1.12x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.4 ms: 1.12x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 23.3 us: 1.11x faster                                                       |
| go                         | 101 ms                                                      | 91.1 ms: 1.11x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.60 us: 1.11x faster                                                       |
| sympy_str                  | 185 ms                                                      | 168 ms: 1.10x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.46 sec: 1.10x faster                                                      |
| logging_simple             | 6.86 us                                                     | 6.27 us: 1.09x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 143 us: 1.09x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 371 ms: 1.09x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.86 sec: 1.09x faster                                                      |
| chaos                      | 48.4 ms                                                     | 44.5 ms: 1.09x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 43.2 ns: 1.09x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 58.4 ms: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 487 ms: 1.07x faster                                                        |
| deepcopy                   | 246 us                                                      | 230 us: 1.07x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 63.8 ms: 1.07x faster                                                       |
| async_tree_io              | 808 ms                                                      | 754 ms: 1.07x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 85.3 ms: 1.07x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 289 ms: 1.07x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 43.6 ms: 1.06x faster                                                       |
| mypy2                      | 459 ms                                                      | 432 ms: 1.06x faster                                                        |
| sympy_expand               | 299 ms                                                      | 282 ms: 1.06x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 88.0 ms: 1.05x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 787 ms: 1.05x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 93.5 ms: 1.04x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.5 ms: 1.04x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.92 us: 1.04x faster                                                       |
| dask                       | 273 ms                                                      | 264 ms: 1.03x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 2.01 us: 1.03x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.42 sec: 1.03x faster                                                      |
| bench_thread_pool          | 872 us                                                      | 853 us: 1.02x faster                                                        |
| deltablue                  | 2.70 ms                                                     | 2.64 ms: 1.02x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 187 ms: 1.02x faster                                                        |
| mako                       | 7.58 ms                                                     | 7.44 ms: 1.02x faster                                                       |
| pycparser                  | 720 ms                                                      | 707 ms: 1.02x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 48.2 ms: 1.01x faster                                                       |
| pidigits                   | 150 ms                                                      | 149 ms: 1.01x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 18.7 us: 1.01x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.1 ms: 1.02x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 67.7 ms: 1.03x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.54 ms: 1.03x slower                                                       |
| meteor_contest             | 75.2 ms                                                     | 78.0 ms: 1.04x slower                                                       |
| pyflate                    | 312 ms                                                      | 324 ms: 1.04x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 745 us: 1.04x slower                                                        |
| python_startup             | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 4.79 ms: 1.05x slower                                                       |
| float                      | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                                       |
| 2to3                       | 214 ms                                                      | 225 ms: 1.05x slower                                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 48.0 ms: 1.06x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 83.0 ms: 1.06x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.09 us: 1.07x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.9 us: 1.07x slower                                                       |
| fannkuch                   | 253 ms                                                      | 272 ms: 1.07x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 56.7 ms: 1.08x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 68.2 ms: 1.08x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.63 ms: 1.09x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.93 us: 1.09x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.82 us: 1.09x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.5 ms: 1.09x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.4 ms: 1.09x slower                                                       |
| regex_dna                  | 116 ms                                                      | 129 ms: 1.11x slower                                                        |
| unpickle                   | 7.57 us                                                     | 8.60 us: 1.14x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 81.0 ms: 1.14x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.73 ms: 1.16x slower                                                       |
| scimark_fft                | 179 ms                                                      | 211 ms: 1.18x slower                                                        |
| nbody                      | 70.3 ms                                                     | 83.0 ms: 1.18x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 82.2 ms: 1.20x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.14 ms: 1.22x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 18.5 ms: 1.31x slower                                                       |
| async_generators           | 177 ms                                                      | 235 ms: 1.32x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (5): docutils, json, pprint_pformat, pprint_safe_repr, chameleon
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.42% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown