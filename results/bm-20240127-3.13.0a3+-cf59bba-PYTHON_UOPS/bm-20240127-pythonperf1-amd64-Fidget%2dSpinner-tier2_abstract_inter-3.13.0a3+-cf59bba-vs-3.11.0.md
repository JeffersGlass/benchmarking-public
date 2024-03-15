
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.05x faster
- HPT reliability: 99.57%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 229 ms: 1.07x slower                                                                  |
| chameleon      | 5.26 ms                                                     | 5.05 ms: 1.04x faster                                                                 |
| tornado_http   | 92.8 ms                                                     | 87.4 ms: 1.06x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                                  |
| async_tree_memoization     | 399 ms                                                      | 343 ms: 1.16x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 466 ms: 1.14x faster                                                                  |
| async_tree_memoization_tg  | 405 ms                                                      | 366 ms: 1.11x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 747 ms: 1.08x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 487 ms: 1.07x faster                                                                  |
| async_tree_none_tg         | 309 ms                                                      | 288 ms: 1.07x faster                                                                  |
| async_tree_io_tg           | 829 ms                                                      | 784 ms: 1.06x faster                                                                  |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 149 ms: 1.00x faster                                                                  |
| float          | 54.4 ms                                                     | 56.7 ms: 1.04x slower                                                                 |
| nbody          | 70.3 ms                                                     | 77.0 ms: 1.09x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.6 ms: 1.08x faster                                                                 |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                                  |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                                 |
| regex_v8       | 14.2 ms                                                     | 15.7 ms: 1.11x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                                                 |
| unpickle_pure_python | 157 us                                                      | 139 us: 1.13x faster                                                                  |
| pickle_pure_python   | 208 us                                                      | 186 us: 1.12x faster                                                                  |
| xml_etree_parse      | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                                 |
| tomli_loads          | 1.46 sec                                                    | 1.40 sec: 1.04x faster                                                                |
| xml_etree_process    | 37.2 ms                                                     | 38.0 ms: 1.02x slower                                                                 |
| xml_etree_iterparse  | 65.6 ms                                                     | 68.9 ms: 1.05x slower                                                                 |
| unpickle_list        | 2.59 us                                                     | 2.73 us: 1.05x slower                                                                 |
| xml_etree_generate   | 52.5 ms                                                     | 55.5 ms: 1.06x slower                                                                 |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.06x slower                                                                 |
| pickle               | 6.64 us                                                     | 7.22 us: 1.09x slower                                                                 |
| unpickle             | 7.57 us                                                     | 8.30 us: 1.10x slower                                                                 |
| pickle_list          | 2.70 us                                                     | 2.98 us: 1.11x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                                                 |
| python_startup_no_site | 16.8 ms                                                     | 18.9 ms: 1.12x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.22 ms: 1.05x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 74.8 us: 4.36x faster                                                                 |
| generators                 | 34.0 ms                                                     | 22.6 ms: 1.50x faster                                                                 |
| asyncio_tcp                | 726 ms                                                      | 491 ms: 1.48x faster                                                                  |
| json_dumps                 | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                                                 |
| logging_silent             | 71.8 ns                                                     | 56.3 ns: 1.27x faster                                                                 |
| richards_super             | 38.7 ms                                                     | 30.9 ms: 1.25x faster                                                                 |
| comprehensions             | 15.6 us                                                     | 12.5 us: 1.25x faster                                                                 |
| sqlglot_parse              | 953 us                                                      | 780 us: 1.22x faster                                                                  |
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                                  |
| raytrace                   | 213 ms                                                      | 176 ms: 1.21x faster                                                                  |
| unpack_sequence            | 46.9 ns                                                     | 39.1 ns: 1.20x faster                                                                 |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.72 sec: 1.18x faster                                                                |
| async_tree_memoization     | 399 ms                                                      | 343 ms: 1.16x faster                                                                  |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                                                 |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 466 ms: 1.14x faster                                                                  |
| richards                   | 31.4 ms                                                     | 27.6 ms: 1.14x faster                                                                 |
| unpickle_pure_python       | 157 us                                                      | 139 us: 1.13x faster                                                                  |
| sympy_sum                  | 100 ms                                                      | 89.1 ms: 1.12x faster                                                                 |
| pickle_pure_python         | 208 us                                                      | 186 us: 1.12x faster                                                                  |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                                 |
| logging_simple             | 6.86 us                                                     | 6.15 us: 1.12x faster                                                                 |
| chaos                      | 48.4 ms                                                     | 43.5 ms: 1.11x faster                                                                 |
| sympy_str                  | 185 ms                                                      | 167 ms: 1.11x faster                                                                  |
| mdp                        | 1.59 sec                                                    | 1.44 sec: 1.11x faster                                                                |
| async_tree_memoization_tg  | 405 ms                                                      | 366 ms: 1.11x faster                                                                  |
| coroutines                 | 15.0 ms                                                     | 13.6 ms: 1.10x faster                                                                 |
| logging_format             | 7.16 us                                                     | 6.59 us: 1.09x faster                                                                 |
| deepcopy                   | 246 us                                                      | 227 us: 1.09x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 747 ms: 1.08x faster                                                                  |
| go                         | 101 ms                                                      | 93.7 ms: 1.08x faster                                                                 |
| regex_compile              | 91.0 ms                                                     | 84.6 ms: 1.08x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 487 ms: 1.07x faster                                                                  |
| nqueens                    | 68.3 ms                                                     | 63.8 ms: 1.07x faster                                                                 |
| async_tree_none_tg         | 309 ms                                                      | 288 ms: 1.07x faster                                                                  |
| deepcopy_memo              | 26.0 us                                                     | 24.4 us: 1.07x faster                                                                 |
| mypy2                      | 459 ms                                                      | 432 ms: 1.06x faster                                                                  |
| tornado_http               | 92.8 ms                                                     | 87.4 ms: 1.06x faster                                                                 |
| dulwich_log                | 46.4 ms                                                     | 43.7 ms: 1.06x faster                                                                 |
| async_tree_io_tg           | 829 ms                                                      | 784 ms: 1.06x faster                                                                  |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.06x faster                                                                 |
| mako                       | 7.58 ms                                                     | 7.22 ms: 1.05x faster                                                                 |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                                                  |
| sqlglot_normalize          | 190 ms                                                      | 182 ms: 1.04x faster                                                                  |
| chameleon                  | 5.26 ms                                                     | 5.05 ms: 1.04x faster                                                                 |
| xml_etree_parse            | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                                 |
| dask                       | 273 ms                                                      | 263 ms: 1.04x faster                                                                  |
| tomli_loads                | 1.46 sec                                                    | 1.40 sec: 1.04x faster                                                                |
| deltablue                  | 2.70 ms                                                     | 2.61 ms: 1.03x faster                                                                 |
| deepcopy_reduce            | 2.06 us                                                     | 2.01 us: 1.02x faster                                                                 |
| crypto_pyaes               | 48.9 ms                                                     | 48.1 ms: 1.01x faster                                                                 |
| pprint_safe_repr           | 529 ms                                                      | 523 ms: 1.01x faster                                                                  |
| pprint_pformat             | 1.09 sec                                                    | 1.08 sec: 1.01x faster                                                                |
| pidigits                   | 150 ms                                                      | 149 ms: 1.00x faster                                                                  |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                                 |
| xml_etree_process          | 37.2 ms                                                     | 38.0 ms: 1.02x slower                                                                 |
| meteor_contest             | 75.2 ms                                                     | 77.0 ms: 1.02x slower                                                                 |
| gc_traversal               | 1.49 ms                                                     | 1.54 ms: 1.03x slower                                                                 |
| create_gc_cycles           | 713 us                                                      | 740 us: 1.04x slower                                                                  |
| float                      | 54.4 ms                                                     | 56.7 ms: 1.04x slower                                                                 |
| pyflate                    | 312 ms                                                      | 326 ms: 1.04x slower                                                                  |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                                  |
| hexiom                     | 4.55 ms                                                     | 4.78 ms: 1.05x slower                                                                 |
| xml_etree_iterparse        | 65.6 ms                                                     | 68.9 ms: 1.05x slower                                                                 |
| python_startup             | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                                                 |
| unpickle_list              | 2.59 us                                                     | 2.73 us: 1.05x slower                                                                 |
| xml_etree_generate         | 52.5 ms                                                     | 55.5 ms: 1.06x slower                                                                 |
| scimark_monte_carlo        | 45.3 ms                                                     | 48.0 ms: 1.06x slower                                                                 |
| json_loads                 | 13.0 us                                                     | 13.8 us: 1.06x slower                                                                 |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                                 |
| 2to3                       | 214 ms                                                      | 229 ms: 1.07x slower                                                                  |
| scimark_sor                | 78.1 ms                                                     | 83.8 ms: 1.07x slower                                                                 |
| fannkuch                   | 253 ms                                                      | 272 ms: 1.07x slower                                                                  |
| pickle                     | 6.64 us                                                     | 7.22 us: 1.09x slower                                                                 |
| nbody                      | 70.3 ms                                                     | 77.0 ms: 1.09x slower                                                                 |
| unpickle                   | 7.57 us                                                     | 8.30 us: 1.10x slower                                                                 |
| coverage                   | 43.4 ms                                                     | 47.8 ms: 1.10x slower                                                                 |
| scimark_fft                | 179 ms                                                      | 198 ms: 1.10x slower                                                                  |
| regex_v8                   | 14.2 ms                                                     | 15.7 ms: 1.11x slower                                                                 |
| pickle_list                | 2.70 us                                                     | 2.98 us: 1.11x slower                                                                 |
| spectral_norm              | 68.3 ms                                                     | 76.2 ms: 1.12x slower                                                                 |
| bench_mp_pool              | 63.2 ms                                                     | 70.8 ms: 1.12x slower                                                                 |
| python_startup_no_site     | 16.8 ms                                                     | 18.9 ms: 1.12x slower                                                                 |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.91 ms: 1.13x slower                                                                 |
| pathlib                    | 70.9 ms                                                     | 80.9 ms: 1.14x slower                                                                 |
| telco                      | 4.06 ms                                                     | 4.73 ms: 1.16x slower                                                                 |
| async_generators           | 177 ms                                                      | 236 ms: 1.33x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                          |

Benchmark hidden because not significant (6): pycparser, docutils, scimark_lu, pickle_dict, bench_thread_pool, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.57% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown