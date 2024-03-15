
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0rc2
- machine: linux-x86_64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.73%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| docutils       | 2.85 sec                                                     | 2.90 sec: 1.02x slower                                             |
| tornado_http   | 124 ms                                                       | 120 ms: 1.04x faster                                               |
| Geometric mean | (ref)                                                        | 1.01x faster                                                       |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 552 ms: 1.14x faster                                               |
| async_tree_none         | 518 ms                                                       | 458 ms: 1.13x faster                                               |
| async_tree_io           | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                             |
| async_tree_cpu_io_mixed | 753 ms                                                       | 702 ms: 1.07x faster                                               |
| Geometric mean          | (ref)                                                        | 1.11x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 87.5 ms: 1.06x faster                                              |
| pidigits       | 251 ms                                                       | 264 ms: 1.05x slower                                               |
| float          | 74.9 ms                                                      | 79.6 ms: 1.06x slower                                              |
| Geometric mean | (ref)                                                        | 1.02x slower                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                               |
| regex_v8       | 24.4 ms                                                      | 23.8 ms: 1.03x faster                                              |
| regex_dna      | 227 ms                                                       | 238 ms: 1.05x slower                                               |
| regex_effbot   | 3.34 ms                                                      | 3.52 ms: 1.05x slower                                              |
| Geometric mean | (ref)                                                        | 1.00x slower                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                              |
| json_loads           | 28.9 us                                                      | 24.4 us: 1.19x faster                                              |
| unpickle_pure_python | 238 us                                                       | 212 us: 1.13x faster                                               |
| xml_etree_parse      | 155 ms                                                       | 146 ms: 1.06x faster                                               |
| tomli_loads          | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                             |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.03x faster                                               |
| pickle_pure_python   | 316 us                                                       | 326 us: 1.03x slower                                               |
| unpickle_list        | 4.60 us                                                      | 4.75 us: 1.03x slower                                              |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                              |
| xml_etree_process    | 55.9 ms                                                      | 58.9 ms: 1.05x slower                                              |
| xml_etree_generate   | 79.7 ms                                                      | 85.8 ms: 1.08x slower                                              |
| unpickle             | 13.3 us                                                      | 14.7 us: 1.11x slower                                              |
| pickle_list          | 3.94 us                                                      | 4.46 us: 1.13x slower                                              |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                       |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.7 ms: 1.09x slower                                              |
| python_startup_no_site | 7.73 ms                                                      | 8.67 ms: 1.12x slower                                              |
| Geometric mean         | (ref)                                                        | 1.11x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 9.92 ms: 1.11x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols | 532 us                                                       | 149 us: 3.57x faster                                               |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                             |
| asyncio_tcp              | 747 ms                                                       | 386 ms: 1.94x faster                                               |
| generators               | 54.6 ms                                                      | 36.7 ms: 1.49x faster                                              |
| json_dumps               | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                              |
| richards_super           | 63.6 ms                                                      | 50.5 ms: 1.26x faster                                              |
| fannkuch                 | 416 ms                                                       | 335 ms: 1.24x faster                                               |
| deltablue                | 3.97 ms                                                      | 3.29 ms: 1.21x faster                                              |
| chaos                    | 74.9 ms                                                      | 62.3 ms: 1.20x faster                                              |
| coroutines               | 27.8 ms                                                      | 23.3 ms: 1.19x faster                                              |
| json_loads               | 28.9 us                                                      | 24.4 us: 1.19x faster                                              |
| gc_traversal             | 4.15 ms                                                      | 3.54 ms: 1.17x faster                                              |
| hexiom                   | 6.98 ms                                                      | 5.97 ms: 1.17x faster                                              |
| scimark_lu               | 114 ms                                                       | 97.6 ms: 1.17x faster                                              |
| comprehensions           | 25.1 us                                                      | 21.8 us: 1.15x faster                                              |
| async_tree_memoization   | 629 ms                                                       | 552 ms: 1.14x faster                                               |
| async_tree_none          | 518 ms                                                       | 458 ms: 1.13x faster                                               |
| unpickle_pure_python     | 238 us                                                       | 212 us: 1.13x faster                                               |
| nqueens                  | 103 ms                                                       | 91.3 ms: 1.12x faster                                              |
| richards                 | 49.7 ms                                                      | 44.6 ms: 1.11x faster                                              |
| mako                     | 11.0 ms                                                      | 9.92 ms: 1.11x faster                                              |
| async_tree_io            | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                             |
| mdp                      | 2.77 sec                                                     | 2.52 sec: 1.10x faster                                             |
| json                     | 5.58 ms                                                      | 5.12 ms: 1.09x faster                                              |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 702 ms: 1.07x faster                                               |
| sqlglot_parse            | 1.51 ms                                                      | 1.41 ms: 1.07x faster                                              |
| regex_compile            | 156 ms                                                       | 146 ms: 1.07x faster                                               |
| pycparser                | 1.31 sec                                                     | 1.23 sec: 1.07x faster                                             |
| go                       | 158 ms                                                       | 148 ms: 1.06x faster                                               |
| nbody                    | 92.9 ms                                                      | 87.5 ms: 1.06x faster                                              |
| xml_etree_parse          | 155 ms                                                       | 146 ms: 1.06x faster                                               |
| logging_simple           | 7.24 us                                                      | 6.84 us: 1.06x faster                                              |
| sqlglot_transpile        | 1.91 ms                                                      | 1.81 ms: 1.06x faster                                              |
| logging_silent           | 100 ns                                                       | 95.9 ns: 1.05x faster                                              |
| spectral_norm            | 95.1 ms                                                      | 91.3 ms: 1.04x faster                                              |
| logging_format           | 7.71 us                                                      | 7.40 us: 1.04x faster                                              |
| tornado_http             | 124 ms                                                       | 120 ms: 1.04x faster                                               |
| dulwich_log              | 67.4 ms                                                      | 64.9 ms: 1.04x faster                                              |
| tomli_loads              | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                             |
| meteor_contest           | 131 ms                                                       | 126 ms: 1.04x faster                                               |
| xml_etree_iterparse      | 107 ms                                                       | 103 ms: 1.03x faster                                               |
| regex_v8                 | 24.4 ms                                                      | 23.8 ms: 1.03x faster                                              |
| bench_thread_pool        | 1.00 ms                                                      | 975 us: 1.03x faster                                               |
| deepcopy                 | 391 us                                                       | 382 us: 1.02x faster                                               |
| crypto_pyaes             | 83.3 ms                                                      | 81.5 ms: 1.02x faster                                              |
| pyflate                  | 449 ms                                                       | 443 ms: 1.02x faster                                               |
| sqlglot_normalize        | 122 ms                                                       | 120 ms: 1.01x faster                                               |
| sqlglot_optimize         | 59.0 ms                                                      | 58.6 ms: 1.01x faster                                              |
| scimark_monte_carlo      | 69.8 ms                                                      | 69.4 ms: 1.01x faster                                              |
| scimark_sor              | 110 ms                                                       | 111 ms: 1.01x slower                                               |
| pathlib                  | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                              |
| deepcopy_reduce          | 3.40 us                                                      | 3.45 us: 1.02x slower                                              |
| pprint_safe_repr         | 805 ms                                                       | 820 ms: 1.02x slower                                               |
| docutils                 | 2.85 sec                                                     | 2.90 sec: 1.02x slower                                             |
| telco                    | 6.81 ms                                                      | 6.99 ms: 1.03x slower                                              |
| scimark_fft              | 281 ms                                                       | 288 ms: 1.03x slower                                               |
| pickle_pure_python       | 316 us                                                       | 326 us: 1.03x slower                                               |
| unpickle_list            | 4.60 us                                                      | 4.75 us: 1.03x slower                                              |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.21 ms: 1.04x slower                                              |
| regex_dna                | 227 ms                                                       | 238 ms: 1.05x slower                                               |
| pidigits                 | 251 ms                                                       | 264 ms: 1.05x slower                                               |
| regex_effbot             | 3.34 ms                                                      | 3.52 ms: 1.05x slower                                              |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                              |
| xml_etree_process        | 55.9 ms                                                      | 58.9 ms: 1.05x slower                                              |
| create_gc_cycles         | 1.58 ms                                                      | 1.66 ms: 1.05x slower                                              |
| float                    | 74.9 ms                                                      | 79.6 ms: 1.06x slower                                              |
| xml_etree_generate       | 79.7 ms                                                      | 85.8 ms: 1.08x slower                                              |
| sqlite_synth             | 2.52 us                                                      | 2.72 us: 1.08x slower                                              |
| python_startup           | 10.7 ms                                                      | 11.7 ms: 1.09x slower                                              |
| unpickle                 | 13.3 us                                                      | 14.7 us: 1.11x slower                                              |
| python_startup_no_site   | 7.73 ms                                                      | 8.67 ms: 1.12x slower                                              |
| pickle_list              | 3.94 us                                                      | 4.46 us: 1.13x slower                                              |
| unpack_sequence          | 45.7 ns                                                      | 53.7 ns: 1.18x slower                                              |
| async_generators         | 322 ms                                                       | 381 ms: 1.19x slower                                               |
| coverage                 | 66.1 ms                                                      | 88.0 ms: 1.33x slower                                              |
| dask                     | 410 ms                                                       | 566 ms: 1.38x slower                                               |
| Geometric mean           | (ref)                                                        | 1.06x faster                                                       |

Benchmark hidden because not significant (6): raytrace, pprint_pformat, 2to3, pickle_dict, deepcopy_memo, bench_mp_pool
Ignored benchmarks (22) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.73% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.16x