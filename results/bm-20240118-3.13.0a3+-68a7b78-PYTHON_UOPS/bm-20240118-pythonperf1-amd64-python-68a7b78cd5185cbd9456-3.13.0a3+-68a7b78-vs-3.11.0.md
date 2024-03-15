
# Results vs. 3.11.0

- fork: python
- ref: 68a7b78cd5185cbd9456
- machine: windows-amd64
- commit hash: 68a7b78
- commit date: 2024-01-18
- overall geometric mean: 1.06x faster
- HPT reliability: 99.95%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.90 ms: 1.07x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 88.2 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.17x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 350 ms: 1.16x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 747 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 728 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| float          | 54.4 ms                                                     | 56.6 ms: 1.04x slower                                                       |
| nbody          | 70.3 ms                                                     | 83.1 ms: 1.18x slower                                                       |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.8 ms: 1.07x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 176 us: 1.19x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 133 us: 1.18x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.6 ms: 1.05x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 37.7 ms: 1.01x slower                                                       |
| pickle_dict          | 18.5 us                                                     | 18.8 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 67.0 ms: 1.02x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.4 us: 1.03x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 55.5 ms: 1.06x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.75 us: 1.06x slower                                                       |
| pickle               | 6.64 us                                                     | 7.30 us: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.40 us: 1.11x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.28 us: 1.22x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.2 ms: 1.08x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.66 ms: 1.01x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 74.0 us: 4.41x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.9 ms: 1.55x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 474 ms: 1.53x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.2 ns: 1.30x faster                                                       |
| richards_super             | 38.7 ms                                                     | 30.3 ms: 1.28x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.62 sec: 1.25x faster                                                      |
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 771 us: 1.24x faster                                                        |
| raytrace                   | 213 ms                                                      | 174 ms: 1.23x faster                                                        |
| comprehensions             | 15.6 us                                                     | 12.9 us: 1.21x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 39.1 ns: 1.20x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 176 us: 1.19x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 133 us: 1.18x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 994 us: 1.17x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.17x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 22.4 us: 1.16x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.1 ms: 1.16x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 350 ms: 1.16x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 54.4 ms: 1.16x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 87.9 ms: 1.14x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| go                         | 101 ms                                                      | 90.4 ms: 1.12x faster                                                       |
| sympy_str                  | 185 ms                                                      | 166 ms: 1.12x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.4 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 747 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 728 ms: 1.11x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.44 sec: 1.11x faster                                                      |
| deepcopy                   | 246 us                                                      | 224 us: 1.10x faster                                                        |
| chaos                      | 48.4 ms                                                     | 44.1 ms: 1.10x faster                                                       |
| mypy2                      | 459 ms                                                      | 421 ms: 1.09x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 42.6 ms: 1.09x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.32 us: 1.09x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.0 ms: 1.08x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.90 ms: 1.07x faster                                                       |
| sympy_expand               | 299 ms                                                      | 278 ms: 1.07x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 84.8 ms: 1.07x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.69 us: 1.07x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 64.5 ms: 1.06x faster                                                       |
| dask                       | 273 ms                                                      | 258 ms: 1.06x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.6 ms: 1.05x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 88.2 ms: 1.05x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 181 ms: 1.05x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                      |
| bench_thread_pool          | 872 us                                                      | 845 us: 1.03x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 2.00 us: 1.03x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 517 ms: 1.02x faster                                                        |
| scimark_sor                | 78.1 ms                                                     | 76.3 ms: 1.02x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.07 sec: 1.02x faster                                                      |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                      |
| gc_traversal               | 1.49 ms                                                     | 1.48 ms: 1.01x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 48.7 ms: 1.00x faster                                                       |
| mako                       | 7.58 ms                                                     | 7.66 ms: 1.01x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 37.7 ms: 1.01x slower                                                       |
| pickle_dict                | 18.5 us                                                     | 18.8 us: 1.01x slower                                                       |
| meteor_contest             | 75.2 ms                                                     | 76.7 ms: 1.02x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 67.0 ms: 1.02x slower                                                       |
| 2to3                       | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 735 us: 1.03x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.4 us: 1.03x slower                                                       |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| python_startup             | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| pyflate                    | 312 ms                                                      | 324 ms: 1.04x slower                                                        |
| float                      | 54.4 ms                                                     | 56.6 ms: 1.04x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.8 ms: 1.05x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 55.5 ms: 1.06x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.75 us: 1.06x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 67.2 ms: 1.06x slower                                                       |
| fannkuch                   | 253 ms                                                      | 272 ms: 1.07x slower                                                        |
| hexiom                     | 4.55 ms                                                     | 4.92 ms: 1.08x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.2 ms: 1.08x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.1 ms: 1.08x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.30 us: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.40 us: 1.11x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 79.1 ms: 1.12x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.65 ms: 1.14x slower                                                       |
| nbody                      | 70.3 ms                                                     | 83.1 ms: 1.18x slower                                                       |
| scimark_fft                | 179 ms                                                      | 215 ms: 1.20x slower                                                        |
| pickle_list                | 2.70 us                                                     | 3.28 us: 1.22x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 85.2 ms: 1.25x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.29 ms: 1.28x slower                                                       |
| async_generators           | 177 ms                                                      | 232 ms: 1.31x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (4): json, pycparser, deltablue, sqlglot_optimize
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.95% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown