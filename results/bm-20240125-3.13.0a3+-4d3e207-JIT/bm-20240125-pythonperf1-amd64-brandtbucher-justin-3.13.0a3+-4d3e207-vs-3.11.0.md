
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: windows-amd64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 220 ms: 1.03x slower                                                |
| chameleon      | 5.26 ms                                                     | 4.91 ms: 1.07x faster                                               |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                              |
| tornado_http   | 92.8 ms                                                     | 86.0 ms: 1.08x faster                                               |
| Geometric mean | (ref)                                                       | 1.04x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 459 ms: 1.15x faster                                                |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                                |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                |
| async_tree_io              | 808 ms                                                      | 730 ms: 1.11x faster                                                |
| async_tree_none_tg         | 309 ms                                                      | 280 ms: 1.10x faster                                                |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 485 ms: 1.08x faster                                                |
| async_tree_io_tg           | 829 ms                                                      | 769 ms: 1.08x faster                                                |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 60.8 ms: 1.16x faster                                               |
| float          | 54.4 ms                                                     | 50.4 ms: 1.08x faster                                               |
| pidigits       | 150 ms                                                      | 154 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                       | 1.07x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 82.3 ms: 1.11x faster                                               |
| regex_dna      | 116 ms                                                      | 119 ms: 1.02x slower                                                |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.06x slower                                               |
| regex_v8       | 14.2 ms                                                     | 16.9 ms: 1.19x slower                                               |
| Geometric mean | (ref)                                                       | 1.04x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.56 ms: 1.46x faster                                               |
| unpickle_pure_python | 157 us                                                      | 131 us: 1.20x faster                                                |
| pickle_pure_python   | 208 us                                                      | 176 us: 1.18x faster                                                |
| tomli_loads          | 1.46 sec                                                    | 1.35 sec: 1.08x faster                                              |
| xml_etree_parse      | 97.6 ms                                                     | 94.6 ms: 1.03x faster                                               |
| xml_etree_process    | 37.2 ms                                                     | 36.6 ms: 1.02x faster                                               |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                               |
| pickle_dict          | 18.5 us                                                     | 18.6 us: 1.00x slower                                               |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                               |
| unpickle_list        | 2.59 us                                                     | 2.75 us: 1.06x slower                                               |
| pickle_list          | 2.70 us                                                     | 2.96 us: 1.10x slower                                               |
| pickle               | 6.64 us                                                     | 7.35 us: 1.11x slower                                               |
| unpickle             | 7.57 us                                                     | 8.61 us: 1.14x slower                                               |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                        |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.0 ms: 1.06x slower                                               |
| python_startup_no_site | 16.8 ms                                                     | 19.1 ms: 1.13x slower                                               |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.98 ms: 1.09x faster                                               |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 72.1 us: 4.52x faster                                               |
| generators                 | 34.0 ms                                                     | 20.1 ms: 1.69x faster                                               |
| asyncio_tcp                | 726 ms                                                      | 487 ms: 1.49x faster                                                |
| json_dumps                 | 8.09 ms                                                     | 5.56 ms: 1.46x faster                                               |
| comprehensions             | 15.6 us                                                     | 11.4 us: 1.37x faster                                               |
| richards_super             | 38.7 ms                                                     | 28.8 ms: 1.35x faster                                               |
| logging_silent             | 71.8 ns                                                     | 54.5 ns: 1.32x faster                                               |
| deltablue                  | 2.70 ms                                                     | 2.08 ms: 1.30x faster                                               |
| richards                   | 31.4 ms                                                     | 25.5 ms: 1.23x faster                                               |
| raytrace                   | 213 ms                                                      | 175 ms: 1.22x faster                                                |
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                |
| sqlglot_parse              | 953 us                                                      | 784 us: 1.22x faster                                                |
| unpickle_pure_python       | 157 us                                                      | 131 us: 1.20x faster                                                |
| unpack_sequence            | 46.9 ns                                                     | 39.5 ns: 1.19x faster                                               |
| pickle_pure_python         | 208 us                                                      | 176 us: 1.18x faster                                                |
| deepcopy_memo              | 26.0 us                                                     | 22.1 us: 1.18x faster                                               |
| nqueens                    | 68.3 ms                                                     | 59.1 ms: 1.16x faster                                               |
| nbody                      | 70.3 ms                                                     | 60.8 ms: 1.16x faster                                               |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.16x faster                                               |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 459 ms: 1.15x faster                                                |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                                |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                               |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                |
| logging_simple             | 6.86 us                                                     | 6.03 us: 1.14x faster                                               |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.13x faster                                               |
| sympy_sum                  | 100 ms                                                      | 88.9 ms: 1.13x faster                                               |
| scimark_lu                 | 62.8 ms                                                     | 55.9 ms: 1.12x faster                                               |
| deepcopy                   | 246 us                                                      | 221 us: 1.12x faster                                                |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.82 sec: 1.11x faster                                              |
| async_tree_io              | 808 ms                                                      | 730 ms: 1.11x faster                                                |
| logging_format             | 7.16 us                                                     | 6.47 us: 1.11x faster                                               |
| chaos                      | 48.4 ms                                                     | 43.7 ms: 1.11x faster                                               |
| regex_compile              | 91.0 ms                                                     | 82.3 ms: 1.11x faster                                               |
| sympy_str                  | 185 ms                                                      | 168 ms: 1.10x faster                                                |
| async_tree_none_tg         | 309 ms                                                      | 280 ms: 1.10x faster                                                |
| mako                       | 7.58 ms                                                     | 6.98 ms: 1.09x faster                                               |
| float                      | 54.4 ms                                                     | 50.4 ms: 1.08x faster                                               |
| tornado_http               | 92.8 ms                                                     | 86.0 ms: 1.08x faster                                               |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 485 ms: 1.08x faster                                                |
| async_tree_io_tg           | 829 ms                                                      | 769 ms: 1.08x faster                                                |
| tomli_loads                | 1.46 sec                                                    | 1.35 sec: 1.08x faster                                              |
| dulwich_log                | 46.4 ms                                                     | 43.2 ms: 1.07x faster                                               |
| chameleon                  | 5.26 ms                                                     | 4.91 ms: 1.07x faster                                               |
| sympy_expand               | 299 ms                                                      | 280 ms: 1.07x faster                                                |
| sqlglot_normalize          | 190 ms                                                      | 180 ms: 1.06x faster                                                |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.06x faster                                               |
| deepcopy_reduce            | 2.06 us                                                     | 1.95 us: 1.05x faster                                               |
| mypy2                      | 459 ms                                                      | 436 ms: 1.05x faster                                                |
| pprint_safe_repr           | 529 ms                                                      | 504 ms: 1.05x faster                                                |
| spectral_norm              | 68.3 ms                                                     | 65.3 ms: 1.05x faster                                               |
| pprint_pformat             | 1.09 sec                                                    | 1.05 sec: 1.04x faster                                              |
| go                         | 101 ms                                                      | 97.4 ms: 1.04x faster                                               |
| crypto_pyaes               | 48.9 ms                                                     | 47.2 ms: 1.04x faster                                               |
| xml_etree_parse            | 97.6 ms                                                     | 94.6 ms: 1.03x faster                                               |
| dask                       | 273 ms                                                      | 265 ms: 1.03x faster                                                |
| mdp                        | 1.59 sec                                                    | 1.55 sec: 1.03x faster                                              |
| fannkuch                   | 253 ms                                                      | 247 ms: 1.03x faster                                                |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                              |
| xml_etree_process          | 37.2 ms                                                     | 36.6 ms: 1.02x faster                                               |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                               |
| pickle_dict                | 18.5 us                                                     | 18.6 us: 1.00x slower                                               |
| scimark_sor                | 78.1 ms                                                     | 78.7 ms: 1.01x slower                                               |
| pyflate                    | 312 ms                                                      | 320 ms: 1.02x slower                                                |
| pidigits                   | 150 ms                                                      | 154 ms: 1.02x slower                                                |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.02x slower                                                |
| gc_traversal               | 1.49 ms                                                     | 1.54 ms: 1.03x slower                                               |
| 2to3                       | 214 ms                                                      | 220 ms: 1.03x slower                                                |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                               |
| meteor_contest             | 75.2 ms                                                     | 78.7 ms: 1.05x slower                                               |
| coverage                   | 43.4 ms                                                     | 45.7 ms: 1.05x slower                                               |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.06x slower                                               |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.72 ms: 1.06x slower                                               |
| create_gc_cycles           | 713 us                                                      | 754 us: 1.06x slower                                                |
| python_startup             | 19.8 ms                                                     | 21.0 ms: 1.06x slower                                               |
| unpickle_list              | 2.59 us                                                     | 2.75 us: 1.06x slower                                               |
| scimark_fft                | 179 ms                                                      | 196 ms: 1.09x slower                                                |
| bench_mp_pool              | 63.2 ms                                                     | 69.2 ms: 1.09x slower                                               |
| pickle_list                | 2.70 us                                                     | 2.96 us: 1.10x slower                                               |
| pickle                     | 6.64 us                                                     | 7.35 us: 1.11x slower                                               |
| telco                      | 4.06 ms                                                     | 4.58 ms: 1.13x slower                                               |
| pathlib                    | 70.9 ms                                                     | 80.1 ms: 1.13x slower                                               |
| python_startup_no_site     | 16.8 ms                                                     | 19.1 ms: 1.13x slower                                               |
| unpickle                   | 7.57 us                                                     | 8.61 us: 1.14x slower                                               |
| hexiom                     | 4.55 ms                                                     | 5.29 ms: 1.16x slower                                               |
| regex_v8                   | 14.2 ms                                                     | 16.9 ms: 1.19x slower                                               |
| scimark_monte_carlo        | 45.3 ms                                                     | 58.7 ms: 1.30x slower                                               |
| async_generators           | 177 ms                                                      | 241 ms: 1.36x slower                                                |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                        |

Benchmark hidden because not significant (5): json, pycparser, bench_thread_pool, xml_etree_generate, sqlglot_optimize
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown