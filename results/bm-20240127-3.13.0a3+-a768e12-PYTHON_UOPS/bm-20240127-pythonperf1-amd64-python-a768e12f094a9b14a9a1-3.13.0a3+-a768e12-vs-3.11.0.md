
# Results vs. 3.11.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-amd64
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.05x faster
- HPT reliability: 99.46%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 222 ms: 1.04x slower                                                        |
| chameleon      | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 86.8 ms: 1.07x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 278 ms: 1.20x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 457 ms: 1.16x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 354 ms: 1.13x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 283 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                                        |
| async_tree_io              | 808 ms                                                      | 750 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                                       |
| nbody          | 70.3 ms                                                     | 83.1 ms: 1.18x slower                                                       |
| Geometric mean | (ref)                                                       | 1.08x slower                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 85.2 ms: 1.07x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 137 us: 1.15x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 182 us: 1.14x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.8 us: 1.02x slower                                                       |
| xml_etree_process    | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 68.0 ms: 1.04x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 56.2 ms: 1.07x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.89 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.20 us: 1.09x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.85 us: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.52 us: 1.12x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.4 ms: 1.10x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.38 ms: 1.03x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 75.6 us: 4.31x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.0 ms: 1.62x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 478 ms: 1.52x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 54.1 ns: 1.33x faster                                                       |
| richards_super             | 38.7 ms                                                     | 30.4 ms: 1.28x faster                                                       |
| raytrace                   | 213 ms                                                      | 170 ms: 1.25x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 789 us: 1.21x faster                                                        |
| comprehensions             | 15.6 us                                                     | 13.0 us: 1.20x faster                                                       |
| async_tree_none            | 332 ms                                                      | 278 ms: 1.20x faster                                                        |
| richards                   | 31.4 ms                                                     | 26.8 ms: 1.17x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 457 ms: 1.16x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 137 us: 1.15x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.1 ms: 1.15x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 182 us: 1.14x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 354 ms: 1.13x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 89.6 ms: 1.12x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 42.1 ns: 1.11x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 23.4 us: 1.11x faster                                                       |
| go                         | 101 ms                                                      | 91.5 ms: 1.10x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.22 us: 1.10x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.86 sec: 1.09x faster                                                      |
| async_tree_none_tg         | 309 ms                                                      | 283 ms: 1.09x faster                                                        |
| chaos                      | 48.4 ms                                                     | 44.4 ms: 1.09x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                                        |
| sympy_str                  | 185 ms                                                      | 170 ms: 1.09x faster                                                        |
| deepcopy                   | 246 us                                                      | 229 us: 1.08x faster                                                        |
| async_tree_io              | 808 ms                                                      | 750 ms: 1.08x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 63.5 ms: 1.08x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 86.8 ms: 1.07x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 58.8 ms: 1.07x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 85.2 ms: 1.07x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.73 us: 1.06x faster                                                       |
| mypy2                      | 459 ms                                                      | 432 ms: 1.06x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 43.7 ms: 1.06x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.05x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                       |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.53 sec: 1.04x faster                                                      |
| deltablue                  | 2.70 ms                                                     | 2.59 ms: 1.04x faster                                                       |
| dask                       | 273 ms                                                      | 263 ms: 1.04x faster                                                        |
| mako                       | 7.58 ms                                                     | 7.38 ms: 1.03x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                                      |
| deepcopy_reduce            | 2.06 us                                                     | 2.01 us: 1.02x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                      |
| sqlglot_normalize          | 190 ms                                                      | 189 ms: 1.00x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.09 sec: 1.01x slower                                                      |
| scimark_sor                | 78.1 ms                                                     | 78.7 ms: 1.01x slower                                                       |
| pickle_dict                | 18.5 us                                                     | 18.8 us: 1.02x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.52 ms: 1.02x slower                                                       |
| bench_thread_pool          | 872 us                                                      | 888 us: 1.02x slower                                                        |
| xml_etree_process          | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                       |
| meteor_contest             | 75.2 ms                                                     | 77.5 ms: 1.03x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.7 ms: 1.03x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 68.0 ms: 1.04x slower                                                       |
| 2to3                       | 214 ms                                                      | 222 ms: 1.04x slower                                                        |
| pyflate                    | 312 ms                                                      | 325 ms: 1.04x slower                                                        |
| python_startup             | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 750 us: 1.05x slower                                                        |
| fannkuch                   | 253 ms                                                      | 266 ms: 1.05x slower                                                        |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| float                      | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.7 ms: 1.05x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 4.80 ms: 1.05x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.3 ms: 1.07x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 56.2 ms: 1.07x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.89 us: 1.07x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 68.4 ms: 1.08x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.20 us: 1.09x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.4 ms: 1.10x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.85 us: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.52 us: 1.12x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 80.2 ms: 1.13x slower                                                       |
| scimark_fft                | 179 ms                                                      | 205 ms: 1.15x slower                                                        |
| telco                      | 4.06 ms                                                     | 4.75 ms: 1.17x slower                                                       |
| nbody                      | 70.3 ms                                                     | 83.1 ms: 1.18x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 80.9 ms: 1.18x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.07 ms: 1.19x slower                                                       |
| async_generators           | 177 ms                                                      | 231 ms: 1.31x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (5): json, pycparser, crypto_pyaes, pprint_safe_repr, pidigits
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.46% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown