
# Results vs. 3.11.0

- fork: python
- ref: 1aec0644447e69e981d5
- machine: windows-amd64
- commit hash: 1aec064
- commit date: 2024-02-01
- overall geometric mean: 1.08x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 219 ms: 1.03x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.89 ms: 1.08x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.62 sec: 1.01x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 86.9 ms: 1.07x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 347 ms: 1.17x faster                                                        |
| async_tree_io              | 808 ms                                                      | 721 ms: 1.12x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 277 ms: 1.11x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 470 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 755 ms: 1.10x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 61.0 ms: 1.15x faster                                                       |
| float          | 54.4 ms                                                     | 50.4 ms: 1.08x faster                                                       |
| pidigits       | 150 ms                                                      | 153 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 81.0 ms: 1.12x faster                                                       |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 21.8 ms: 1.54x slower                                                       |
| Geometric mean | (ref)                                                       | 1.11x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.48 ms: 1.48x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 127 us: 1.23x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 179 us: 1.17x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.8 ms: 1.03x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.1 us: 1.02x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.8 ms: 1.02x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.82 us: 1.05x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.73 us: 1.06x slower                                                       |
| pickle               | 6.64 us                                                     | 7.48 us: 1.13x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.81 us: 1.16x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.9 ms: 1.06x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.9 ms: 1.13x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.79 ms: 1.12x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.9 us: 4.59x faster                                                       |
| generators                 | 34.0 ms                                                     | 19.9 ms: 1.71x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.48 ms: 1.48x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 499 ms: 1.46x faster                                                        |
| comprehensions             | 15.6 us                                                     | 11.5 us: 1.36x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 53.9 ns: 1.33x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.06 ms: 1.31x faster                                                       |
| richards_super             | 38.7 ms                                                     | 29.6 ms: 1.31x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 764 us: 1.25x faster                                                        |
| raytrace                   | 213 ms                                                      | 171 ms: 1.25x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 127 us: 1.23x faster                                                        |
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                        |
| richards                   | 31.4 ms                                                     | 25.9 ms: 1.21x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 38.7 ns: 1.21x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 977 us: 1.19x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 57.5 ms: 1.19x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 179 us: 1.17x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 347 ms: 1.17x faster                                                        |
| nbody                      | 70.3 ms                                                     | 61.0 ms: 1.15x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 22.6 us: 1.15x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                       |
| logging_simple             | 6.86 us                                                     | 5.98 us: 1.15x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.54 us: 1.14x faster                                                       |
| chaos                      | 48.4 ms                                                     | 42.6 ms: 1.14x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 81.0 ms: 1.12x faster                                                       |
| async_tree_io              | 808 ms                                                      | 721 ms: 1.12x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                                      |
| mako                       | 7.58 ms                                                     | 6.79 ms: 1.12x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.43 us: 1.11x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 277 ms: 1.11x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 470 ms: 1.11x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.84 sec: 1.10x faster                                                      |
| sympy_sum                  | 100 ms                                                      | 91.0 ms: 1.10x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 57.2 ms: 1.10x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 755 ms: 1.10x faster                                                        |
| sympy_str                  | 185 ms                                                      | 169 ms: 1.09x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 42.6 ms: 1.09x faster                                                       |
| deepcopy                   | 246 us                                                      | 226 us: 1.09x faster                                                        |
| float                      | 54.4 ms                                                     | 50.4 ms: 1.08x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 45.3 ms: 1.08x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.89 ms: 1.08x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 86.9 ms: 1.07x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 501 ms: 1.06x faster                                                        |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.96 us: 1.05x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.4 ms: 1.05x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.04 sec: 1.05x faster                                                      |
| mypy2                      | 459 ms                                                      | 439 ms: 1.05x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 183 ms: 1.04x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 65.8 ms: 1.04x faster                                                       |
| fannkuch                   | 253 ms                                                      | 244 ms: 1.04x faster                                                        |
| pycparser                  | 720 ms                                                      | 695 ms: 1.04x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.8 ms: 1.03x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.1 us: 1.02x faster                                                       |
| dask                       | 273 ms                                                      | 268 ms: 1.02x faster                                                        |
| go                         | 101 ms                                                      | 99.3 ms: 1.02x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.62 sec: 1.01x faster                                                      |
| xml_etree_process          | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                                       |
| pyflate                    | 312 ms                                                      | 315 ms: 1.01x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 76.2 ms: 1.01x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.2 ms: 1.02x slower                                                       |
| pidigits                   | 150 ms                                                      | 153 ms: 1.02x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 53.8 ms: 1.02x slower                                                       |
| 2to3                       | 214 ms                                                      | 219 ms: 1.03x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 742 us: 1.04x slower                                                        |
| pickle_list                | 2.70 us                                                     | 2.82 us: 1.05x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| mdp                        | 1.59 sec                                                    | 1.68 sec: 1.05x slower                                                      |
| python_startup             | 19.8 ms                                                     | 20.9 ms: 1.06x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.73 us: 1.06x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.73 ms: 1.06x slower                                                       |
| scimark_fft                | 179 ms                                                      | 195 ms: 1.09x slower                                                        |
| coverage                   | 43.4 ms                                                     | 47.6 ms: 1.10x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.46 ms: 1.10x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 70.2 ms: 1.11x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.9 ms: 1.13x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.48 us: 1.13x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 81.5 ms: 1.15x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.27 ms: 1.16x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.81 us: 1.16x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 57.0 ms: 1.26x slower                                                       |
| async_generators           | 177 ms                                                      | 241 ms: 1.36x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 21.8 ms: 1.54x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                                |

Benchmark hidden because not significant (3): json, scimark_sor, bench_thread_pool
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown