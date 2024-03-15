
# Results vs. 3.11.0

- fork: python
- ref: 384429d1c0cf011dcf88
- machine: windows-amd64
- commit hash: 384429d
- commit date: 2024-01-24
- overall geometric mean: 1.05x faster
- HPT reliability: 99.52%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.04x slower                                                        |
| chameleon      | 5.26 ms                                                     | 5.12 ms: 1.03x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.62 sec: 1.01x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 88.3 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 349 ms: 1.14x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 472 ms: 1.12x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 366 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 742 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 489 ms: 1.07x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 288 ms: 1.07x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| float          | 54.4 ms                                                     | 56.3 ms: 1.04x slower                                                       |
| nbody          | 70.3 ms                                                     | 78.4 ms: 1.11x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.4 ms: 1.08x faster                                                       |
| regex_dna      | 116 ms                                                      | 118 ms: 1.01x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.70 ms: 1.42x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 137 us: 1.15x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 183 us: 1.14x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 95.2 ms: 1.03x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.42 sec: 1.02x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.7 us: 1.01x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.65 us: 1.02x slower                                                       |
| xml_etree_process    | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 68.2 ms: 1.04x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.06x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 56.0 ms: 1.07x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.89 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.30 us: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.35 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.24 ms: 1.05x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 75.7 us: 4.31x faster                                                       |
| generators                 | 34.0 ms                                                     | 22.6 ms: 1.50x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 491 ms: 1.48x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.70 ms: 1.42x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 56.1 ns: 1.28x faster                                                       |
| richards_super             | 38.7 ms                                                     | 31.0 ms: 1.25x faster                                                       |
| raytrace                   | 213 ms                                                      | 174 ms: 1.22x faster                                                        |
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                        |
| comprehensions             | 15.6 us                                                     | 13.0 us: 1.21x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 810 us: 1.18x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 39.9 ns: 1.18x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 137 us: 1.15x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 349 ms: 1.14x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 183 us: 1.14x faster                                                        |
| richards                   | 31.4 ms                                                     | 27.6 ms: 1.14x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.2 ms: 1.13x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 89.2 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 472 ms: 1.12x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 23.2 us: 1.12x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.18 us: 1.11x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.44 sec: 1.11x faster                                                      |
| sympy_str                  | 185 ms                                                      | 167 ms: 1.11x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 366 ms: 1.11x faster                                                        |
| chaos                      | 48.4 ms                                                     | 44.1 ms: 1.10x faster                                                       |
| go                         | 101 ms                                                      | 92.4 ms: 1.09x faster                                                       |
| async_tree_io              | 808 ms                                                      | 742 ms: 1.09x faster                                                        |
| deepcopy                   | 246 us                                                      | 228 us: 1.08x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 84.4 ms: 1.08x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.69 us: 1.07x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 489 ms: 1.07x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 288 ms: 1.07x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.90 sec: 1.07x faster                                                      |
| dulwich_log                | 46.4 ms                                                     | 43.5 ms: 1.07x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 59.2 ms: 1.06x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                                        |
| mypy2                      | 459 ms                                                      | 434 ms: 1.06x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.05x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 64.9 ms: 1.05x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 88.3 ms: 1.05x faster                                                       |
| mako                       | 7.58 ms                                                     | 7.24 ms: 1.05x faster                                                       |
| sympy_expand               | 299 ms                                                      | 285 ms: 1.05x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 183 ms: 1.04x faster                                                        |
| dask                       | 273 ms                                                      | 264 ms: 1.04x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 5.12 ms: 1.03x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 95.2 ms: 1.03x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 2.01 us: 1.02x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.42 sec: 1.02x faster                                                      |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.62 sec: 1.01x faster                                                      |
| pprint_pformat             | 1.09 sec                                                    | 1.08 sec: 1.01x faster                                                      |
| deltablue                  | 2.70 ms                                                     | 2.68 ms: 1.01x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 525 ms: 1.01x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 48.6 ms: 1.01x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.7 us: 1.01x slower                                                       |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.01x slower                                                        |
| unpickle_list              | 2.59 us                                                     | 2.65 us: 1.02x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.54 ms: 1.03x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.6 ms: 1.03x slower                                                       |
| float                      | 54.4 ms                                                     | 56.3 ms: 1.04x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 68.2 ms: 1.04x slower                                                       |
| 2to3                       | 214 ms                                                      | 223 ms: 1.04x slower                                                        |
| fannkuch                   | 253 ms                                                      | 264 ms: 1.04x slower                                                        |
| pyflate                    | 312 ms                                                      | 326 ms: 1.04x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 748 us: 1.05x slower                                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.8 ms: 1.06x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.8 us: 1.06x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 4.85 ms: 1.06x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 56.0 ms: 1.07x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.89 us: 1.07x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 68.2 ms: 1.08x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 84.4 ms: 1.08x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.7 ms: 1.10x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.30 us: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.35 us: 1.10x slower                                                       |
| nbody                      | 70.3 ms                                                     | 78.4 ms: 1.11x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 80.5 ms: 1.14x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.67 ms: 1.15x slower                                                       |
| scimark_fft                | 179 ms                                                      | 207 ms: 1.15x slower                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.05 ms: 1.18x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 81.0 ms: 1.19x slower                                                       |
| async_generators           | 177 ms                                                      | 232 ms: 1.31x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (4): bench_thread_pool, meteor_contest, pycparser, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.52% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown