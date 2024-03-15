
# Results vs. 3.11.0

- fork: python
- ref: v3.11.6
- machine: windows-amd64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.96%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 207 ms: 1.03x faster                                        |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                      |
| tornado_http   | 92.8 ms                                                     | 90.5 ms: 1.03x faster                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (2): chameleon, html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_none         | 332 ms                                                      | 311 ms: 1.07x faster                                        |
| async_tree_memoization  | 399 ms                                                      | 375 ms: 1.06x faster                                        |
| async_tree_io           | 808 ms                                                      | 778 ms: 1.04x faster                                        |
| async_tree_cpu_io_mixed | 530 ms                                                      | 515 ms: 1.03x faster                                        |
| Geometric mean          | (ref)                                                       | 1.05x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.01x faster                                        |
| nbody          | 70.3 ms                                                     | 69.7 ms: 1.01x faster                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 91.7 ms: 1.01x slower                                       |
| regex_effbot   | 1.50 ms                                                     | 1.53 ms: 1.02x slower                                       |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                        |
| Geometric mean | (ref)                                                       | 1.02x slower                                                |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 7.74 ms: 1.05x faster                                       |
| unpickle_pure_python | 157 us                                                      | 151 us: 1.04x faster                                        |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                       |
| tomli_loads          | 1.46 sec                                                    | 1.42 sec: 1.03x faster                                      |
| pickle_pure_python   | 208 us                                                      | 203 us: 1.03x faster                                        |
| pickle               | 6.64 us                                                     | 6.67 us: 1.01x slower                                       |
| xml_etree_generate   | 52.5 ms                                                     | 52.9 ms: 1.01x slower                                       |
| unpickle             | 7.57 us                                                     | 7.67 us: 1.01x slower                                       |
| json_loads           | 13.0 us                                                     | 13.2 us: 1.01x slower                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                       |
| unpickle_list        | 2.59 us                                                     | 2.64 us: 1.02x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (3): xml_etree_parse, pickle_dict, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.6 ms: 1.08x faster                                       |
| python_startup         | 19.8 ms                                                     | 18.6 ms: 1.06x faster                                       |
| Geometric mean         | (ref)                                                       | 1.07x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.2 ms: 1.07x faster                                       |
| genshi_xml      | 39.9 ms                                                     | 38.1 ms: 1.05x faster                                       |
| django_template | 24.4 ms                                                     | 23.6 ms: 1.04x faster                                       |
| mako            | 7.58 ms                                                     | 7.31 ms: 1.04x faster                                       |
| Geometric mean  | (ref)                                                       | 1.05x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site   | 16.8 ms                                                     | 15.6 ms: 1.08x faster                                       |
| bench_mp_pool            | 63.2 ms                                                     | 58.7 ms: 1.08x faster                                       |
| genshi_text              | 18.4 ms                                                     | 17.2 ms: 1.07x faster                                       |
| nqueens                  | 68.3 ms                                                     | 63.7 ms: 1.07x faster                                       |
| async_tree_none          | 332 ms                                                      | 311 ms: 1.07x faster                                        |
| async_tree_memoization   | 399 ms                                                      | 375 ms: 1.06x faster                                        |
| python_startup           | 19.8 ms                                                     | 18.6 ms: 1.06x faster                                       |
| raytrace                 | 213 ms                                                      | 203 ms: 1.05x faster                                        |
| fannkuch                 | 253 ms                                                      | 241 ms: 1.05x faster                                        |
| genshi_xml               | 39.9 ms                                                     | 38.1 ms: 1.05x faster                                       |
| json_dumps               | 8.09 ms                                                     | 7.74 ms: 1.05x faster                                       |
| unpickle_pure_python     | 157 us                                                      | 151 us: 1.04x faster                                        |
| dask                     | 273 ms                                                      | 263 ms: 1.04x faster                                        |
| django_template          | 24.4 ms                                                     | 23.6 ms: 1.04x faster                                       |
| mako                     | 7.58 ms                                                     | 7.31 ms: 1.04x faster                                       |
| pycparser                | 720 ms                                                      | 694 ms: 1.04x faster                                        |
| async_tree_io            | 808 ms                                                      | 778 ms: 1.04x faster                                        |
| aiohttp                  | 883 us                                                      | 853 us: 1.04x faster                                        |
| xml_etree_iterparse      | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                       |
| telco                    | 4.06 ms                                                     | 3.93 ms: 1.03x faster                                       |
| pathlib                  | 70.9 ms                                                     | 68.5 ms: 1.03x faster                                       |
| dulwich_log              | 46.4 ms                                                     | 45.0 ms: 1.03x faster                                       |
| 2to3                     | 214 ms                                                      | 207 ms: 1.03x faster                                        |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 515 ms: 1.03x faster                                        |
| tomli_loads              | 1.46 sec                                                    | 1.42 sec: 1.03x faster                                      |
| deepcopy_memo            | 26.0 us                                                     | 25.3 us: 1.03x faster                                       |
| deltablue                | 2.70 ms                                                     | 2.63 ms: 1.03x faster                                       |
| sqlite_synth             | 1.77 us                                                     | 1.72 us: 1.03x faster                                       |
| pickle_pure_python       | 208 us                                                      | 203 us: 1.03x faster                                        |
| tornado_http             | 92.8 ms                                                     | 90.5 ms: 1.03x faster                                       |
| richards                 | 31.4 ms                                                     | 30.6 ms: 1.03x faster                                       |
| pyflate                  | 312 ms                                                      | 305 ms: 1.02x faster                                        |
| pprint_safe_repr         | 529 ms                                                      | 517 ms: 1.02x faster                                        |
| pprint_pformat           | 1.09 sec                                                    | 1.06 sec: 1.02x faster                                      |
| bench_thread_pool        | 872 us                                                      | 852 us: 1.02x faster                                        |
| docutils                 | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                      |
| logging_simple           | 6.86 us                                                     | 6.72 us: 1.02x faster                                       |
| sqlalchemy_declarative   | 85.6 ms                                                     | 83.8 ms: 1.02x faster                                       |
| sqlglot_transpile        | 1.16 ms                                                     | 1.14 ms: 1.02x faster                                       |
| coroutines               | 15.0 ms                                                     | 14.7 ms: 1.02x faster                                       |
| scimark_sor              | 78.1 ms                                                     | 76.8 ms: 1.02x faster                                       |
| sympy_integrate          | 14.0 ms                                                     | 13.8 ms: 1.02x faster                                       |
| sqlalchemy_imperative    | 10.4 ms                                                     | 10.3 ms: 1.02x faster                                       |
| sqlglot_parse            | 953 us                                                      | 938 us: 1.02x faster                                        |
| logging_silent           | 71.8 ns                                                     | 70.7 ns: 1.02x faster                                       |
| thrift                   | 494 us                                                      | 487 us: 1.01x faster                                        |
| scimark_lu               | 62.8 ms                                                     | 61.9 ms: 1.01x faster                                       |
| unpack_sequence          | 46.9 ns                                                     | 46.3 ns: 1.01x faster                                       |
| spectral_norm            | 68.3 ms                                                     | 67.5 ms: 1.01x faster                                       |
| pidigits                 | 150 ms                                                      | 148 ms: 1.01x faster                                        |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.55 ms: 1.01x faster                                       |
| richards_super           | 38.7 ms                                                     | 38.4 ms: 1.01x faster                                       |
| nbody                    | 70.3 ms                                                     | 69.7 ms: 1.01x faster                                       |
| gc_traversal             | 1.49 ms                                                     | 1.48 ms: 1.01x faster                                       |
| generators               | 34.0 ms                                                     | 33.7 ms: 1.01x faster                                       |
| typing_runtime_protocols | 326 us                                                      | 324 us: 1.00x faster                                        |
| flaskblogging            | 2.03 sec                                                    | 2.03 sec: 1.00x slower                                      |
| pickle                   | 6.64 us                                                     | 6.67 us: 1.01x slower                                       |
| xml_etree_generate       | 52.5 ms                                                     | 52.9 ms: 1.01x slower                                       |
| regex_compile            | 91.0 ms                                                     | 91.7 ms: 1.01x slower                                       |
| crypto_pyaes             | 48.9 ms                                                     | 49.3 ms: 1.01x slower                                       |
| go                       | 101 ms                                                      | 102 ms: 1.01x slower                                        |
| scimark_fft              | 179 ms                                                      | 181 ms: 1.01x slower                                        |
| async_generators         | 177 ms                                                      | 179 ms: 1.01x slower                                        |
| sqlglot_normalize        | 190 ms                                                      | 192 ms: 1.01x slower                                        |
| meteor_contest           | 75.2 ms                                                     | 76.1 ms: 1.01x slower                                       |
| sympy_str                | 185 ms                                                      | 187 ms: 1.01x slower                                        |
| unpickle                 | 7.57 us                                                     | 7.67 us: 1.01x slower                                       |
| json_loads               | 13.0 us                                                     | 13.2 us: 1.01x slower                                       |
| sqlglot_optimize         | 34.5 ms                                                     | 35.1 ms: 1.01x slower                                       |
| xml_etree_process        | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                       |
| sympy_sum                | 100 ms                                                      | 102 ms: 1.02x slower                                        |
| deepcopy_reduce          | 2.06 us                                                     | 2.10 us: 1.02x slower                                       |
| regex_effbot             | 1.50 ms                                                     | 1.53 ms: 1.02x slower                                       |
| unpickle_list            | 2.59 us                                                     | 2.64 us: 1.02x slower                                       |
| scimark_monte_carlo      | 45.3 ms                                                     | 46.3 ms: 1.02x slower                                       |
| sympy_expand             | 299 ms                                                      | 305 ms: 1.02x slower                                        |
| chaos                    | 48.4 ms                                                     | 49.7 ms: 1.03x slower                                       |
| regex_dna                | 116 ms                                                      | 122 ms: 1.05x slower                                        |
| mdp                      | 1.59 sec                                                    | 1.71 sec: 1.08x slower                                      |
| coverage                 | 43.4 ms                                                     | 53.6 ms: 1.23x slower                                       |
| Geometric mean           | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (16): pylint, create_gc_cycles, chameleon, xml_etree_parse, pickle_dict, hexiom, deepcopy, float, html5lib, regex_v8, pickle_list, logging_format, asyncio_tcp, comprehensions, json, asyncio_tcp_ssl
Ignored benchmarks (5) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown