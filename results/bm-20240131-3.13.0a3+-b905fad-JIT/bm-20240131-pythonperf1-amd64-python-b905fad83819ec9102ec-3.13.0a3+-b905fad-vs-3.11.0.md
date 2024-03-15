
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 222 ms: 1.04x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.72 ms: 1.12x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 86.3 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 462 ms: 1.15x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 350 ms: 1.14x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 358 ms: 1.13x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 473 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 749 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 770 ms: 1.08x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 63.0 ms: 1.12x faster                                                       |
| float          | 54.4 ms                                                     | 52.0 ms: 1.04x faster                                                       |
| pidigits       | 150 ms                                                      | 154 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 81.6 ms: 1.12x faster                                                       |
| regex_dna      | 116 ms                                                      | 125 ms: 1.08x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 17.0 ms: 1.20x slower                                                       |
| Geometric mean | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.51 ms: 1.47x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 127 us: 1.23x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 177 us: 1.18x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.28 sec: 1.14x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 35.7 ms: 1.04x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 17.9 us: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.7 ms: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 51.8 ms: 1.01x faster                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.84 us: 1.06x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.77 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.21 us: 1.09x slower                                                       |
| unpickle             | 7.57 us                                                     | 9.00 us: 1.19x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.6 ms: 1.09x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 19.6 ms: 1.17x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.78 ms: 1.12x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.2 us: 4.64x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.2 ms: 1.68x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 492 ms: 1.47x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.51 ms: 1.47x faster                                                       |
| richards_super             | 38.7 ms                                                     | 28.5 ms: 1.36x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 53.2 ns: 1.35x faster                                                       |
| comprehensions             | 15.6 us                                                     | 11.6 us: 1.35x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.10 ms: 1.29x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 757 us: 1.26x faster                                                        |
| raytrace                   | 213 ms                                                      | 170 ms: 1.26x faster                                                        |
| richards                   | 31.4 ms                                                     | 25.4 ms: 1.24x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 127 us: 1.23x faster                                                        |
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 21.8 us: 1.19x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 177 us: 1.18x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 39.8 ns: 1.18x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 990 us: 1.18x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.74 sec: 1.16x faster                                                      |
| coroutines                 | 15.0 ms                                                     | 12.9 ms: 1.16x faster                                                       |
| logging_simple             | 6.86 us                                                     | 5.97 us: 1.15x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 59.5 ms: 1.15x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 462 ms: 1.15x faster                                                        |
| chaos                      | 48.4 ms                                                     | 42.4 ms: 1.14x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 350 ms: 1.14x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.28 sec: 1.14x faster                                                      |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.13x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 55.5 ms: 1.13x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 358 ms: 1.13x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                        |
| mako                       | 7.58 ms                                                     | 6.78 ms: 1.12x faster                                                       |
| nbody                      | 70.3 ms                                                     | 63.0 ms: 1.12x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.42 us: 1.12x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 81.6 ms: 1.12x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.72 ms: 1.12x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 90.3 ms: 1.11x faster                                                       |
| deepcopy                   | 246 us                                                      | 222 us: 1.11x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 473 ms: 1.11x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 42.0 ms: 1.10x faster                                                       |
| sympy_str                  | 185 ms                                                      | 169 ms: 1.09x faster                                                        |
| async_tree_io              | 808 ms                                                      | 749 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 770 ms: 1.08x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 86.3 ms: 1.08x faster                                                       |
| sympy_expand               | 299 ms                                                      | 282 ms: 1.06x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 180 ms: 1.05x faster                                                        |
| mypy2                      | 459 ms                                                      | 436 ms: 1.05x faster                                                        |
| pprint_safe_repr           | 529 ms                                                      | 503 ms: 1.05x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.03 sec: 1.05x faster                                                      |
| sympy_integrate            | 14.0 ms                                                     | 13.4 ms: 1.05x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.96 us: 1.05x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 65.2 ms: 1.05x faster                                                       |
| pycparser                  | 720 ms                                                      | 688 ms: 1.05x faster                                                        |
| float                      | 54.4 ms                                                     | 52.0 ms: 1.04x faster                                                       |
| dask                       | 273 ms                                                      | 261 ms: 1.04x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 46.8 ms: 1.04x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 35.7 ms: 1.04x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.9 us: 1.04x faster                                                       |
| scimark_sor                | 78.1 ms                                                     | 76.1 ms: 1.03x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                      |
| fannkuch                   | 253 ms                                                      | 248 ms: 1.02x faster                                                        |
| go                         | 101 ms                                                      | 99.3 ms: 1.02x faster                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.7 ms: 1.01x faster                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 51.8 ms: 1.01x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.58 sec: 1.01x faster                                                      |
| gc_traversal               | 1.49 ms                                                     | 1.50 ms: 1.01x slower                                                       |
| pyflate                    | 312 ms                                                      | 315 ms: 1.01x slower                                                        |
| pidigits                   | 150 ms                                                      | 154 ms: 1.03x slower                                                        |
| 2to3                       | 214 ms                                                      | 222 ms: 1.04x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 78.7 ms: 1.05x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 748 us: 1.05x slower                                                        |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.84 us: 1.06x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.72 ms: 1.06x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.77 us: 1.07x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.6 ms: 1.07x slower                                                       |
| regex_dna                  | 116 ms                                                      | 125 ms: 1.08x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.21 us: 1.09x slower                                                       |
| python_startup             | 19.8 ms                                                     | 21.6 ms: 1.09x slower                                                       |
| scimark_fft                | 179 ms                                                      | 197 ms: 1.10x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 80.1 ms: 1.13x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.60 ms: 1.13x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.27 ms: 1.16x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 73.2 ms: 1.16x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 19.6 ms: 1.17x slower                                                       |
| unpickle                   | 7.57 us                                                     | 9.00 us: 1.19x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 17.0 ms: 1.20x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 58.0 ms: 1.28x slower                                                       |
| async_generators           | 177 ms                                                      | 240 ms: 1.36x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                                |

Benchmark hidden because not significant (3): json, sqlglot_optimize, bench_thread_pool
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown