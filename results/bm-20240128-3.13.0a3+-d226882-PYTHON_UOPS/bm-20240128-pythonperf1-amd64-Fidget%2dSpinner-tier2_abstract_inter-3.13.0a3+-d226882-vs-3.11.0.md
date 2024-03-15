
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.05x faster
- HPT reliability: 99.37%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 224 ms: 1.05x slower                                                                  |
| chameleon      | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                                 |
| docutils       | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                                |
| tornado_http   | 92.8 ms                                                     | 85.8 ms: 1.08x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 276 ms: 1.21x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 464 ms: 1.14x faster                                                                  |
| async_tree_memoization     | 399 ms                                                      | 350 ms: 1.14x faster                                                                  |
| async_tree_memoization_tg  | 405 ms                                                      | 363 ms: 1.12x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 744 ms: 1.09x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 488 ms: 1.07x faster                                                                  |
| async_tree_none_tg         | 309 ms                                                      | 289 ms: 1.07x faster                                                                  |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                                                  |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 58.1 ms: 1.07x slower                                                                 |
| nbody          | 70.3 ms                                                     | 78.8 ms: 1.12x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.06x slower                                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 85.8 ms: 1.06x faster                                                                 |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                                  |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                                 |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.51 ms: 1.47x faster                                                                 |
| pickle_pure_python   | 208 us                                                      | 179 us: 1.16x faster                                                                  |
| unpickle_pure_python | 157 us                                                      | 137 us: 1.14x faster                                                                  |
| pickle_dict          | 18.5 us                                                     | 18.6 us: 1.01x slower                                                                 |
| xml_etree_process    | 37.2 ms                                                     | 38.0 ms: 1.02x slower                                                                 |
| xml_etree_iterparse  | 65.6 ms                                                     | 69.1 ms: 1.05x slower                                                                 |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                                 |
| xml_etree_generate   | 52.5 ms                                                     | 55.6 ms: 1.06x slower                                                                 |
| pickle               | 6.64 us                                                     | 7.11 us: 1.07x slower                                                                 |
| pickle_list          | 2.70 us                                                     | 2.91 us: 1.08x slower                                                                 |
| unpickle_list        | 2.59 us                                                     | 2.81 us: 1.08x slower                                                                 |
| unpickle             | 7.57 us                                                     | 8.45 us: 1.12x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (2): xml_etree_parse, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                                 |
| python_startup_no_site | 16.8 ms                                                     | 18.4 ms: 1.09x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.99 ms: 1.05x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 73.7 us: 4.42x faster                                                                 |
| generators                 | 34.0 ms                                                     | 20.9 ms: 1.63x faster                                                                 |
| asyncio_tcp                | 726 ms                                                      | 490 ms: 1.48x faster                                                                  |
| json_dumps                 | 8.09 ms                                                     | 5.51 ms: 1.47x faster                                                                 |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.49 sec: 1.36x faster                                                                |
| logging_silent             | 71.8 ns                                                     | 55.0 ns: 1.30x faster                                                                 |
| richards_super             | 38.7 ms                                                     | 30.2 ms: 1.28x faster                                                                 |
| sqlglot_parse              | 953 us                                                      | 782 us: 1.22x faster                                                                  |
| unpack_sequence            | 46.9 ns                                                     | 38.7 ns: 1.21x faster                                                                 |
| async_tree_none            | 332 ms                                                      | 276 ms: 1.21x faster                                                                  |
| comprehensions             | 15.6 us                                                     | 13.0 us: 1.21x faster                                                                 |
| raytrace                   | 213 ms                                                      | 178 ms: 1.20x faster                                                                  |
| richards                   | 31.4 ms                                                     | 26.6 ms: 1.18x faster                                                                 |
| pickle_pure_python         | 208 us                                                      | 179 us: 1.16x faster                                                                  |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                                                 |
| unpickle_pure_python       | 157 us                                                      | 137 us: 1.14x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 464 ms: 1.14x faster                                                                  |
| async_tree_memoization     | 399 ms                                                      | 350 ms: 1.14x faster                                                                  |
| sympy_sum                  | 100 ms                                                      | 88.7 ms: 1.13x faster                                                                 |
| scimark_lu                 | 62.8 ms                                                     | 55.9 ms: 1.12x faster                                                                 |
| deepcopy_memo              | 26.0 us                                                     | 23.2 us: 1.12x faster                                                                 |
| async_tree_memoization_tg  | 405 ms                                                      | 363 ms: 1.12x faster                                                                  |
| deepcopy                   | 246 us                                                      | 223 us: 1.11x faster                                                                  |
| mdp                        | 1.59 sec                                                    | 1.44 sec: 1.11x faster                                                                |
| logging_simple             | 6.86 us                                                     | 6.23 us: 1.10x faster                                                                 |
| chaos                      | 48.4 ms                                                     | 44.1 ms: 1.10x faster                                                                 |
| go                         | 101 ms                                                      | 92.3 ms: 1.09x faster                                                                 |
| sympy_str                  | 185 ms                                                      | 169 ms: 1.09x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 744 ms: 1.09x faster                                                                  |
| tornado_http               | 92.8 ms                                                     | 85.8 ms: 1.08x faster                                                                 |
| coroutines                 | 15.0 ms                                                     | 13.9 ms: 1.08x faster                                                                 |
| dulwich_log                | 46.4 ms                                                     | 43.1 ms: 1.08x faster                                                                 |
| nqueens                    | 68.3 ms                                                     | 63.5 ms: 1.08x faster                                                                 |
| logging_format             | 7.16 us                                                     | 6.67 us: 1.07x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 488 ms: 1.07x faster                                                                  |
| sympy_expand               | 299 ms                                                      | 280 ms: 1.07x faster                                                                  |
| async_tree_none_tg         | 309 ms                                                      | 289 ms: 1.07x faster                                                                  |
| mypy2                      | 459 ms                                                      | 431 ms: 1.07x faster                                                                  |
| sqlite_synth               | 1.77 us                                                     | 1.66 us: 1.06x faster                                                                 |
| pycparser                  | 720 ms                                                      | 678 ms: 1.06x faster                                                                  |
| regex_compile              | 91.0 ms                                                     | 85.8 ms: 1.06x faster                                                                 |
| deepcopy_reduce            | 2.06 us                                                     | 1.94 us: 1.06x faster                                                                 |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                                                  |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.06x faster                                                                 |
| chameleon                  | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                                 |
| dask                       | 273 ms                                                      | 262 ms: 1.04x faster                                                                  |
| crypto_pyaes               | 48.9 ms                                                     | 47.3 ms: 1.03x faster                                                                 |
| sqlglot_normalize          | 190 ms                                                      | 186 ms: 1.02x faster                                                                  |
| docutils                   | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                                |
| bench_thread_pool          | 872 us                                                      | 857 us: 1.02x faster                                                                  |
| scimark_sor                | 78.1 ms                                                     | 77.7 ms: 1.01x faster                                                                 |
| pprint_safe_repr           | 529 ms                                                      | 527 ms: 1.01x faster                                                                  |
| pickle_dict                | 18.5 us                                                     | 18.6 us: 1.01x slower                                                                 |
| deltablue                  | 2.70 ms                                                     | 2.74 ms: 1.01x slower                                                                 |
| sqlglot_optimize           | 34.5 ms                                                     | 35.1 ms: 1.02x slower                                                                 |
| gc_traversal               | 1.49 ms                                                     | 1.52 ms: 1.02x slower                                                                 |
| xml_etree_process          | 37.2 ms                                                     | 38.0 ms: 1.02x slower                                                                 |
| coverage                   | 43.4 ms                                                     | 45.0 ms: 1.04x slower                                                                 |
| python_startup             | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                                 |
| meteor_contest             | 75.2 ms                                                     | 78.7 ms: 1.05x slower                                                                 |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                                  |
| 2to3                       | 214 ms                                                      | 224 ms: 1.05x slower                                                                  |
| create_gc_cycles           | 713 us                                                      | 750 us: 1.05x slower                                                                  |
| mako                       | 7.58 ms                                                     | 7.99 ms: 1.05x slower                                                                 |
| xml_etree_iterparse        | 65.6 ms                                                     | 69.1 ms: 1.05x slower                                                                 |
| pyflate                    | 312 ms                                                      | 329 ms: 1.05x slower                                                                  |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                                                 |
| xml_etree_generate         | 52.5 ms                                                     | 55.6 ms: 1.06x slower                                                                 |
| fannkuch                   | 253 ms                                                      | 268 ms: 1.06x slower                                                                  |
| scimark_monte_carlo        | 45.3 ms                                                     | 48.2 ms: 1.06x slower                                                                 |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                                 |
| float                      | 54.4 ms                                                     | 58.1 ms: 1.07x slower                                                                 |
| pickle                     | 6.64 us                                                     | 7.11 us: 1.07x slower                                                                 |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                                 |
| pickle_list                | 2.70 us                                                     | 2.91 us: 1.08x slower                                                                 |
| unpickle_list              | 2.59 us                                                     | 2.81 us: 1.08x slower                                                                 |
| bench_mp_pool              | 63.2 ms                                                     | 68.7 ms: 1.09x slower                                                                 |
| python_startup_no_site     | 16.8 ms                                                     | 18.4 ms: 1.09x slower                                                                 |
| hexiom                     | 4.55 ms                                                     | 5.01 ms: 1.10x slower                                                                 |
| unpickle                   | 7.57 us                                                     | 8.45 us: 1.12x slower                                                                 |
| json                       | 2.98 ms                                                     | 3.34 ms: 1.12x slower                                                                 |
| nbody                      | 70.3 ms                                                     | 78.8 ms: 1.12x slower                                                                 |
| pathlib                    | 70.9 ms                                                     | 79.8 ms: 1.13x slower                                                                 |
| scimark_fft                | 179 ms                                                      | 209 ms: 1.16x slower                                                                  |
| telco                      | 4.06 ms                                                     | 4.74 ms: 1.17x slower                                                                 |
| spectral_norm              | 68.3 ms                                                     | 80.3 ms: 1.18x slower                                                                 |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.19 ms: 1.24x slower                                                                 |
| async_generators           | 177 ms                                                      | 230 ms: 1.30x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                          |

Benchmark hidden because not significant (4): xml_etree_parse, pidigits, tomli_loads, pprint_pformat
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.37% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown