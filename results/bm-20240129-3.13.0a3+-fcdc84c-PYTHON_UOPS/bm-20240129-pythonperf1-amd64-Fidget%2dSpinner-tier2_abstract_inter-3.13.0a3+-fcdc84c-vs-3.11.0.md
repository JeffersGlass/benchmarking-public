
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.05x faster
- HPT reliability: 99.81%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 224 ms: 1.05x slower                                                                  |
| chameleon      | 5.26 ms                                                     | 5.05 ms: 1.04x faster                                                                 |
| docutils       | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                                |
| tornado_http   | 92.8 ms                                                     | 88.1 ms: 1.05x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 276 ms: 1.20x faster                                                                  |
| async_tree_memoization     | 399 ms                                                      | 355 ms: 1.12x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 473 ms: 1.12x faster                                                                  |
| async_tree_memoization_tg  | 405 ms                                                      | 366 ms: 1.11x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                                                  |
| async_tree_none_tg         | 309 ms                                                      | 284 ms: 1.09x faster                                                                  |
| async_tree_io_tg           | 829 ms                                                      | 770 ms: 1.08x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 756 ms: 1.07x faster                                                                  |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.02x faster                                                                  |
| float          | 54.4 ms                                                     | 56.6 ms: 1.04x slower                                                                 |
| nbody          | 70.3 ms                                                     | 76.8 ms: 1.09x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.6 ms: 1.08x faster                                                                 |
| regex_dna      | 116 ms                                                      | 123 ms: 1.06x slower                                                                  |
| regex_effbot   | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                                                 |
| regex_v8       | 14.2 ms                                                     | 15.7 ms: 1.11x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.76 ms: 1.40x faster                                                                 |
| unpickle_pure_python | 157 us                                                      | 135 us: 1.16x faster                                                                  |
| pickle_pure_python   | 208 us                                                      | 181 us: 1.15x faster                                                                  |
| xml_etree_parse      | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                                 |
| tomli_loads          | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                                |
| pickle_dict          | 18.5 us                                                     | 18.8 us: 1.01x slower                                                                 |
| xml_etree_process    | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                                                 |
| xml_etree_iterparse  | 65.6 ms                                                     | 68.4 ms: 1.04x slower                                                                 |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                                 |
| xml_etree_generate   | 52.5 ms                                                     | 55.6 ms: 1.06x slower                                                                 |
| unpickle_list        | 2.59 us                                                     | 2.78 us: 1.07x slower                                                                 |
| pickle_list          | 2.70 us                                                     | 2.99 us: 1.11x slower                                                                 |
| pickle               | 6.64 us                                                     | 7.37 us: 1.11x slower                                                                 |
| unpickle             | 7.57 us                                                     | 8.48 us: 1.12x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                                                 |
| python_startup_no_site | 16.8 ms                                                     | 18.8 ms: 1.12x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                          |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 75.3 us: 4.33x faster                                                                 |
| generators                 | 34.0 ms                                                     | 22.0 ms: 1.55x faster                                                                 |
| asyncio_tcp                | 726 ms                                                      | 495 ms: 1.47x faster                                                                  |
| json_dumps                 | 8.09 ms                                                     | 5.76 ms: 1.40x faster                                                                 |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.52 sec: 1.33x faster                                                                |
| logging_silent             | 71.8 ns                                                     | 55.2 ns: 1.30x faster                                                                 |
| richards_super             | 38.7 ms                                                     | 30.6 ms: 1.27x faster                                                                 |
| raytrace                   | 213 ms                                                      | 174 ms: 1.23x faster                                                                  |
| comprehensions             | 15.6 us                                                     | 12.8 us: 1.22x faster                                                                 |
| sqlglot_parse              | 953 us                                                      | 787 us: 1.21x faster                                                                  |
| unpack_sequence            | 46.9 ns                                                     | 39.0 ns: 1.20x faster                                                                 |
| async_tree_none            | 332 ms                                                      | 276 ms: 1.20x faster                                                                  |
| unpickle_pure_python       | 157 us                                                      | 135 us: 1.16x faster                                                                  |
| pickle_pure_python         | 208 us                                                      | 181 us: 1.15x faster                                                                  |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                                 |
| richards                   | 31.4 ms                                                     | 27.3 ms: 1.15x faster                                                                 |
| sqlglot_transpile          | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                                                 |
| sympy_sum                  | 100 ms                                                      | 89.1 ms: 1.12x faster                                                                 |
| chaos                      | 48.4 ms                                                     | 43.1 ms: 1.12x faster                                                                 |
| async_tree_memoization     | 399 ms                                                      | 355 ms: 1.12x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 473 ms: 1.12x faster                                                                  |
| sympy_str                  | 185 ms                                                      | 166 ms: 1.11x faster                                                                  |
| mdp                        | 1.59 sec                                                    | 1.43 sec: 1.11x faster                                                                |
| sqlite_synth               | 1.77 us                                                     | 1.59 us: 1.11x faster                                                                 |
| logging_simple             | 6.86 us                                                     | 6.20 us: 1.11x faster                                                                 |
| async_tree_memoization_tg  | 405 ms                                                      | 366 ms: 1.11x faster                                                                  |
| deepcopy_memo              | 26.0 us                                                     | 23.7 us: 1.09x faster                                                                 |
| deepcopy                   | 246 us                                                      | 226 us: 1.09x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                                                  |
| go                         | 101 ms                                                      | 93.0 ms: 1.09x faster                                                                 |
| async_tree_none_tg         | 309 ms                                                      | 284 ms: 1.09x faster                                                                  |
| scimark_lu                 | 62.8 ms                                                     | 57.9 ms: 1.08x faster                                                                 |
| async_tree_io_tg           | 829 ms                                                      | 770 ms: 1.08x faster                                                                  |
| regex_compile              | 91.0 ms                                                     | 84.6 ms: 1.08x faster                                                                 |
| logging_format             | 7.16 us                                                     | 6.66 us: 1.08x faster                                                                 |
| dulwich_log                | 46.4 ms                                                     | 43.2 ms: 1.07x faster                                                                 |
| async_tree_io              | 808 ms                                                      | 756 ms: 1.07x faster                                                                  |
| nqueens                    | 68.3 ms                                                     | 64.7 ms: 1.06x faster                                                                 |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.05x faster                                                                 |
| tornado_http               | 92.8 ms                                                     | 88.1 ms: 1.05x faster                                                                 |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                                                  |
| mypy2                      | 459 ms                                                      | 437 ms: 1.05x faster                                                                  |
| pycparser                  | 720 ms                                                      | 687 ms: 1.05x faster                                                                  |
| chameleon                  | 5.26 ms                                                     | 5.05 ms: 1.04x faster                                                                 |
| xml_etree_parse            | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                                 |
| deepcopy_reduce            | 2.06 us                                                     | 2.00 us: 1.03x faster                                                                 |
| dask                       | 273 ms                                                      | 265 ms: 1.03x faster                                                                  |
| sqlglot_normalize          | 190 ms                                                      | 186 ms: 1.02x faster                                                                  |
| tomli_loads                | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                                |
| deltablue                  | 2.70 ms                                                     | 2.65 ms: 1.02x faster                                                                 |
| docutils                   | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                                |
| pprint_pformat             | 1.09 sec                                                    | 1.07 sec: 1.02x faster                                                                |
| pidigits                   | 150 ms                                                      | 148 ms: 1.02x faster                                                                  |
| crypto_pyaes               | 48.9 ms                                                     | 48.1 ms: 1.02x faster                                                                 |
| pprint_safe_repr           | 529 ms                                                      | 523 ms: 1.01x faster                                                                  |
| scimark_sor                | 78.1 ms                                                     | 79.0 ms: 1.01x slower                                                                 |
| pickle_dict                | 18.5 us                                                     | 18.8 us: 1.01x slower                                                                 |
| gc_traversal               | 1.49 ms                                                     | 1.52 ms: 1.02x slower                                                                 |
| xml_etree_process          | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                                                 |
| meteor_contest             | 75.2 ms                                                     | 76.5 ms: 1.02x slower                                                                 |
| pyflate                    | 312 ms                                                      | 322 ms: 1.03x slower                                                                  |
| create_gc_cycles           | 713 us                                                      | 737 us: 1.03x slower                                                                  |
| sqlglot_optimize           | 34.5 ms                                                     | 35.7 ms: 1.03x slower                                                                 |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.0 ms: 1.04x slower                                                                 |
| float                      | 54.4 ms                                                     | 56.6 ms: 1.04x slower                                                                 |
| xml_etree_iterparse        | 65.6 ms                                                     | 68.4 ms: 1.04x slower                                                                 |
| 2to3                       | 214 ms                                                      | 224 ms: 1.05x slower                                                                  |
| python_startup             | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                                                 |
| regex_dna                  | 116 ms                                                      | 123 ms: 1.06x slower                                                                  |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                                                 |
| xml_etree_generate         | 52.5 ms                                                     | 55.6 ms: 1.06x slower                                                                 |
| fannkuch                   | 253 ms                                                      | 269 ms: 1.06x slower                                                                  |
| regex_effbot               | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                                                 |
| unpickle_list              | 2.59 us                                                     | 2.78 us: 1.07x slower                                                                 |
| hexiom                     | 4.55 ms                                                     | 4.90 ms: 1.08x slower                                                                 |
| scimark_fft                | 179 ms                                                      | 195 ms: 1.09x slower                                                                  |
| nbody                      | 70.3 ms                                                     | 76.8 ms: 1.09x slower                                                                 |
| bench_mp_pool              | 63.2 ms                                                     | 69.2 ms: 1.09x slower                                                                 |
| coverage                   | 43.4 ms                                                     | 47.7 ms: 1.10x slower                                                                 |
| regex_v8                   | 14.2 ms                                                     | 15.7 ms: 1.11x slower                                                                 |
| pickle_list                | 2.70 us                                                     | 2.99 us: 1.11x slower                                                                 |
| pickle                     | 6.64 us                                                     | 7.37 us: 1.11x slower                                                                 |
| python_startup_no_site     | 16.8 ms                                                     | 18.8 ms: 1.12x slower                                                                 |
| unpickle                   | 7.57 us                                                     | 8.48 us: 1.12x slower                                                                 |
| telco                      | 4.06 ms                                                     | 4.64 ms: 1.14x slower                                                                 |
| pathlib                    | 70.9 ms                                                     | 81.1 ms: 1.14x slower                                                                 |
| spectral_norm              | 68.3 ms                                                     | 80.1 ms: 1.17x slower                                                                 |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.02 ms: 1.17x slower                                                                 |
| async_generators           | 177 ms                                                      | 228 ms: 1.29x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                          |

Benchmark hidden because not significant (3): mako, bench_thread_pool, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.81% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown