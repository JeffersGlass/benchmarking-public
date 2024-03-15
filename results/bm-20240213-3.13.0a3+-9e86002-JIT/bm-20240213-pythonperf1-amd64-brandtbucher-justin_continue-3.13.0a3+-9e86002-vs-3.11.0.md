
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_continue
- machine: windows-amd64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| chameleon      | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                        |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                       |
| tornado_http   | 92.8 ms                                                     | 84.9 ms: 1.09x faster                                                        |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                 |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                         |
| async_tree_memoization     | 399 ms                                                      | 334 ms: 1.19x faster                                                         |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 445 ms: 1.19x faster                                                         |
| async_tree_memoization_tg  | 405 ms                                                      | 340 ms: 1.19x faster                                                         |
| async_tree_none_tg         | 309 ms                                                      | 267 ms: 1.16x faster                                                         |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 463 ms: 1.13x faster                                                         |
| async_tree_io              | 808 ms                                                      | 720 ms: 1.12x faster                                                         |
| async_tree_io_tg           | 829 ms                                                      | 740 ms: 1.12x faster                                                         |
| Geometric mean             | (ref)                                                       | 1.17x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.5 ms: 1.18x faster                                                        |
| float          | 54.4 ms                                                     | 50.2 ms: 1.08x faster                                                        |
| pidigits       | 150 ms                                                      | 151 ms: 1.00x slower                                                         |
| Geometric mean | (ref)                                                       | 1.08x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 78.1 ms: 1.17x faster                                                        |
| regex_dna      | 116 ms                                                      | 120 ms: 1.04x slower                                                         |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.05x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.61 ms: 1.44x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 126 us: 1.24x faster                                                         |
| pickle_pure_python   | 208 us                                                      | 174 us: 1.20x faster                                                         |
| tomli_loads          | 1.46 sec                                                    | 1.26 sec: 1.16x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 17.5 us: 1.05x faster                                                        |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.4 ms: 1.03x faster                                                        |
| xml_etree_process    | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 94.4 ms: 1.03x faster                                                        |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.06x slower                                                        |
| unpickle_list        | 2.59 us                                                     | 2.79 us: 1.08x slower                                                        |
| pickle               | 6.64 us                                                     | 7.43 us: 1.12x slower                                                        |
| unpickle             | 7.57 us                                                     | 8.58 us: 1.13x slower                                                        |
| pickle_list          | 2.70 us                                                     | 3.09 us: 1.15x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.2 ms: 1.02x slower                                                        |
| python_startup_no_site | 16.8 ms                                                     | 18.1 ms: 1.08x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.15 ms: 1.23x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 68.8 us: 4.73x faster                                                        |
| generators                 | 34.0 ms                                                     | 19.9 ms: 1.71x faster                                                        |
| asyncio_tcp                | 726 ms                                                      | 468 ms: 1.55x faster                                                         |
| json_dumps                 | 8.09 ms                                                     | 5.61 ms: 1.44x faster                                                        |
| comprehensions             | 15.6 us                                                     | 11.1 us: 1.41x faster                                                        |
| deltablue                  | 2.70 ms                                                     | 1.96 ms: 1.37x faster                                                        |
| richards_super             | 38.7 ms                                                     | 28.2 ms: 1.37x faster                                                        |
| logging_silent             | 71.8 ns                                                     | 53.0 ns: 1.35x faster                                                        |
| raytrace                   | 213 ms                                                      | 167 ms: 1.27x faster                                                         |
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                         |
| sqlglot_parse              | 953 us                                                      | 755 us: 1.26x faster                                                         |
| richards                   | 31.4 ms                                                     | 25.0 ms: 1.26x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 126 us: 1.24x faster                                                         |
| mako                       | 7.58 ms                                                     | 6.15 ms: 1.23x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 21.2 us: 1.22x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 38.8 ns: 1.21x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 965 us: 1.21x faster                                                         |
| pickle_pure_python         | 208 us                                                      | 174 us: 1.20x faster                                                         |
| async_tree_memoization     | 399 ms                                                      | 334 ms: 1.19x faster                                                         |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 445 ms: 1.19x faster                                                         |
| async_tree_memoization_tg  | 405 ms                                                      | 340 ms: 1.19x faster                                                         |
| nbody                      | 70.3 ms                                                     | 59.5 ms: 1.18x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.72 sec: 1.18x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 53.4 ms: 1.18x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 78.1 ms: 1.17x faster                                                        |
| chaos                      | 48.4 ms                                                     | 41.6 ms: 1.16x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 58.8 ms: 1.16x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.52 us: 1.16x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 86.4 ms: 1.16x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 267 ms: 1.16x faster                                                         |
| tomli_loads                | 1.46 sec                                                    | 1.26 sec: 1.16x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 40.5 ms: 1.15x faster                                                        |
| deepcopy                   | 246 us                                                      | 216 us: 1.14x faster                                                         |
| logging_simple             | 6.86 us                                                     | 6.00 us: 1.14x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 59.9 ms: 1.14x faster                                                        |
| sympy_str                  | 185 ms                                                      | 163 ms: 1.14x faster                                                         |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 463 ms: 1.13x faster                                                         |
| pprint_pformat             | 1.09 sec                                                    | 967 ms: 1.12x faster                                                         |
| async_tree_io              | 808 ms                                                      | 720 ms: 1.12x faster                                                         |
| pprint_safe_repr           | 529 ms                                                      | 473 ms: 1.12x faster                                                         |
| async_tree_io_tg           | 829 ms                                                      | 740 ms: 1.12x faster                                                         |
| logging_format             | 7.16 us                                                     | 6.42 us: 1.12x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 172 ms: 1.10x faster                                                         |
| fannkuch                   | 253 ms                                                      | 230 ms: 1.10x faster                                                         |
| chameleon                  | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 84.9 ms: 1.09x faster                                                        |
| mypy2                      | 459 ms                                                      | 421 ms: 1.09x faster                                                         |
| crypto_pyaes               | 48.9 ms                                                     | 44.9 ms: 1.09x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 12.9 ms: 1.09x faster                                                        |
| float                      | 54.4 ms                                                     | 50.2 ms: 1.08x faster                                                        |
| sympy_expand               | 299 ms                                                      | 276 ms: 1.08x faster                                                         |
| bench_thread_pool          | 872 us                                                      | 808 us: 1.08x faster                                                         |
| pycparser                  | 720 ms                                                      | 671 ms: 1.07x faster                                                         |
| go                         | 101 ms                                                      | 94.3 ms: 1.07x faster                                                        |
| pyflate                    | 312 ms                                                      | 291 ms: 1.07x faster                                                         |
| dask                       | 273 ms                                                      | 255 ms: 1.07x faster                                                         |
| deepcopy_reduce            | 2.06 us                                                     | 1.95 us: 1.06x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 17.5 us: 1.05x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                       |
| scimark_sor                | 78.1 ms                                                     | 74.6 ms: 1.05x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.3 ms: 1.04x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.4 ms: 1.03x faster                                                        |
| xml_etree_process          | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 94.4 ms: 1.03x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.51 ms: 1.03x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.56 sec: 1.02x faster                                                       |
| meteor_contest             | 75.2 ms                                                     | 73.8 ms: 1.02x faster                                                        |
| pidigits                   | 150 ms                                                      | 151 ms: 1.00x slower                                                         |
| create_gc_cycles           | 713 us                                                      | 728 us: 1.02x slower                                                         |
| python_startup             | 19.8 ms                                                     | 20.2 ms: 1.02x slower                                                        |
| regex_dna                  | 116 ms                                                      | 120 ms: 1.04x slower                                                         |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.05x slower                                                        |
| bench_mp_pool              | 63.2 ms                                                     | 66.2 ms: 1.05x slower                                                        |
| scimark_fft                | 179 ms                                                      | 188 ms: 1.05x slower                                                         |
| coverage                   | 43.4 ms                                                     | 45.6 ms: 1.05x slower                                                        |
| hexiom                     | 4.55 ms                                                     | 4.82 ms: 1.06x slower                                                        |
| json_loads                 | 13.0 us                                                     | 13.8 us: 1.06x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                        |
| python_startup_no_site     | 16.8 ms                                                     | 18.1 ms: 1.08x slower                                                        |
| unpickle_list              | 2.59 us                                                     | 2.79 us: 1.08x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 76.9 ms: 1.09x slower                                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 49.2 ms: 1.09x slower                                                        |
| json                       | 2.98 ms                                                     | 3.26 ms: 1.09x slower                                                        |
| pickle                     | 6.64 us                                                     | 7.43 us: 1.12x slower                                                        |
| telco                      | 4.06 ms                                                     | 4.58 ms: 1.13x slower                                                        |
| unpickle                   | 7.57 us                                                     | 8.58 us: 1.13x slower                                                        |
| pickle_list                | 2.70 us                                                     | 3.09 us: 1.15x slower                                                        |
| async_generators           | 177 ms                                                      | 238 ms: 1.34x slower                                                         |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                 |

Benchmark hidden because not significant (3): gc_traversal, 2to3, xml_etree_generate
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown