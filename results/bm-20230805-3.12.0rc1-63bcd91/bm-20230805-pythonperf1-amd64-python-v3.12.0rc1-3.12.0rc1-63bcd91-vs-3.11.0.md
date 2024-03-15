
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0rc1
- machine: windows-amd64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 211 ms: 1.01x faster                                              |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                            |
| tornado_http   | 92.8 ms                                                     | 87.2 ms: 1.06x faster                                             |
| Geometric mean | (ref)                                                       | 1.03x faster                                                      |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 331 ms: 1.21x faster                                              |
| async_tree_none         | 332 ms                                                      | 286 ms: 1.16x faster                                              |
| async_tree_io           | 808 ms                                                      | 701 ms: 1.15x faster                                              |
| async_tree_cpu_io_mixed | 530 ms                                                      | 471 ms: 1.13x faster                                              |
| Geometric mean          | (ref)                                                       | 1.16x faster                                                      |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 68.7 ms: 1.02x faster                                             |
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                              |
| float          | 54.4 ms                                                     | 53.8 ms: 1.01x faster                                             |
| Geometric mean | (ref)                                                       | 1.02x faster                                                      |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 85.8 ms: 1.06x faster                                             |
| regex_v8       | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                             |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                              |
| regex_effbot   | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                             |
| Geometric mean | (ref)                                                       | 1.01x slower                                                      |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                             |
| unpickle_pure_python | 157 us                                                      | 133 us: 1.18x faster                                              |
| pickle_pure_python   | 208 us                                                      | 191 us: 1.09x faster                                              |
| tomli_loads          | 1.46 sec                                                    | 1.35 sec: 1.08x faster                                            |
| xml_etree_parse      | 97.6 ms                                                     | 91.3 ms: 1.07x faster                                             |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.1 ms: 1.04x faster                                             |
| pickle_dict          | 18.5 us                                                     | 18.3 us: 1.01x faster                                             |
| xml_etree_process    | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                             |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                             |
| xml_etree_generate   | 52.5 ms                                                     | 55.1 ms: 1.05x slower                                             |
| pickle               | 6.64 us                                                     | 6.98 us: 1.05x slower                                             |
| pickle_list          | 2.70 us                                                     | 2.87 us: 1.07x slower                                             |
| unpickle_list        | 2.59 us                                                     | 2.79 us: 1.08x slower                                             |
| unpickle             | 7.57 us                                                     | 8.38 us: 1.11x slower                                             |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                      |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 18.7 ms: 1.05x faster                                             |
| python_startup_no_site | 16.8 ms                                                     | 16.1 ms: 1.05x faster                                             |
| Geometric mean         | (ref)                                                       | 1.05x faster                                                      |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.82 ms: 1.11x faster                                             |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| typing_runtime_protocols | 326 us                                                      | 93.3 us: 3.49x faster                                             |
| asyncio_tcp              | 726 ms                                                      | 470 ms: 1.54x faster                                              |
| generators               | 34.0 ms                                                     | 22.5 ms: 1.51x faster                                             |
| json_dumps               | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                             |
| unpack_sequence          | 46.9 ns                                                     | 35.1 ns: 1.33x faster                                             |
| richards_super           | 38.7 ms                                                     | 29.5 ms: 1.31x faster                                             |
| deltablue                | 2.70 ms                                                     | 2.13 ms: 1.27x faster                                             |
| async_tree_memoization   | 399 ms                                                      | 331 ms: 1.21x faster                                              |
| richards                 | 31.4 ms                                                     | 26.1 ms: 1.20x faster                                             |
| logging_silent           | 71.8 ns                                                     | 60.0 ns: 1.20x faster                                             |
| sqlglot_parse            | 953 us                                                      | 800 us: 1.19x faster                                              |
| unpickle_pure_python     | 157 us                                                      | 133 us: 1.18x faster                                              |
| go                       | 101 ms                                                      | 86.3 ms: 1.17x faster                                             |
| async_tree_none          | 332 ms                                                      | 286 ms: 1.16x faster                                              |
| raytrace                 | 213 ms                                                      | 184 ms: 1.16x faster                                              |
| async_tree_io            | 808 ms                                                      | 701 ms: 1.15x faster                                              |
| sqlglot_transpile        | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                             |
| hexiom                   | 4.55 ms                                                     | 3.98 ms: 1.14x faster                                             |
| deepcopy_memo            | 26.0 us                                                     | 22.9 us: 1.14x faster                                             |
| chaos                    | 48.4 ms                                                     | 42.8 ms: 1.13x faster                                             |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 471 ms: 1.13x faster                                              |
| mdp                      | 1.59 sec                                                    | 1.43 sec: 1.12x faster                                            |
| mako                     | 7.58 ms                                                     | 6.82 ms: 1.11x faster                                             |
| nqueens                  | 68.3 ms                                                     | 61.6 ms: 1.11x faster                                             |
| comprehensions           | 15.6 us                                                     | 14.1 us: 1.11x faster                                             |
| scimark_lu               | 62.8 ms                                                     | 57.1 ms: 1.10x faster                                             |
| scimark_monte_carlo      | 45.3 ms                                                     | 41.5 ms: 1.09x faster                                             |
| pickle_pure_python       | 208 us                                                      | 191 us: 1.09x faster                                              |
| dulwich_log              | 46.4 ms                                                     | 42.5 ms: 1.09x faster                                             |
| tomli_loads              | 1.46 sec                                                    | 1.35 sec: 1.08x faster                                            |
| logging_simple           | 6.86 us                                                     | 6.37 us: 1.08x faster                                             |
| fannkuch                 | 253 ms                                                      | 236 ms: 1.08x faster                                              |
| deepcopy                 | 246 us                                                      | 229 us: 1.08x faster                                              |
| pycparser                | 720 ms                                                      | 670 ms: 1.07x faster                                              |
| pyflate                  | 312 ms                                                      | 292 ms: 1.07x faster                                              |
| xml_etree_parse          | 97.6 ms                                                     | 91.3 ms: 1.07x faster                                             |
| coroutines               | 15.0 ms                                                     | 14.0 ms: 1.07x faster                                             |
| asyncio_tcp_ssl          | 2.03 sec                                                    | 1.90 sec: 1.07x faster                                            |
| tornado_http             | 92.8 ms                                                     | 87.2 ms: 1.06x faster                                             |
| pprint_pformat           | 1.09 sec                                                    | 1.02 sec: 1.06x faster                                            |
| regex_compile            | 91.0 ms                                                     | 85.8 ms: 1.06x faster                                             |
| spectral_norm            | 68.3 ms                                                     | 64.4 ms: 1.06x faster                                             |
| sqlglot_normalize        | 190 ms                                                      | 180 ms: 1.06x faster                                              |
| logging_format           | 7.16 us                                                     | 6.77 us: 1.06x faster                                             |
| python_startup           | 19.8 ms                                                     | 18.7 ms: 1.05x faster                                             |
| pprint_safe_repr         | 529 ms                                                      | 504 ms: 1.05x faster                                              |
| python_startup_no_site   | 16.8 ms                                                     | 16.1 ms: 1.05x faster                                             |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.47 ms: 1.04x faster                                             |
| crypto_pyaes             | 48.9 ms                                                     | 46.9 ms: 1.04x faster                                             |
| xml_etree_iterparse      | 65.6 ms                                                     | 63.1 ms: 1.04x faster                                             |
| aiohttp                  | 883 us                                                      | 854 us: 1.03x faster                                              |
| scimark_fft              | 179 ms                                                      | 174 ms: 1.03x faster                                              |
| sqlglot_optimize         | 34.5 ms                                                     | 33.5 ms: 1.03x faster                                             |
| meteor_contest           | 75.2 ms                                                     | 73.1 ms: 1.03x faster                                             |
| regex_v8                 | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                             |
| docutils                 | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                            |
| nbody                    | 70.3 ms                                                     | 68.7 ms: 1.02x faster                                             |
| telco                    | 4.06 ms                                                     | 3.98 ms: 1.02x faster                                             |
| pidigits                 | 150 ms                                                      | 147 ms: 1.02x faster                                              |
| sqlite_synth             | 1.77 us                                                     | 1.73 us: 1.02x faster                                             |
| gc_traversal             | 1.49 ms                                                     | 1.47 ms: 1.01x faster                                             |
| pickle_dict              | 18.5 us                                                     | 18.3 us: 1.01x faster                                             |
| 2to3                     | 214 ms                                                      | 211 ms: 1.01x faster                                              |
| float                    | 54.4 ms                                                     | 53.8 ms: 1.01x faster                                             |
| scimark_sor              | 78.1 ms                                                     | 78.7 ms: 1.01x slower                                             |
| deepcopy_reduce          | 2.06 us                                                     | 2.08 us: 1.01x slower                                             |
| xml_etree_process        | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                             |
| json_loads               | 13.0 us                                                     | 13.5 us: 1.04x slower                                             |
| regex_dna                | 116 ms                                                      | 121 ms: 1.04x slower                                              |
| xml_etree_generate       | 52.5 ms                                                     | 55.1 ms: 1.05x slower                                             |
| bench_mp_pool            | 63.2 ms                                                     | 66.3 ms: 1.05x slower                                             |
| pickle                   | 6.64 us                                                     | 6.98 us: 1.05x slower                                             |
| pickle_list              | 2.70 us                                                     | 2.87 us: 1.07x slower                                             |
| regex_effbot             | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                             |
| unpickle_list            | 2.59 us                                                     | 2.79 us: 1.08x slower                                             |
| pathlib                  | 70.9 ms                                                     | 78.1 ms: 1.10x slower                                             |
| unpickle                 | 7.57 us                                                     | 8.38 us: 1.11x slower                                             |
| coverage                 | 43.4 ms                                                     | 52.1 ms: 1.20x slower                                             |
| async_generators         | 177 ms                                                      | 229 ms: 1.29x slower                                              |
| dask                     | 273 ms                                                      | 361 ms: 1.32x slower                                              |
| Geometric mean           | (ref)                                                       | 1.08x faster                                                      |

Benchmark hidden because not significant (3): bench_thread_pool, json, create_gc_cycles
Ignored benchmarks (19) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown