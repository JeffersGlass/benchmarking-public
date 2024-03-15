
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 224 ms: 1.05x slower                                                                  |
| chameleon      | 5.26 ms                                                     | 4.77 ms: 1.10x faster                                                                 |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                                |
| tornado_http   | 92.8 ms                                                     | 86.7 ms: 1.07x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.16x faster                                                                  |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                                                  |
| async_tree_memoization_tg  | 405 ms                                                      | 356 ms: 1.14x faster                                                                  |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                                  |
| async_tree_none_tg         | 309 ms                                                      | 283 ms: 1.09x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 483 ms: 1.08x faster                                                                  |
| async_tree_io_tg           | 829 ms                                                      | 774 ms: 1.07x faster                                                                  |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 62.2 ms: 1.13x faster                                                                 |
| float          | 54.4 ms                                                     | 52.1 ms: 1.04x faster                                                                 |
| pidigits       | 150 ms                                                      | 154 ms: 1.03x slower                                                                  |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 82.7 ms: 1.10x faster                                                                 |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                                 |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                                  |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.44 ms: 1.49x faster                                                                 |
| unpickle_pure_python | 157 us                                                      | 131 us: 1.20x faster                                                                  |
| pickle_pure_python   | 208 us                                                      | 177 us: 1.18x faster                                                                  |
| tomli_loads          | 1.46 sec                                                    | 1.28 sec: 1.13x faster                                                                |
| pickle_dict          | 18.5 us                                                     | 17.7 us: 1.05x faster                                                                 |
| xml_etree_process    | 37.2 ms                                                     | 35.8 ms: 1.04x faster                                                                 |
| xml_etree_parse      | 97.6 ms                                                     | 95.2 ms: 1.03x faster                                                                 |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.7 ms: 1.01x faster                                                                 |
| xml_etree_generate   | 52.5 ms                                                     | 52.2 ms: 1.01x faster                                                                 |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                                                 |
| pickle_list          | 2.70 us                                                     | 2.82 us: 1.05x slower                                                                 |
| unpickle_list        | 2.59 us                                                     | 2.84 us: 1.10x slower                                                                 |
| pickle               | 6.64 us                                                     | 7.31 us: 1.10x slower                                                                 |
| unpickle             | 7.57 us                                                     | 8.44 us: 1.12x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.1 ms: 1.07x slower                                                                 |
| python_startup_no_site | 16.8 ms                                                     | 19.1 ms: 1.14x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.86 ms: 1.11x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 68.1 us: 4.78x faster                                                                 |
| generators                 | 34.0 ms                                                     | 20.9 ms: 1.62x faster                                                                 |
| asyncio_tcp                | 726 ms                                                      | 483 ms: 1.50x faster                                                                  |
| json_dumps                 | 8.09 ms                                                     | 5.44 ms: 1.49x faster                                                                 |
| logging_silent             | 71.8 ns                                                     | 52.2 ns: 1.38x faster                                                                 |
| richards_super             | 38.7 ms                                                     | 28.3 ms: 1.37x faster                                                                 |
| comprehensions             | 15.6 us                                                     | 11.7 us: 1.34x faster                                                                 |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.52 sec: 1.33x faster                                                                |
| deltablue                  | 2.70 ms                                                     | 2.10 ms: 1.29x faster                                                                 |
| richards                   | 31.4 ms                                                     | 24.9 ms: 1.26x faster                                                                 |
| sqlglot_parse              | 953 us                                                      | 760 us: 1.25x faster                                                                  |
| raytrace                   | 213 ms                                                      | 172 ms: 1.24x faster                                                                  |
| deepcopy_memo              | 26.0 us                                                     | 21.2 us: 1.22x faster                                                                 |
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                                  |
| unpack_sequence            | 46.9 ns                                                     | 39.1 ns: 1.20x faster                                                                 |
| unpickle_pure_python       | 157 us                                                      | 131 us: 1.20x faster                                                                  |
| sqlglot_transpile          | 1.16 ms                                                     | 984 us: 1.18x faster                                                                  |
| pickle_pure_python         | 208 us                                                      | 177 us: 1.18x faster                                                                  |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.16x faster                                                                  |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                                                  |
| nqueens                    | 68.3 ms                                                     | 59.7 ms: 1.14x faster                                                                 |
| logging_simple             | 6.86 us                                                     | 6.02 us: 1.14x faster                                                                 |
| scimark_lu                 | 62.8 ms                                                     | 55.2 ms: 1.14x faster                                                                 |
| chaos                      | 48.4 ms                                                     | 42.5 ms: 1.14x faster                                                                 |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.14x faster                                                                 |
| async_tree_memoization_tg  | 405 ms                                                      | 356 ms: 1.14x faster                                                                  |
| tomli_loads                | 1.46 sec                                                    | 1.28 sec: 1.13x faster                                                                |
| nbody                      | 70.3 ms                                                     | 62.2 ms: 1.13x faster                                                                 |
| deepcopy                   | 246 us                                                      | 218 us: 1.13x faster                                                                  |
| coroutines                 | 15.0 ms                                                     | 13.5 ms: 1.11x faster                                                                 |
| mako                       | 7.58 ms                                                     | 6.86 ms: 1.11x faster                                                                 |
| logging_format             | 7.16 us                                                     | 6.48 us: 1.11x faster                                                                 |
| sympy_sum                  | 100 ms                                                      | 90.7 ms: 1.10x faster                                                                 |
| chameleon                  | 5.26 ms                                                     | 4.77 ms: 1.10x faster                                                                 |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                                  |
| regex_compile              | 91.0 ms                                                     | 82.7 ms: 1.10x faster                                                                 |
| dulwich_log                | 46.4 ms                                                     | 42.2 ms: 1.10x faster                                                                 |
| async_tree_none_tg         | 309 ms                                                      | 283 ms: 1.09x faster                                                                  |
| sympy_str                  | 185 ms                                                      | 170 ms: 1.09x faster                                                                  |
| spectral_norm              | 68.3 ms                                                     | 62.9 ms: 1.09x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 483 ms: 1.08x faster                                                                  |
| async_tree_io_tg           | 829 ms                                                      | 774 ms: 1.07x faster                                                                  |
| sympy_expand               | 299 ms                                                      | 279 ms: 1.07x faster                                                                  |
| tornado_http               | 92.8 ms                                                     | 86.7 ms: 1.07x faster                                                                 |
| deepcopy_reduce            | 2.06 us                                                     | 1.93 us: 1.07x faster                                                                 |
| pprint_safe_repr           | 529 ms                                                      | 498 ms: 1.06x faster                                                                  |
| sqlglot_normalize          | 190 ms                                                      | 180 ms: 1.06x faster                                                                  |
| mypy2                      | 459 ms                                                      | 435 ms: 1.05x faster                                                                  |
| pprint_pformat             | 1.09 sec                                                    | 1.03 sec: 1.05x faster                                                                |
| pickle_dict                | 18.5 us                                                     | 17.7 us: 1.05x faster                                                                 |
| float                      | 54.4 ms                                                     | 52.1 ms: 1.04x faster                                                                 |
| xml_etree_process          | 37.2 ms                                                     | 35.8 ms: 1.04x faster                                                                 |
| go                         | 101 ms                                                      | 97.4 ms: 1.04x faster                                                                 |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                                |
| dask                       | 273 ms                                                      | 265 ms: 1.03x faster                                                                  |
| xml_etree_parse            | 97.6 ms                                                     | 95.2 ms: 1.03x faster                                                                 |
| crypto_pyaes               | 48.9 ms                                                     | 47.9 ms: 1.02x faster                                                                 |
| bench_thread_pool          | 872 us                                                      | 859 us: 1.01x faster                                                                  |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.7 ms: 1.01x faster                                                                 |
| sympy_integrate            | 14.0 ms                                                     | 13.9 ms: 1.01x faster                                                                 |
| fannkuch                   | 253 ms                                                      | 251 ms: 1.01x faster                                                                  |
| xml_etree_generate         | 52.5 ms                                                     | 52.2 ms: 1.01x faster                                                                 |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                                 |
| pyflate                    | 312 ms                                                      | 316 ms: 1.01x slower                                                                  |
| gc_traversal               | 1.49 ms                                                     | 1.52 ms: 1.01x slower                                                                 |
| mdp                        | 1.59 sec                                                    | 1.62 sec: 1.02x slower                                                                |
| pidigits                   | 150 ms                                                      | 154 ms: 1.03x slower                                                                  |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                                 |
| json_loads                 | 13.0 us                                                     | 13.5 us: 1.04x slower                                                                 |
| create_gc_cycles           | 713 us                                                      | 745 us: 1.04x slower                                                                  |
| pickle_list                | 2.70 us                                                     | 2.82 us: 1.05x slower                                                                 |
| 2to3                       | 214 ms                                                      | 224 ms: 1.05x slower                                                                  |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                                  |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                                 |
| coverage                   | 43.4 ms                                                     | 45.8 ms: 1.06x slower                                                                 |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.72 ms: 1.06x slower                                                                 |
| meteor_contest             | 75.2 ms                                                     | 80.1 ms: 1.07x slower                                                                 |
| python_startup             | 19.8 ms                                                     | 21.1 ms: 1.07x slower                                                                 |
| scimark_fft                | 179 ms                                                      | 195 ms: 1.09x slower                                                                  |
| unpickle_list              | 2.59 us                                                     | 2.84 us: 1.10x slower                                                                 |
| pickle                     | 6.64 us                                                     | 7.31 us: 1.10x slower                                                                 |
| unpickle                   | 7.57 us                                                     | 8.44 us: 1.12x slower                                                                 |
| json                       | 2.98 ms                                                     | 3.33 ms: 1.12x slower                                                                 |
| pathlib                    | 70.9 ms                                                     | 79.8 ms: 1.13x slower                                                                 |
| bench_mp_pool              | 63.2 ms                                                     | 71.4 ms: 1.13x slower                                                                 |
| telco                      | 4.06 ms                                                     | 4.59 ms: 1.13x slower                                                                 |
| python_startup_no_site     | 16.8 ms                                                     | 19.1 ms: 1.14x slower                                                                 |
| hexiom                     | 4.55 ms                                                     | 5.44 ms: 1.19x slower                                                                 |
| scimark_monte_carlo        | 45.3 ms                                                     | 58.3 ms: 1.29x slower                                                                 |
| async_generators           | 177 ms                                                      | 242 ms: 1.37x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                                          |

Benchmark hidden because not significant (2): pycparser, scimark_sor
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown