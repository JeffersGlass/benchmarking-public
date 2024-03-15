
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.06x faster
- HPT reliability: 99.93%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.04x slower                                                                  |
| chameleon      | 5.26 ms                                                     | 5.03 ms: 1.05x faster                                                                 |
| docutils       | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                                |
| tornado_http   | 92.8 ms                                                     | 88.5 ms: 1.05x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 271 ms: 1.23x faster                                                                  |
| async_tree_memoization     | 399 ms                                                      | 344 ms: 1.16x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 457 ms: 1.16x faster                                                                  |
| async_tree_memoization_tg  | 405 ms                                                      | 351 ms: 1.15x faster                                                                  |
| async_tree_io_tg           | 829 ms                                                      | 738 ms: 1.12x faster                                                                  |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 722 ms: 1.12x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 470 ms: 1.11x faster                                                                  |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.02x faster                                                                  |
| float          | 54.4 ms                                                     | 56.6 ms: 1.04x slower                                                                 |
| nbody          | 70.3 ms                                                     | 81.4 ms: 1.16x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.06x slower                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.4 ms: 1.08x faster                                                                 |
| regex_dna      | 116 ms                                                      | 118 ms: 1.01x slower                                                                  |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                                 |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                                                 |
| pickle_pure_python   | 208 us                                                      | 180 us: 1.16x faster                                                                  |
| unpickle_pure_python | 157 us                                                      | 137 us: 1.14x faster                                                                  |
| xml_etree_parse      | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                                                 |
| tomli_loads          | 1.46 sec                                                    | 1.44 sec: 1.01x faster                                                                |
| pickle_dict          | 18.5 us                                                     | 18.3 us: 1.01x faster                                                                 |
| xml_etree_iterparse  | 65.6 ms                                                     | 66.3 ms: 1.01x slower                                                                 |
| xml_etree_generate   | 52.5 ms                                                     | 54.5 ms: 1.04x slower                                                                 |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                                                 |
| unpickle_list        | 2.59 us                                                     | 2.79 us: 1.08x slower                                                                 |
| unpickle             | 7.57 us                                                     | 8.33 us: 1.10x slower                                                                 |
| pickle               | 6.64 us                                                     | 7.41 us: 1.12x slower                                                                 |
| pickle_list          | 2.70 us                                                     | 3.09 us: 1.14x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                          |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.0 ms: 1.06x slower                                                                 |
| python_startup_no_site | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.50 ms: 1.01x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 72.5 us: 4.49x faster                                                                 |
| generators                 | 34.0 ms                                                     | 21.6 ms: 1.57x faster                                                                 |
| asyncio_tcp                | 726 ms                                                      | 468 ms: 1.55x faster                                                                  |
| json_dumps                 | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                                                 |
| logging_silent             | 71.8 ns                                                     | 55.3 ns: 1.30x faster                                                                 |
| richards_super             | 38.7 ms                                                     | 30.7 ms: 1.26x faster                                                                 |
| raytrace                   | 213 ms                                                      | 173 ms: 1.24x faster                                                                  |
| comprehensions             | 15.6 us                                                     | 12.7 us: 1.23x faster                                                                 |
| sqlglot_parse              | 953 us                                                      | 776 us: 1.23x faster                                                                  |
| async_tree_none            | 332 ms                                                      | 271 ms: 1.23x faster                                                                  |
| unpack_sequence            | 46.9 ns                                                     | 39.5 ns: 1.19x faster                                                                 |
| mdp                        | 1.59 sec                                                    | 1.36 sec: 1.18x faster                                                                |
| sqlglot_transpile          | 1.16 ms                                                     | 1.00 ms: 1.16x faster                                                                 |
| async_tree_memoization     | 399 ms                                                      | 344 ms: 1.16x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 457 ms: 1.16x faster                                                                  |
| richards                   | 31.4 ms                                                     | 27.1 ms: 1.16x faster                                                                 |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.75 sec: 1.16x faster                                                                |
| pickle_pure_python         | 208 us                                                      | 180 us: 1.16x faster                                                                  |
| deepcopy_memo              | 26.0 us                                                     | 22.5 us: 1.16x faster                                                                 |
| async_tree_memoization_tg  | 405 ms                                                      | 351 ms: 1.15x faster                                                                  |
| unpickle_pure_python       | 157 us                                                      | 137 us: 1.14x faster                                                                  |
| sympy_sum                  | 100 ms                                                      | 88.3 ms: 1.13x faster                                                                 |
| coroutines                 | 15.0 ms                                                     | 13.3 ms: 1.12x faster                                                                 |
| async_tree_io_tg           | 829 ms                                                      | 738 ms: 1.12x faster                                                                  |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 722 ms: 1.12x faster                                                                  |
| scimark_lu                 | 62.8 ms                                                     | 56.2 ms: 1.12x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 470 ms: 1.11x faster                                                                  |
| sympy_str                  | 185 ms                                                      | 167 ms: 1.11x faster                                                                  |
| deepcopy                   | 246 us                                                      | 223 us: 1.11x faster                                                                  |
| chaos                      | 48.4 ms                                                     | 43.8 ms: 1.11x faster                                                                 |
| dulwich_log                | 46.4 ms                                                     | 42.1 ms: 1.10x faster                                                                 |
| logging_simple             | 6.86 us                                                     | 6.23 us: 1.10x faster                                                                 |
| go                         | 101 ms                                                      | 92.3 ms: 1.10x faster                                                                 |
| sqlite_synth               | 1.77 us                                                     | 1.61 us: 1.09x faster                                                                 |
| mypy2                      | 459 ms                                                      | 423 ms: 1.09x faster                                                                  |
| regex_compile              | 91.0 ms                                                     | 84.4 ms: 1.08x faster                                                                 |
| sympy_expand               | 299 ms                                                      | 280 ms: 1.07x faster                                                                  |
| sympy_integrate            | 14.0 ms                                                     | 13.2 ms: 1.07x faster                                                                 |
| logging_format             | 7.16 us                                                     | 6.74 us: 1.06x faster                                                                 |
| tornado_http               | 92.8 ms                                                     | 88.5 ms: 1.05x faster                                                                 |
| dask                       | 273 ms                                                      | 260 ms: 1.05x faster                                                                  |
| chameleon                  | 5.26 ms                                                     | 5.03 ms: 1.05x faster                                                                 |
| nqueens                    | 68.3 ms                                                     | 65.5 ms: 1.04x faster                                                                 |
| sqlglot_normalize          | 190 ms                                                      | 182 ms: 1.04x faster                                                                  |
| xml_etree_parse            | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                                                 |
| docutils                   | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                                |
| deepcopy_reduce            | 2.06 us                                                     | 1.99 us: 1.04x faster                                                                 |
| pprint_pformat             | 1.09 sec                                                    | 1.06 sec: 1.02x faster                                                                |
| crypto_pyaes               | 48.9 ms                                                     | 47.9 ms: 1.02x faster                                                                 |
| pprint_safe_repr           | 529 ms                                                      | 519 ms: 1.02x faster                                                                  |
| bench_thread_pool          | 872 us                                                      | 856 us: 1.02x faster                                                                  |
| pidigits                   | 150 ms                                                      | 148 ms: 1.02x faster                                                                  |
| tomli_loads                | 1.46 sec                                                    | 1.44 sec: 1.01x faster                                                                |
| mako                       | 7.58 ms                                                     | 7.50 ms: 1.01x faster                                                                 |
| pickle_dict                | 18.5 us                                                     | 18.3 us: 1.01x faster                                                                 |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                                 |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                                 |
| meteor_contest             | 75.2 ms                                                     | 75.9 ms: 1.01x slower                                                                 |
| deltablue                  | 2.70 ms                                                     | 2.73 ms: 1.01x slower                                                                 |
| xml_etree_iterparse        | 65.6 ms                                                     | 66.3 ms: 1.01x slower                                                                 |
| scimark_sor                | 78.1 ms                                                     | 79.0 ms: 1.01x slower                                                                 |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.01x slower                                                                  |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                                 |
| xml_etree_generate         | 52.5 ms                                                     | 54.5 ms: 1.04x slower                                                                 |
| coverage                   | 43.4 ms                                                     | 45.0 ms: 1.04x slower                                                                 |
| pyflate                    | 312 ms                                                      | 324 ms: 1.04x slower                                                                  |
| create_gc_cycles           | 713 us                                                      | 742 us: 1.04x slower                                                                  |
| json_loads                 | 13.0 us                                                     | 13.5 us: 1.04x slower                                                                 |
| float                      | 54.4 ms                                                     | 56.6 ms: 1.04x slower                                                                 |
| 2to3                       | 214 ms                                                      | 223 ms: 1.04x slower                                                                  |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                                 |
| fannkuch                   | 253 ms                                                      | 267 ms: 1.05x slower                                                                  |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.7 ms: 1.05x slower                                                                 |
| python_startup             | 19.8 ms                                                     | 21.0 ms: 1.06x slower                                                                 |
| unpickle_list              | 2.59 us                                                     | 2.79 us: 1.08x slower                                                                 |
| hexiom                     | 4.55 ms                                                     | 4.94 ms: 1.09x slower                                                                 |
| unpickle                   | 7.57 us                                                     | 8.33 us: 1.10x slower                                                                 |
| python_startup_no_site     | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                                                 |
| bench_mp_pool              | 63.2 ms                                                     | 69.7 ms: 1.10x slower                                                                 |
| pickle                     | 6.64 us                                                     | 7.41 us: 1.12x slower                                                                 |
| pathlib                    | 70.9 ms                                                     | 79.3 ms: 1.12x slower                                                                 |
| scimark_fft                | 179 ms                                                      | 202 ms: 1.13x slower                                                                  |
| pickle_list                | 2.70 us                                                     | 3.09 us: 1.14x slower                                                                 |
| nbody                      | 70.3 ms                                                     | 81.4 ms: 1.16x slower                                                                 |
| spectral_norm              | 68.3 ms                                                     | 80.6 ms: 1.18x slower                                                                 |
| telco                      | 4.06 ms                                                     | 4.80 ms: 1.18x slower                                                                 |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.19 ms: 1.24x slower                                                                 |
| async_generators           | 177 ms                                                      | 236 ms: 1.33x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                          |

Benchmark hidden because not significant (3): pycparser, xml_etree_process, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.93% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown