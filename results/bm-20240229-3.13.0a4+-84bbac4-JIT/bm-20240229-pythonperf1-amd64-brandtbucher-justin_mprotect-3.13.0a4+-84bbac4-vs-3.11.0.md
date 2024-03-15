# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-amd64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.04x slower                                                         |
| chameleon      | 5.26 ms                                                     | 4.78 ms: 1.10x faster                                                        |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                       |
| tornado_http   | 92.8 ms                                                     | 85.0 ms: 1.09x faster                                                        |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 267 ms: 1.25x faster                                                         |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                         |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                                         |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                         |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                         |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 464 ms: 1.13x faster                                                         |
| async_tree_io              | 808 ms                                                      | 725 ms: 1.11x faster                                                         |
| async_tree_io_tg           | 829 ms                                                      | 759 ms: 1.09x faster                                                         |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 57.7 ms: 1.22x faster                                                        |
| float          | 54.4 ms                                                     | 49.1 ms: 1.11x faster                                                        |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 82.2 ms: 1.11x faster                                                        |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                         |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.52 ms: 1.47x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 127 us: 1.23x faster                                                         |
| tomli_loads          | 1.46 sec                                                    | 1.19 sec: 1.23x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                                         |
| pickle_dict          | 18.5 us                                                     | 17.3 us: 1.07x faster                                                        |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.1 ms: 1.06x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                        |
| xml_etree_process    | 37.2 ms                                                     | 35.8 ms: 1.04x faster                                                        |
| json_loads           | 13.0 us                                                     | 14.0 us: 1.07x slower                                                        |
| pickle_list          | 2.70 us                                                     | 2.90 us: 1.08x slower                                                        |
| unpickle_list        | 2.59 us                                                     | 2.79 us: 1.08x slower                                                        |
| pickle               | 6.64 us                                                     | 7.16 us: 1.08x slower                                                        |
| unpickle             | 7.57 us                                                     | 8.68 us: 1.15x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.06x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 23.8 ms: 1.20x slower                                                        |
| python_startup_no_site | 16.8 ms                                                     | 21.5 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.24x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 5.66 ms: 1.34x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.4 us: 4.63x faster                                                        |
| generators                 | 34.0 ms                                                     | 20.4 ms: 1.67x faster                                                        |
| asyncio_tcp                | 726 ms                                                      | 471 ms: 1.54x faster                                                         |
| comprehensions             | 15.6 us                                                     | 10.6 us: 1.48x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.52 ms: 1.47x faster                                                        |
| mako                       | 7.58 ms                                                     | 5.66 ms: 1.34x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 51.0 ms: 1.34x faster                                                        |
| logging_silent             | 71.8 ns                                                     | 55.8 ns: 1.29x faster                                                        |
| deltablue                  | 2.70 ms                                                     | 2.13 ms: 1.26x faster                                                        |
| async_tree_none            | 332 ms                                                      | 267 ms: 1.25x faster                                                         |
| richards_super             | 38.7 ms                                                     | 31.2 ms: 1.24x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 127 us: 1.23x faster                                                         |
| sqlglot_parse              | 953 us                                                      | 774 us: 1.23x faster                                                         |
| tomli_loads                | 1.46 sec                                                    | 1.19 sec: 1.23x faster                                                       |
| chaos                      | 48.4 ms                                                     | 39.6 ms: 1.22x faster                                                        |
| nbody                      | 70.3 ms                                                     | 57.7 ms: 1.22x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                                         |
| deepcopy_memo              | 26.0 us                                                     | 21.9 us: 1.19x faster                                                        |
| raytrace                   | 213 ms                                                      | 180 ms: 1.18x faster                                                         |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                         |
| sqlglot_transpile          | 1.16 ms                                                     | 994 us: 1.17x faster                                                         |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                                         |
| logging_simple             | 6.86 us                                                     | 5.88 us: 1.17x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 86.0 ms: 1.16x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.38 sec: 1.15x faster                                                       |
| fannkuch                   | 253 ms                                                      | 220 ms: 1.15x faster                                                         |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                         |
| crypto_pyaes               | 48.9 ms                                                     | 42.7 ms: 1.14x faster                                                        |
| sympy_str                  | 185 ms                                                      | 162 ms: 1.14x faster                                                         |
| logging_format             | 7.16 us                                                     | 6.28 us: 1.14x faster                                                        |
| deepcopy                   | 246 us                                                      | 217 us: 1.14x faster                                                         |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                         |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.27 ms: 1.13x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.79 sec: 1.13x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 468 ms: 1.13x faster                                                         |
| richards                   | 31.4 ms                                                     | 27.8 ms: 1.13x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 962 ms: 1.13x faster                                                         |
| dulwich_log                | 46.4 ms                                                     | 41.1 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 464 ms: 1.13x faster                                                         |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.4 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 725 ms: 1.11x faster                                                         |
| nqueens                    | 68.3 ms                                                     | 61.4 ms: 1.11x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 82.2 ms: 1.11x faster                                                        |
| float                      | 54.4 ms                                                     | 49.1 ms: 1.11x faster                                                        |
| pyflate                    | 312 ms                                                      | 283 ms: 1.10x faster                                                         |
| chameleon                  | 5.26 ms                                                     | 4.78 ms: 1.10x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 174 ms: 1.09x faster                                                         |
| tornado_http               | 92.8 ms                                                     | 85.0 ms: 1.09x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 759 ms: 1.09x faster                                                         |
| scimark_monte_carlo        | 45.3 ms                                                     | 41.7 ms: 1.09x faster                                                        |
| sympy_expand               | 299 ms                                                      | 275 ms: 1.09x faster                                                         |
| sympy_integrate            | 14.0 ms                                                     | 13.1 ms: 1.07x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.93 us: 1.07x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 17.3 us: 1.07x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 821 us: 1.06x faster                                                         |
| scimark_fft                | 179 ms                                                      | 169 ms: 1.06x faster                                                         |
| xml_etree_iterparse        | 65.6 ms                                                     | 62.1 ms: 1.06x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                        |
| mypy2                      | 459 ms                                                      | 438 ms: 1.05x faster                                                         |
| hexiom                     | 4.55 ms                                                     | 4.37 ms: 1.04x faster                                                        |
| xml_etree_process          | 37.2 ms                                                     | 35.8 ms: 1.04x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                       |
| go                         | 101 ms                                                      | 98.4 ms: 1.03x faster                                                        |
| meteor_contest             | 75.2 ms                                                     | 73.4 ms: 1.03x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 34.2 ms: 1.01x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 46.6 ns: 1.01x faster                                                        |
| gc_traversal               | 1.49 ms                                                     | 1.53 ms: 1.02x slower                                                        |
| scimark_sor                | 78.1 ms                                                     | 80.6 ms: 1.03x slower                                                        |
| 2to3                       | 214 ms                                                      | 223 ms: 1.04x slower                                                         |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                         |
| create_gc_cycles           | 713 us                                                      | 748 us: 1.05x slower                                                         |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 75.0 ms: 1.06x slower                                                        |
| coverage                   | 43.4 ms                                                     | 46.4 ms: 1.07x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                        |
| json_loads                 | 13.0 us                                                     | 14.0 us: 1.07x slower                                                        |
| pickle_list                | 2.70 us                                                     | 2.90 us: 1.08x slower                                                        |
| unpickle_list              | 2.59 us                                                     | 2.79 us: 1.08x slower                                                        |
| pickle                     | 6.64 us                                                     | 7.16 us: 1.08x slower                                                        |
| json                       | 2.98 ms                                                     | 3.22 ms: 1.08x slower                                                        |
| bench_mp_pool              | 63.2 ms                                                     | 69.8 ms: 1.10x slower                                                        |
| scimark_lu                 | 62.8 ms                                                     | 70.4 ms: 1.12x slower                                                        |
| telco                      | 4.06 ms                                                     | 4.66 ms: 1.15x slower                                                        |
| unpickle                   | 7.57 us                                                     | 8.68 us: 1.15x slower                                                        |
| python_startup             | 19.8 ms                                                     | 23.8 ms: 1.20x slower                                                        |
| python_startup_no_site     | 16.8 ms                                                     | 21.5 ms: 1.28x slower                                                        |
| dask                       | 273 ms                                                      | 360 ms: 1.32x slower                                                         |
| async_generators           | 177 ms                                                      | 240 ms: 1.36x slower                                                         |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                 |

Benchmark hidden because not significant (3): pidigits, xml_etree_generate, pycparser
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown