
# Results vs. 3.11.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-amd64
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.09x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 210 ms: 1.02x faster                                                        |
| chameleon      | 5.26 ms                                                     | 4.81 ms: 1.09x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 85.8 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 275 ms: 1.21x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 465 ms: 1.14x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 353 ms: 1.13x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 359 ms: 1.13x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 279 ms: 1.11x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 477 ms: 1.10x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 769 ms: 1.08x faster                                                        |
| async_tree_io              | 808 ms                                                      | 751 ms: 1.08x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 53.5 ms: 1.02x faster                                                       |
| pidigits       | 150 ms                                                      | 149 ms: 1.00x faster                                                        |
| nbody          | 70.3 ms                                                     | 72.3 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 76.9 ms: 1.18x faster                                                       |
| regex_dna      | 116 ms                                                      | 118 ms: 1.02x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.06x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 17.1 ms: 1.20x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.63 ms: 1.44x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 130 us: 1.20x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 185 us: 1.13x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.43 sec: 1.01x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 37.0 ms: 1.01x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.6 us: 1.01x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.9 ms: 1.03x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.75 us: 1.06x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.88 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.25 us: 1.09x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.68 us: 1.15x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.65 ms: 1.14x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 73.1 us: 4.46x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.3 ms: 1.60x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 491 ms: 1.48x faster                                                        |
| comprehensions             | 15.6 us                                                     | 10.9 us: 1.44x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.63 ms: 1.44x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.01 ms: 1.34x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.5 ns: 1.29x faster                                                       |
| raytrace                   | 213 ms                                                      | 166 ms: 1.29x faster                                                        |
| richards_super             | 38.7 ms                                                     | 31.0 ms: 1.25x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 37.6 ns: 1.25x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 778 us: 1.22x faster                                                        |
| chaos                      | 48.4 ms                                                     | 39.6 ms: 1.22x faster                                                       |
| async_tree_none            | 332 ms                                                      | 275 ms: 1.21x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 83.1 ms: 1.21x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 130 us: 1.20x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 981 us: 1.19x faster                                                        |
| hexiom                     | 4.55 ms                                                     | 3.84 ms: 1.18x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 76.9 ms: 1.18x faster                                                       |
| go                         | 101 ms                                                      | 85.5 ms: 1.18x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 53.8 ms: 1.17x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 42.3 ms: 1.16x faster                                                       |
| sympy_str                  | 185 ms                                                      | 161 ms: 1.15x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 22.6 us: 1.15x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.65 ms: 1.14x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 465 ms: 1.14x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 60.2 ms: 1.13x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 12.4 ms: 1.13x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 353 ms: 1.13x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 359 ms: 1.13x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 185 us: 1.13x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.42 sec: 1.12x faster                                                      |
| richards                   | 31.4 ms                                                     | 28.0 ms: 1.12x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 41.4 ms: 1.12x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.4 ms: 1.12x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.16 us: 1.11x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.46 us: 1.11x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 279 ms: 1.11x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 61.8 ms: 1.11x faster                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 41.0 ms: 1.10x faster                                                       |
| mypy2                      | 459 ms                                                      | 419 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 477 ms: 1.10x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.81 ms: 1.09x faster                                                       |
| deepcopy                   | 246 us                                                      | 226 us: 1.09x faster                                                        |
| sympy_expand               | 299 ms                                                      | 276 ms: 1.08x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 85.8 ms: 1.08x faster                                                       |
| fannkuch                   | 253 ms                                                      | 235 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 769 ms: 1.08x faster                                                        |
| async_tree_io              | 808 ms                                                      | 751 ms: 1.08x faster                                                        |
| pyflate                    | 312 ms                                                      | 293 ms: 1.07x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 179 ms: 1.06x faster                                                        |
| dask                       | 273 ms                                                      | 259 ms: 1.05x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.45 ms: 1.05x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.93 sec: 1.05x faster                                                      |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| deepcopy_reduce            | 2.06 us                                                     | 1.97 us: 1.04x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.04 sec: 1.04x faster                                                      |
| sqlglot_optimize           | 34.5 ms                                                     | 33.2 ms: 1.04x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 512 ms: 1.03x faster                                                        |
| meteor_contest             | 75.2 ms                                                     | 73.7 ms: 1.02x faster                                                       |
| 2to3                       | 214 ms                                                      | 210 ms: 1.02x faster                                                        |
| float                      | 54.4 ms                                                     | 53.5 ms: 1.02x faster                                                       |
| scimark_fft                | 179 ms                                                      | 177 ms: 1.02x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.43 sec: 1.01x faster                                                      |
| scimark_sor                | 78.1 ms                                                     | 77.4 ms: 1.01x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 37.0 ms: 1.01x faster                                                       |
| pidigits                   | 150 ms                                                      | 149 ms: 1.00x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 18.6 us: 1.01x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.52 ms: 1.02x slower                                                       |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.02x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 53.9 ms: 1.03x slower                                                       |
| nbody                      | 70.3 ms                                                     | 72.3 ms: 1.03x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.5 us: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.06x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.75 us: 1.06x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.2 ms: 1.06x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 760 us: 1.07x slower                                                        |
| pickle_list                | 2.70 us                                                     | 2.88 us: 1.07x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 67.9 ms: 1.07x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.25 us: 1.09x slower                                                       |
| json                       | 2.98 ms                                                     | 3.39 ms: 1.14x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 81.0 ms: 1.14x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.68 us: 1.15x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.71 ms: 1.16x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 17.1 ms: 1.20x slower                                                       |
| async_generators           | 177 ms                                                      | 235 ms: 1.33x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.09x faster                                                                |

Benchmark hidden because not significant (3): pycparser, bench_thread_pool, xml_etree_iterparse
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown