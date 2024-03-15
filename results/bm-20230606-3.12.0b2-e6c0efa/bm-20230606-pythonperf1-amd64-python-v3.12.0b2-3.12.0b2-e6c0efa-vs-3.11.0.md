
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b2
- machine: windows-amd64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.96%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 216 ms: 1.01x slower                                            |
| docutils       | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                          |
| tornado_http   | 92.8 ms                                                     | 88.5 ms: 1.05x faster                                           |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 347 ms: 1.15x faster                                            |
| async_tree_none         | 332 ms                                                      | 298 ms: 1.12x faster                                            |
| async_tree_io           | 808 ms                                                      | 744 ms: 1.08x faster                                            |
| async_tree_cpu_io_mixed | 530 ms                                                      | 493 ms: 1.08x faster                                            |
| Geometric mean          | (ref)                                                       | 1.11x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 68.3 ms: 1.03x faster                                           |
| float          | 54.4 ms                                                     | 55.2 ms: 1.01x slower                                           |
| pidigits       | 150 ms                                                      | 153 ms: 1.02x slower                                            |
| Geometric mean | (ref)                                                       | 1.00x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 87.9 ms: 1.04x faster                                           |
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| regex_dna      | 116 ms                                                      | 125 ms: 1.07x slower                                            |
| regex_effbot   | 1.50 ms                                                     | 1.63 ms: 1.08x slower                                           |
| Geometric mean | (ref)                                                       | 1.02x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                           |
| unpickle_pure_python | 157 us                                                      | 135 us: 1.16x faster                                            |
| xml_etree_parse      | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                           |
| tomli_loads          | 1.46 sec                                                    | 1.37 sec: 1.06x faster                                          |
| pickle_pure_python   | 208 us                                                      | 197 us: 1.06x faster                                            |
| pickle_dict          | 18.5 us                                                     | 18.2 us: 1.02x faster                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 65.0 ms: 1.01x faster                                           |
| xml_etree_process    | 37.2 ms                                                     | 38.3 ms: 1.03x slower                                           |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                           |
| pickle_list          | 2.70 us                                                     | 2.85 us: 1.06x slower                                           |
| pickle               | 6.64 us                                                     | 7.11 us: 1.07x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 57.0 ms: 1.08x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.90 us: 1.12x slower                                           |
| unpickle             | 7.57 us                                                     | 8.48 us: 1.12x slower                                           |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.2 ms: 1.02x slower                                           |
| python_startup_no_site | 16.8 ms                                                     | 17.4 ms: 1.03x slower                                           |
| Geometric mean         | (ref)                                                       | 1.03x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.05 ms: 1.08x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 326 us                                                      | 95.0 us: 3.43x faster                                           |
| asyncio_tcp              | 726 ms                                                      | 478 ms: 1.52x faster                                            |
| generators               | 34.0 ms                                                     | 22.4 ms: 1.51x faster                                           |
| json_dumps               | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                           |
| richards_super           | 38.7 ms                                                     | 29.2 ms: 1.32x faster                                           |
| deltablue                | 2.70 ms                                                     | 2.08 ms: 1.30x faster                                           |
| richards                 | 31.4 ms                                                     | 25.7 ms: 1.22x faster                                           |
| logging_silent           | 71.8 ns                                                     | 59.4 ns: 1.21x faster                                           |
| unpack_sequence          | 46.9 ns                                                     | 39.1 ns: 1.20x faster                                           |
| sqlglot_parse            | 953 us                                                      | 799 us: 1.19x faster                                            |
| unpickle_pure_python     | 157 us                                                      | 135 us: 1.16x faster                                            |
| mdp                      | 1.59 sec                                                    | 1.38 sec: 1.16x faster                                          |
| sqlglot_transpile        | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                           |
| go                       | 101 ms                                                      | 87.8 ms: 1.15x faster                                           |
| async_tree_memoization   | 399 ms                                                      | 347 ms: 1.15x faster                                            |
| raytrace                 | 213 ms                                                      | 187 ms: 1.14x faster                                            |
| hexiom                   | 4.55 ms                                                     | 4.00 ms: 1.14x faster                                           |
| chaos                    | 48.4 ms                                                     | 42.8 ms: 1.13x faster                                           |
| nqueens                  | 68.3 ms                                                     | 61.1 ms: 1.12x faster                                           |
| async_tree_none          | 332 ms                                                      | 298 ms: 1.12x faster                                            |
| scimark_lu               | 62.8 ms                                                     | 56.8 ms: 1.10x faster                                           |
| deepcopy_memo            | 26.0 us                                                     | 23.8 us: 1.09x faster                                           |
| comprehensions           | 15.6 us                                                     | 14.4 us: 1.09x faster                                           |
| async_tree_io            | 808 ms                                                      | 744 ms: 1.08x faster                                            |
| coroutines               | 15.0 ms                                                     | 13.9 ms: 1.08x faster                                           |
| mako                     | 7.58 ms                                                     | 7.05 ms: 1.08x faster                                           |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 493 ms: 1.08x faster                                            |
| xml_etree_parse          | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                           |
| scimark_monte_carlo      | 45.3 ms                                                     | 42.6 ms: 1.06x faster                                           |
| tomli_loads              | 1.46 sec                                                    | 1.37 sec: 1.06x faster                                          |
| pickle_pure_python       | 208 us                                                      | 197 us: 1.06x faster                                            |
| pycparser                | 720 ms                                                      | 680 ms: 1.06x faster                                            |
| fannkuch                 | 253 ms                                                      | 240 ms: 1.06x faster                                            |
| pyflate                  | 312 ms                                                      | 296 ms: 1.06x faster                                            |
| pprint_pformat           | 1.09 sec                                                    | 1.03 sec: 1.05x faster                                          |
| logging_simple           | 6.86 us                                                     | 6.54 us: 1.05x faster                                           |
| dulwich_log              | 46.4 ms                                                     | 44.2 ms: 1.05x faster                                           |
| tornado_http             | 92.8 ms                                                     | 88.5 ms: 1.05x faster                                           |
| sqlglot_normalize        | 190 ms                                                      | 183 ms: 1.04x faster                                            |
| pprint_safe_repr         | 529 ms                                                      | 510 ms: 1.04x faster                                            |
| spectral_norm            | 68.3 ms                                                     | 66.0 ms: 1.04x faster                                           |
| regex_compile            | 91.0 ms                                                     | 87.9 ms: 1.04x faster                                           |
| crypto_pyaes             | 48.9 ms                                                     | 47.2 ms: 1.04x faster                                           |
| scimark_fft              | 179 ms                                                      | 174 ms: 1.03x faster                                            |
| nbody                    | 70.3 ms                                                     | 68.3 ms: 1.03x faster                                           |
| logging_format           | 7.16 us                                                     | 7.01 us: 1.02x faster                                           |
| deepcopy                 | 246 us                                                      | 241 us: 1.02x faster                                            |
| sqlglot_optimize         | 34.5 ms                                                     | 33.8 ms: 1.02x faster                                           |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.52 ms: 1.02x faster                                           |
| meteor_contest           | 75.2 ms                                                     | 73.9 ms: 1.02x faster                                           |
| regex_v8                 | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| pickle_dict              | 18.5 us                                                     | 18.2 us: 1.02x faster                                           |
| scimark_sor              | 78.1 ms                                                     | 77.3 ms: 1.01x faster                                           |
| xml_etree_iterparse      | 65.6 ms                                                     | 65.0 ms: 1.01x faster                                           |
| 2to3                     | 214 ms                                                      | 216 ms: 1.01x slower                                            |
| sqlite_synth             | 1.77 us                                                     | 1.79 us: 1.01x slower                                           |
| float                    | 54.4 ms                                                     | 55.2 ms: 1.01x slower                                           |
| docutils                 | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                          |
| deepcopy_reduce          | 2.06 us                                                     | 2.10 us: 1.02x slower                                           |
| telco                    | 4.06 ms                                                     | 4.15 ms: 1.02x slower                                           |
| pidigits                 | 150 ms                                                      | 153 ms: 1.02x slower                                            |
| python_startup           | 19.8 ms                                                     | 20.2 ms: 1.02x slower                                           |
| gc_traversal             | 1.49 ms                                                     | 1.53 ms: 1.02x slower                                           |
| xml_etree_process        | 37.2 ms                                                     | 38.3 ms: 1.03x slower                                           |
| python_startup_no_site   | 16.8 ms                                                     | 17.4 ms: 1.03x slower                                           |
| create_gc_cycles         | 713 us                                                      | 744 us: 1.04x slower                                            |
| json_loads               | 13.0 us                                                     | 13.7 us: 1.06x slower                                           |
| pickle_list              | 2.70 us                                                     | 2.85 us: 1.06x slower                                           |
| pickle                   | 6.64 us                                                     | 7.11 us: 1.07x slower                                           |
| regex_dna                | 116 ms                                                      | 125 ms: 1.07x slower                                            |
| bench_mp_pool            | 63.2 ms                                                     | 68.0 ms: 1.08x slower                                           |
| xml_etree_generate       | 52.5 ms                                                     | 57.0 ms: 1.08x slower                                           |
| regex_effbot             | 1.50 ms                                                     | 1.63 ms: 1.08x slower                                           |
| unpickle_list            | 2.59 us                                                     | 2.90 us: 1.12x slower                                           |
| unpickle                 | 7.57 us                                                     | 8.48 us: 1.12x slower                                           |
| pathlib                  | 70.9 ms                                                     | 83.2 ms: 1.17x slower                                           |
| coverage                 | 43.4 ms                                                     | 52.5 ms: 1.21x slower                                           |
| async_generators         | 177 ms                                                      | 233 ms: 1.32x slower                                            |
| dask                     | 273 ms                                                      | 373 ms: 1.37x slower                                            |
| Geometric mean           | (ref)                                                       | 1.06x faster                                                    |

Benchmark hidden because not significant (4): bench_thread_pool, aiohttp, json, asyncio_tcp_ssl
Ignored benchmarks (19) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown