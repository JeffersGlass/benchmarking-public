
# Results vs. 3.11.0

- fork: python
- ref: v3.11.8
- machine: windows-amd64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.02x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 206 ms: 1.03x faster                                        |
| chameleon      | 5.26 ms                                                     | 5.18 ms: 1.02x faster                                       |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                      |
| tornado_http   | 92.8 ms                                                     | 88.0 ms: 1.05x faster                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization_tg  | 405 ms                                                      | 372 ms: 1.09x faster                                        |
| async_tree_none            | 332 ms                                                      | 312 ms: 1.06x faster                                        |
| async_tree_none_tg         | 309 ms                                                      | 292 ms: 1.06x faster                                        |
| async_tree_memoization     | 399 ms                                                      | 379 ms: 1.05x faster                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 500 ms: 1.05x faster                                        |
| async_tree_io_tg           | 829 ms                                                      | 794 ms: 1.04x faster                                        |
| async_tree_io              | 808 ms                                                      | 785 ms: 1.03x faster                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.01x faster                                        |
| float          | 54.4 ms                                                     | 53.6 ms: 1.01x faster                                       |
| nbody          | 70.3 ms                                                     | 71.7 ms: 1.02x slower                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.6 ms: 1.05x faster                                       |
| regex_compile  | 91.0 ms                                                     | 88.2 ms: 1.03x faster                                       |
| regex_effbot   | 1.50 ms                                                     | 1.49 ms: 1.00x faster                                       |
| regex_dna      | 116 ms                                                      | 117 ms: 1.01x slower                                        |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| unpickle_pure_python | 157 us                                                      | 150 us: 1.05x faster                                        |
| pickle_pure_python   | 208 us                                                      | 201 us: 1.04x faster                                        |
| json_dumps           | 8.09 ms                                                     | 7.80 ms: 1.04x faster                                       |
| tomli_loads          | 1.46 sec                                                    | 1.42 sec: 1.03x faster                                      |
| xml_etree_process    | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                       |
| json_loads           | 13.0 us                                                     | 12.9 us: 1.01x faster                                       |
| unpickle_list        | 2.59 us                                                     | 2.61 us: 1.01x slower                                       |
| pickle               | 6.64 us                                                     | 6.78 us: 1.02x slower                                       |
| unpickle             | 7.57 us                                                     | 7.78 us: 1.03x slower                                       |
| xml_etree_parse      | 97.6 ms                                                     | 102 ms: 1.04x slower                                        |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                |

Benchmark hidden because not significant (4): pickle_dict, xml_etree_iterparse, xml_etree_generate, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.3 ms: 1.10x faster                                       |
| python_startup         | 19.8 ms                                                     | 18.4 ms: 1.07x faster                                       |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.1 ms: 1.08x faster                                       |
| genshi_xml      | 39.9 ms                                                     | 38.3 ms: 1.04x faster                                       |
| django_template | 24.4 ms                                                     | 23.9 ms: 1.02x faster                                       |
| mako            | 7.58 ms                                                     | 7.47 ms: 1.02x faster                                       |
| Geometric mean  | (ref)                                                       | 1.04x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site     | 16.8 ms                                                     | 15.3 ms: 1.10x faster                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 372 ms: 1.09x faster                                        |
| genshi_text                | 18.4 ms                                                     | 17.1 ms: 1.08x faster                                       |
| python_startup             | 19.8 ms                                                     | 18.4 ms: 1.07x faster                                       |
| async_tree_none            | 332 ms                                                      | 312 ms: 1.06x faster                                        |
| pathlib                    | 70.9 ms                                                     | 66.9 ms: 1.06x faster                                       |
| raytrace                   | 213 ms                                                      | 202 ms: 1.06x faster                                        |
| nqueens                    | 68.3 ms                                                     | 64.7 ms: 1.06x faster                                       |
| async_tree_none_tg         | 309 ms                                                      | 292 ms: 1.06x faster                                        |
| tornado_http               | 92.8 ms                                                     | 88.0 ms: 1.05x faster                                       |
| deepcopy_memo              | 26.0 us                                                     | 24.6 us: 1.05x faster                                       |
| dulwich_log                | 46.4 ms                                                     | 44.0 ms: 1.05x faster                                       |
| async_tree_memoization     | 399 ms                                                      | 379 ms: 1.05x faster                                        |
| pycparser                  | 720 ms                                                      | 684 ms: 1.05x faster                                        |
| fannkuch                   | 253 ms                                                      | 241 ms: 1.05x faster                                        |
| pylint                     | 323 ms                                                      | 308 ms: 1.05x faster                                        |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                      |
| unpickle_pure_python       | 157 us                                                      | 150 us: 1.05x faster                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 500 ms: 1.05x faster                                        |
| regex_v8                   | 14.2 ms                                                     | 13.6 ms: 1.05x faster                                       |
| async_tree_io_tg           | 829 ms                                                      | 794 ms: 1.04x faster                                        |
| aiohttp                    | 883 us                                                      | 846 us: 1.04x faster                                        |
| genshi_xml                 | 39.9 ms                                                     | 38.3 ms: 1.04x faster                                       |
| pickle_pure_python         | 208 us                                                      | 201 us: 1.04x faster                                        |
| dask                       | 273 ms                                                      | 263 ms: 1.04x faster                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.5 ms: 1.04x faster                                       |
| richards                   | 31.4 ms                                                     | 30.3 ms: 1.04x faster                                       |
| json_dumps                 | 8.09 ms                                                     | 7.80 ms: 1.04x faster                                       |
| telco                      | 4.06 ms                                                     | 3.93 ms: 1.04x faster                                       |
| 2to3                       | 214 ms                                                      | 206 ms: 1.03x faster                                        |
| regex_compile              | 91.0 ms                                                     | 88.2 ms: 1.03x faster                                       |
| sqlite_synth               | 1.77 us                                                     | 1.71 us: 1.03x faster                                       |
| scimark_lu                 | 62.8 ms                                                     | 61.0 ms: 1.03x faster                                       |
| bench_mp_pool              | 63.2 ms                                                     | 61.4 ms: 1.03x faster                                       |
| deltablue                  | 2.70 ms                                                     | 2.62 ms: 1.03x faster                                       |
| async_tree_io              | 808 ms                                                      | 785 ms: 1.03x faster                                        |
| richards_super             | 38.7 ms                                                     | 37.6 ms: 1.03x faster                                       |
| comprehensions             | 15.6 us                                                     | 15.2 us: 1.03x faster                                       |
| logging_silent             | 71.8 ns                                                     | 69.9 ns: 1.03x faster                                       |
| bench_thread_pool          | 872 us                                                      | 849 us: 1.03x faster                                        |
| tomli_loads                | 1.46 sec                                                    | 1.42 sec: 1.03x faster                                      |
| sqlalchemy_declarative     | 85.6 ms                                                     | 83.4 ms: 1.03x faster                                       |
| sqlglot_parse              | 953 us                                                      | 929 us: 1.03x faster                                        |
| pyflate                    | 312 ms                                                      | 305 ms: 1.02x faster                                        |
| crypto_pyaes               | 48.9 ms                                                     | 47.7 ms: 1.02x faster                                       |
| sqlalchemy_imperative      | 10.4 ms                                                     | 10.2 ms: 1.02x faster                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.14 ms: 1.02x faster                                       |
| django_template            | 24.4 ms                                                     | 23.9 ms: 1.02x faster                                       |
| scimark_sor                | 78.1 ms                                                     | 76.6 ms: 1.02x faster                                       |
| deepcopy                   | 246 us                                                      | 242 us: 1.02x faster                                        |
| thrift                     | 494 us                                                      | 485 us: 1.02x faster                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.07 sec: 1.02x faster                                      |
| logging_simple             | 6.86 us                                                     | 6.75 us: 1.02x faster                                       |
| sympy_sum                  | 100 ms                                                      | 98.5 ms: 1.02x faster                                       |
| mypy2                      | 459 ms                                                      | 452 ms: 1.02x faster                                        |
| mako                       | 7.58 ms                                                     | 7.47 ms: 1.02x faster                                       |
| generators                 | 34.0 ms                                                     | 33.5 ms: 1.02x faster                                       |
| chameleon                  | 5.26 ms                                                     | 5.18 ms: 1.02x faster                                       |
| spectral_norm              | 68.3 ms                                                     | 67.3 ms: 1.01x faster                                       |
| pidigits                   | 150 ms                                                      | 148 ms: 1.01x faster                                        |
| float                      | 54.4 ms                                                     | 53.6 ms: 1.01x faster                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                       |
| pprint_safe_repr           | 529 ms                                                      | 522 ms: 1.01x faster                                        |
| sympy_str                  | 185 ms                                                      | 183 ms: 1.01x faster                                        |
| hexiom                     | 4.55 ms                                                     | 4.51 ms: 1.01x faster                                       |
| coroutines                 | 15.0 ms                                                     | 14.8 ms: 1.01x faster                                       |
| json_loads                 | 13.0 us                                                     | 12.9 us: 1.01x faster                                       |
| meteor_contest             | 75.2 ms                                                     | 74.7 ms: 1.01x faster                                       |
| logging_format             | 7.16 us                                                     | 7.13 us: 1.01x faster                                       |
| gc_traversal               | 1.49 ms                                                     | 1.49 ms: 1.01x faster                                       |
| regex_effbot               | 1.50 ms                                                     | 1.49 ms: 1.00x faster                                       |
| flaskblogging              | 2.03 sec                                                    | 2.03 sec: 1.00x slower                                      |
| typing_runtime_protocols   | 326 us                                                      | 328 us: 1.01x slower                                        |
| unpickle_list              | 2.59 us                                                     | 2.61 us: 1.01x slower                                       |
| regex_dna                  | 116 ms                                                      | 117 ms: 1.01x slower                                        |
| unpack_sequence            | 46.9 ns                                                     | 47.3 ns: 1.01x slower                                       |
| sqlglot_normalize          | 190 ms                                                      | 192 ms: 1.01x slower                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                       |
| mdp                        | 1.59 sec                                                    | 1.61 sec: 1.01x slower                                      |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.61 ms: 1.01x slower                                       |
| scimark_fft                | 179 ms                                                      | 182 ms: 1.01x slower                                        |
| nbody                      | 70.3 ms                                                     | 71.7 ms: 1.02x slower                                       |
| pickle                     | 6.64 us                                                     | 6.78 us: 1.02x slower                                       |
| go                         | 101 ms                                                      | 103 ms: 1.02x slower                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 46.5 ms: 1.03x slower                                       |
| unpickle                   | 7.57 us                                                     | 7.78 us: 1.03x slower                                       |
| coverage                   | 43.4 ms                                                     | 44.8 ms: 1.03x slower                                       |
| deepcopy_reduce            | 2.06 us                                                     | 2.13 us: 1.03x slower                                       |
| xml_etree_parse            | 97.6 ms                                                     | 102 ms: 1.04x slower                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (13): asyncio_tcp_ssl, asyncio_tcp, async_tree_cpu_io_mixed, html5lib, create_gc_cycles, pickle_dict, xml_etree_iterparse, chaos, async_generators, sympy_expand, xml_etree_generate, pickle_list, json


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown