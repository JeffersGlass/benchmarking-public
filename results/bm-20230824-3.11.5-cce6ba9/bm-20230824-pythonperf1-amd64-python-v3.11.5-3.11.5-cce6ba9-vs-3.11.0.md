
# Results vs. 3.11.0

- fork: python
- ref: v3.11.5
- machine: windows-amd64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.01x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 208 ms: 1.02x faster                                        |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                      |
| tornado_http   | 92.8 ms                                                     | 90.6 ms: 1.02x faster                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (2): chameleon, html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_none         | 332 ms                                                      | 311 ms: 1.07x faster                                        |
| async_tree_memoization  | 399 ms                                                      | 375 ms: 1.06x faster                                        |
| async_tree_io           | 808 ms                                                      | 779 ms: 1.04x faster                                        |
| async_tree_cpu_io_mixed | 530 ms                                                      | 516 ms: 1.03x faster                                        |
| Geometric mean          | (ref)                                                       | 1.05x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.02x faster                                        |
| float          | 54.4 ms                                                     | 53.9 ms: 1.01x faster                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                       |
| regex_effbot   | 1.50 ms                                                     | 1.49 ms: 1.01x faster                                       |
| regex_dna      | 116 ms                                                      | 117 ms: 1.01x slower                                        |
| Geometric mean | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 7.63 ms: 1.06x faster                                       |
| unpickle_pure_python | 157 us                                                      | 151 us: 1.04x faster                                        |
| tomli_loads          | 1.46 sec                                                    | 1.41 sec: 1.04x faster                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.4 ms: 1.04x faster                                       |
| pickle_pure_python   | 208 us                                                      | 202 us: 1.03x faster                                        |
| xml_etree_generate   | 52.5 ms                                                     | 51.8 ms: 1.01x faster                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                       |
| unpickle_list        | 2.59 us                                                     | 2.60 us: 1.00x slower                                       |
| pickle_list          | 2.70 us                                                     | 2.75 us: 1.02x slower                                       |
| pickle               | 6.64 us                                                     | 6.86 us: 1.03x slower                                       |
| unpickle             | 7.57 us                                                     | 7.92 us: 1.05x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (3): xml_etree_parse, json_loads, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 16.5 ms: 1.02x faster                                       |
| python_startup         | 19.8 ms                                                     | 19.4 ms: 1.02x faster                                       |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.5 ms: 1.05x faster                                       |
| genshi_xml      | 39.9 ms                                                     | 38.0 ms: 1.05x faster                                       |
| django_template | 24.4 ms                                                     | 23.9 ms: 1.02x faster                                       |
| mako            | 7.58 ms                                                     | 7.44 ms: 1.02x faster                                       |
| Geometric mean  | (ref)                                                       | 1.04x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| nqueens                  | 68.3 ms                                                     | 62.3 ms: 1.10x faster                                       |
| async_tree_none          | 332 ms                                                      | 311 ms: 1.07x faster                                        |
| async_tree_memoization   | 399 ms                                                      | 375 ms: 1.06x faster                                        |
| dulwich_log              | 46.4 ms                                                     | 43.6 ms: 1.06x faster                                       |
| json_dumps               | 8.09 ms                                                     | 7.63 ms: 1.06x faster                                       |
| genshi_text              | 18.4 ms                                                     | 17.5 ms: 1.05x faster                                       |
| genshi_xml               | 39.9 ms                                                     | 38.0 ms: 1.05x faster                                       |
| raytrace                 | 213 ms                                                      | 203 ms: 1.05x faster                                        |
| deepcopy_memo            | 26.0 us                                                     | 24.7 us: 1.05x faster                                       |
| logging_simple           | 6.86 us                                                     | 6.56 us: 1.05x faster                                       |
| richards                 | 31.4 ms                                                     | 30.1 ms: 1.04x faster                                       |
| unpickle_pure_python     | 157 us                                                      | 151 us: 1.04x faster                                        |
| async_tree_io            | 808 ms                                                      | 779 ms: 1.04x faster                                        |
| tomli_loads              | 1.46 sec                                                    | 1.41 sec: 1.04x faster                                      |
| xml_etree_iterparse      | 65.6 ms                                                     | 63.4 ms: 1.04x faster                                       |
| aiohttp                  | 883 us                                                      | 853 us: 1.03x faster                                        |
| pickle_pure_python       | 208 us                                                      | 202 us: 1.03x faster                                        |
| deltablue                | 2.70 ms                                                     | 2.61 ms: 1.03x faster                                       |
| pyflate                  | 312 ms                                                      | 302 ms: 1.03x faster                                        |
| coroutines               | 15.0 ms                                                     | 14.5 ms: 1.03x faster                                       |
| pprint_pformat           | 1.09 sec                                                    | 1.05 sec: 1.03x faster                                      |
| pprint_safe_repr         | 529 ms                                                      | 513 ms: 1.03x faster                                        |
| dask                     | 273 ms                                                      | 265 ms: 1.03x faster                                        |
| unpack_sequence          | 46.9 ns                                                     | 45.5 ns: 1.03x faster                                       |
| regex_v8                 | 14.2 ms                                                     | 13.8 ms: 1.03x faster                                       |
| sqlglot_transpile        | 1.16 ms                                                     | 1.13 ms: 1.03x faster                                       |
| pycparser                | 720 ms                                                      | 699 ms: 1.03x faster                                        |
| sqlite_synth             | 1.77 us                                                     | 1.72 us: 1.03x faster                                       |
| bench_mp_pool            | 63.2 ms                                                     | 61.5 ms: 1.03x faster                                       |
| sqlglot_parse            | 953 us                                                      | 928 us: 1.03x faster                                        |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 516 ms: 1.03x faster                                        |
| telco                    | 4.06 ms                                                     | 3.96 ms: 1.03x faster                                       |
| 2to3                     | 214 ms                                                      | 208 ms: 1.02x faster                                        |
| django_template          | 24.4 ms                                                     | 23.9 ms: 1.02x faster                                       |
| logging_silent           | 71.8 ns                                                     | 70.0 ns: 1.02x faster                                       |
| tornado_http             | 92.8 ms                                                     | 90.6 ms: 1.02x faster                                       |
| docutils                 | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                      |
| go                       | 101 ms                                                      | 98.8 ms: 1.02x faster                                       |
| sqlalchemy_declarative   | 85.6 ms                                                     | 83.8 ms: 1.02x faster                                       |
| sympy_integrate          | 14.0 ms                                                     | 13.7 ms: 1.02x faster                                       |
| deepcopy                 | 246 us                                                      | 241 us: 1.02x faster                                        |
| scimark_sor              | 78.1 ms                                                     | 76.5 ms: 1.02x faster                                       |
| mako                     | 7.58 ms                                                     | 7.44 ms: 1.02x faster                                       |
| python_startup_no_site   | 16.8 ms                                                     | 16.5 ms: 1.02x faster                                       |
| richards_super           | 38.7 ms                                                     | 38.0 ms: 1.02x faster                                       |
| python_startup           | 19.8 ms                                                     | 19.4 ms: 1.02x faster                                       |
| crypto_pyaes             | 48.9 ms                                                     | 48.1 ms: 1.02x faster                                       |
| pathlib                  | 70.9 ms                                                     | 69.7 ms: 1.02x faster                                       |
| pidigits                 | 150 ms                                                      | 148 ms: 1.02x faster                                        |
| logging_format           | 7.16 us                                                     | 7.06 us: 1.01x faster                                       |
| xml_etree_generate       | 52.5 ms                                                     | 51.8 ms: 1.01x faster                                       |
| spectral_norm            | 68.3 ms                                                     | 67.5 ms: 1.01x faster                                       |
| thrift                   | 494 us                                                      | 488 us: 1.01x faster                                        |
| gc_traversal             | 1.49 ms                                                     | 1.48 ms: 1.01x faster                                       |
| regex_effbot             | 1.50 ms                                                     | 1.49 ms: 1.01x faster                                       |
| sympy_str                | 185 ms                                                      | 183 ms: 1.01x faster                                        |
| float                    | 54.4 ms                                                     | 53.9 ms: 1.01x faster                                       |
| xml_etree_process        | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                       |
| sqlalchemy_imperative    | 10.4 ms                                                     | 10.4 ms: 1.00x faster                                       |
| flaskblogging            | 2.03 sec                                                    | 2.03 sec: 1.00x slower                                      |
| typing_runtime_protocols | 326 us                                                      | 327 us: 1.00x slower                                        |
| unpickle_list            | 2.59 us                                                     | 2.60 us: 1.00x slower                                       |
| regex_dna                | 116 ms                                                      | 117 ms: 1.01x slower                                        |
| scimark_fft              | 179 ms                                                      | 181 ms: 1.01x slower                                        |
| async_generators         | 177 ms                                                      | 180 ms: 1.02x slower                                        |
| comprehensions           | 15.6 us                                                     | 15.9 us: 1.02x slower                                       |
| meteor_contest           | 75.2 ms                                                     | 76.8 ms: 1.02x slower                                       |
| mdp                      | 1.59 sec                                                    | 1.63 sec: 1.02x slower                                      |
| pickle_list              | 2.70 us                                                     | 2.75 us: 1.02x slower                                       |
| chaos                    | 48.4 ms                                                     | 49.5 ms: 1.02x slower                                       |
| scimark_monte_carlo      | 45.3 ms                                                     | 46.5 ms: 1.03x slower                                       |
| pickle                   | 6.64 us                                                     | 6.86 us: 1.03x slower                                       |
| unpickle                 | 7.57 us                                                     | 7.92 us: 1.05x slower                                       |
| fannkuch                 | 253 ms                                                      | 268 ms: 1.06x slower                                        |
| coverage                 | 43.4 ms                                                     | 54.3 ms: 1.25x slower                                       |
| Geometric mean           | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (22): asyncio_tcp, pylint, bench_thread_pool, xml_etree_parse, create_gc_cycles, generators, nbody, scimark_lu, json_loads, html5lib, scimark_sparse_mat_mult, sqlglot_optimize, deepcopy_reduce, sympy_expand, sqlglot_normalize, hexiom, chameleon, pickle_dict, sympy_sum, regex_compile, asyncio_tcp_ssl, json
Ignored benchmarks (5) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown