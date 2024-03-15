
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a3
- machine: windows-amd64
- commit hash: f009305
- commit date: 2024-01-17
- overall geometric mean: 1.06x faster
- HPT reliability: 99.87%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 217 ms: 1.02x slower                                            |
| chameleon      | 5.26 ms                                                     | 5.10 ms: 1.03x faster                                           |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                          |
| tornado_http   | 92.8 ms                                                     | 88.2 ms: 1.05x faster                                           |
| Geometric mean | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                            |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                            |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                            |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                            |
| async_tree_none_tg         | 309 ms                                                      | 275 ms: 1.12x faster                                            |
| async_tree_io              | 808 ms                                                      | 722 ms: 1.12x faster                                            |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 469 ms: 1.12x faster                                            |
| async_tree_io_tg           | 829 ms                                                      | 748 ms: 1.11x faster                                            |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.02x faster                                            |
| float          | 54.4 ms                                                     | 55.5 ms: 1.02x slower                                           |
| nbody          | 70.3 ms                                                     | 79.2 ms: 1.13x slower                                           |
| Geometric mean | (ref)                                                       | 1.04x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.2 ms: 1.08x faster                                           |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                            |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                           |
| regex_v8       | 14.2 ms                                                     | 15.5 ms: 1.10x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                           |
| unpickle_pure_python | 157 us                                                      | 137 us: 1.15x faster                                            |
| pickle_pure_python   | 208 us                                                      | 182 us: 1.15x faster                                            |
| tomli_loads          | 1.46 sec                                                    | 1.38 sec: 1.05x faster                                          |
| xml_etree_parse      | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                           |
| pickle_dict          | 18.5 us                                                     | 18.8 us: 1.02x slower                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 67.5 ms: 1.03x slower                                           |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.04x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 55.2 ms: 1.05x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.73 us: 1.05x slower                                           |
| unpickle             | 7.57 us                                                     | 8.21 us: 1.08x slower                                           |
| pickle               | 6.64 us                                                     | 7.37 us: 1.11x slower                                           |
| pickle_list          | 2.70 us                                                     | 3.08 us: 1.14x slower                                           |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                    |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.7 ms: 1.04x slower                                           |
| python_startup_no_site | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                           |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.29 ms: 1.04x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf1-amd64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 74.9 us: 4.35x faster                                           |
| generators                 | 34.0 ms                                                     | 20.6 ms: 1.65x faster                                           |
| asyncio_tcp                | 726 ms                                                      | 468 ms: 1.55x faster                                            |
| json_dumps                 | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                           |
| logging_silent             | 71.8 ns                                                     | 55.3 ns: 1.30x faster                                           |
| richards_super             | 38.7 ms                                                     | 30.5 ms: 1.27x faster                                           |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.62 sec: 1.25x faster                                          |
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                            |
| comprehensions             | 15.6 us                                                     | 12.7 us: 1.23x faster                                           |
| raytrace                   | 213 ms                                                      | 174 ms: 1.23x faster                                            |
| sqlglot_parse              | 953 us                                                      | 778 us: 1.23x faster                                            |
| unpack_sequence            | 46.9 ns                                                     | 39.1 ns: 1.20x faster                                           |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                            |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                            |
| sqlglot_transpile          | 1.16 ms                                                     | 1000 us: 1.17x faster                                           |
| richards                   | 31.4 ms                                                     | 27.0 ms: 1.16x faster                                           |
| coroutines                 | 15.0 ms                                                     | 12.9 ms: 1.16x faster                                           |
| sympy_sum                  | 100 ms                                                      | 86.6 ms: 1.16x faster                                           |
| unpickle_pure_python       | 157 us                                                      | 137 us: 1.15x faster                                            |
| pickle_pure_python         | 208 us                                                      | 182 us: 1.15x faster                                            |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                            |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.12x faster                                           |
| async_tree_none_tg         | 309 ms                                                      | 275 ms: 1.12x faster                                            |
| async_tree_io              | 808 ms                                                      | 722 ms: 1.12x faster                                            |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 469 ms: 1.12x faster                                            |
| sympy_str                  | 185 ms                                                      | 166 ms: 1.11x faster                                            |
| go                         | 101 ms                                                      | 90.8 ms: 1.11x faster                                           |
| async_tree_io_tg           | 829 ms                                                      | 748 ms: 1.11x faster                                            |
| scimark_lu                 | 62.8 ms                                                     | 56.9 ms: 1.10x faster                                           |
| logging_simple             | 6.86 us                                                     | 6.23 us: 1.10x faster                                           |
| chaos                      | 48.4 ms                                                     | 44.0 ms: 1.10x faster                                           |
| deepcopy_memo              | 26.0 us                                                     | 23.7 us: 1.09x faster                                           |
| dulwich_log                | 46.4 ms                                                     | 42.6 ms: 1.09x faster                                           |
| nqueens                    | 68.3 ms                                                     | 63.0 ms: 1.09x faster                                           |
| mypy2                      | 459 ms                                                      | 424 ms: 1.08x faster                                            |
| mdp                        | 1.59 sec                                                    | 1.47 sec: 1.08x faster                                          |
| regex_compile              | 91.0 ms                                                     | 84.2 ms: 1.08x faster                                           |
| sympy_integrate            | 14.0 ms                                                     | 13.1 ms: 1.07x faster                                           |
| deepcopy                   | 246 us                                                      | 230 us: 1.07x faster                                            |
| sympy_expand               | 299 ms                                                      | 279 ms: 1.07x faster                                            |
| logging_format             | 7.16 us                                                     | 6.70 us: 1.07x faster                                           |
| pycparser                  | 720 ms                                                      | 675 ms: 1.07x faster                                            |
| dask                       | 273 ms                                                      | 257 ms: 1.06x faster                                            |
| sqlglot_normalize          | 190 ms                                                      | 180 ms: 1.06x faster                                            |
| tornado_http               | 92.8 ms                                                     | 88.2 ms: 1.05x faster                                           |
| tomli_loads                | 1.46 sec                                                    | 1.38 sec: 1.05x faster                                          |
| mako                       | 7.58 ms                                                     | 7.29 ms: 1.04x faster                                           |
| deltablue                  | 2.70 ms                                                     | 2.60 ms: 1.04x faster                                           |
| xml_etree_parse            | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                           |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                          |
| chameleon                  | 5.26 ms                                                     | 5.10 ms: 1.03x faster                                           |
| crypto_pyaes               | 48.9 ms                                                     | 47.7 ms: 1.02x faster                                           |
| deepcopy_reduce            | 2.06 us                                                     | 2.02 us: 1.02x faster                                           |
| pidigits                   | 150 ms                                                      | 148 ms: 1.02x faster                                            |
| pprint_pformat             | 1.09 sec                                                    | 1.09 sec: 1.00x slower                                          |
| meteor_contest             | 75.2 ms                                                     | 76.2 ms: 1.01x slower                                           |
| 2to3                       | 214 ms                                                      | 217 ms: 1.02x slower                                            |
| pickle_dict                | 18.5 us                                                     | 18.8 us: 1.02x slower                                           |
| float                      | 54.4 ms                                                     | 55.5 ms: 1.02x slower                                           |
| scimark_sor                | 78.1 ms                                                     | 79.9 ms: 1.02x slower                                           |
| xml_etree_iterparse        | 65.6 ms                                                     | 67.5 ms: 1.03x slower                                           |
| create_gc_cycles           | 713 us                                                      | 738 us: 1.03x slower                                            |
| pyflate                    | 312 ms                                                      | 323 ms: 1.03x slower                                            |
| fannkuch                   | 253 ms                                                      | 264 ms: 1.04x slower                                            |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.04x slower                                           |
| python_startup             | 19.8 ms                                                     | 20.7 ms: 1.04x slower                                           |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                            |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.5 ms: 1.05x slower                                           |
| xml_etree_generate         | 52.5 ms                                                     | 55.2 ms: 1.05x slower                                           |
| unpickle_list              | 2.59 us                                                     | 2.73 us: 1.05x slower                                           |
| hexiom                     | 4.55 ms                                                     | 4.82 ms: 1.06x slower                                           |
| coverage                   | 43.4 ms                                                     | 46.0 ms: 1.06x slower                                           |
| bench_mp_pool              | 63.2 ms                                                     | 67.1 ms: 1.06x slower                                           |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                           |
| unpickle                   | 7.57 us                                                     | 8.21 us: 1.08x slower                                           |
| regex_v8                   | 14.2 ms                                                     | 15.5 ms: 1.10x slower                                           |
| python_startup_no_site     | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                           |
| pathlib                    | 70.9 ms                                                     | 78.3 ms: 1.10x slower                                           |
| pickle                     | 6.64 us                                                     | 7.37 us: 1.11x slower                                           |
| nbody                      | 70.3 ms                                                     | 79.2 ms: 1.13x slower                                           |
| scimark_fft                | 179 ms                                                      | 203 ms: 1.13x slower                                            |
| pickle_list                | 2.70 us                                                     | 3.08 us: 1.14x slower                                           |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.95 ms: 1.14x slower                                           |
| telco                      | 4.06 ms                                                     | 4.66 ms: 1.15x slower                                           |
| spectral_norm              | 68.3 ms                                                     | 79.9 ms: 1.17x slower                                           |
| json                       | 2.98 ms                                                     | 3.52 ms: 1.18x slower                                           |
| async_generators           | 177 ms                                                      | 227 ms: 1.28x slower                                            |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                    |

Benchmark hidden because not significant (5): bench_thread_pool, gc_traversal, pprint_safe_repr, sqlglot_optimize, xml_etree_process
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.87% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown