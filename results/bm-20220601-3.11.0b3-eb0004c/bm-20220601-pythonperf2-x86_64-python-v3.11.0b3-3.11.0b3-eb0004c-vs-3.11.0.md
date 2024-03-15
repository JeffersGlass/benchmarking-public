
# Results vs. 3.11.0

- fork: python
- ref: v3.11.0b3
- machine: linux-x86_64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.00x slower \*
- HPT reliability: 87.52%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 284 ms: 1.01x faster                                             |
| chameleon      | 7.92 ms                                                      | 7.60 ms: 1.04x faster                                            |
| docutils       | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                           |
| html5lib       | 72.2 ms                                                      | 71.0 ms: 1.02x faster                                            |
| tornado_http   | 124 ms                                                       | 119 ms: 1.05x faster                                             |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 617 ms: 1.02x faster                                             |
| async_tree_none         | 518 ms                                                       | 513 ms: 1.01x faster                                             |
| async_tree_cpu_io_mixed | 753 ms                                                       | 810 ms: 1.08x slower                                             |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 73.9 ms: 1.01x faster                                            |
| pidigits       | 251 ms                                                       | 252 ms: 1.00x slower                                             |
| Geometric mean | (ref)                                                        | 1.00x faster                                                     |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.05 ms: 1.10x faster                                            |
| regex_dna      | 227 ms                                                       | 219 ms: 1.04x faster                                             |
| regex_v8       | 24.4 ms                                                      | 24.3 ms: 1.00x faster                                            |
| Geometric mean | (ref)                                                        | 1.03x faster                                                     |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|---------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_loads          | 28.9 us                                                      | 25.2 us: 1.15x faster                                            |
| xml_etree_iterparse | 107 ms                                                       | 103 ms: 1.04x faster                                             |
| pickle_dict         | 32.3 us                                                      | 31.3 us: 1.03x faster                                            |
| pickle              | 9.89 us                                                      | 9.80 us: 1.01x faster                                            |
| pickle_list         | 3.94 us                                                      | 3.92 us: 1.00x faster                                            |
| xml_etree_generate  | 79.7 ms                                                      | 80.2 ms: 1.01x slower                                            |
| pickle_pure_python  | 316 us                                                       | 319 us: 1.01x slower                                             |
| json_dumps          | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                            |
| Geometric mean      | (ref)                                                        | 1.02x faster                                                     |

Benchmark hidden because not significant (5): xml_etree_parse, unpickle, unpickle_list, unpickle_pure_python, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                            |
| python_startup_no_site | 7.73 ms                                                      | 7.70 ms: 1.00x faster                                            |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| genshi_text     | 25.5 ms                                                      | 26.3 ms: 1.03x slower                                            |
| django_template | 39.3 ms                                                      | 41.4 ms: 1.05x slower                                            |
| genshi_xml      | 57.1 ms                                                      | 60.1 ms: 1.05x slower                                            |
| Geometric mean  | (ref)                                                        | 1.03x slower                                                     |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_loads              | 28.9 us                                                      | 25.2 us: 1.15x faster                                            |
| regex_effbot            | 3.34 ms                                                      | 3.05 ms: 1.10x faster                                            |
| json                    | 5.58 ms                                                      | 5.20 ms: 1.07x faster                                            |
| nqueens                 | 103 ms                                                       | 97.6 ms: 1.05x faster                                            |
| tornado_http            | 124 ms                                                       | 119 ms: 1.05x faster                                             |
| sympy_sum               | 186 ms                                                       | 177 ms: 1.05x faster                                             |
| chameleon               | 7.92 ms                                                      | 7.60 ms: 1.04x faster                                            |
| sympy_expand            | 553 ms                                                       | 531 ms: 1.04x faster                                             |
| pprint_safe_repr        | 805 ms                                                       | 774 ms: 1.04x faster                                             |
| bench_mp_pool           | 4.70 ms                                                      | 4.52 ms: 1.04x faster                                            |
| regex_dna               | 227 ms                                                       | 219 ms: 1.04x faster                                             |
| gunicorn                | 966 us                                                       | 931 us: 1.04x faster                                             |
| xml_etree_iterparse     | 107 ms                                                       | 103 ms: 1.04x faster                                             |
| scimark_lu              | 114 ms                                                       | 110 ms: 1.04x faster                                             |
| pickle_dict             | 32.3 us                                                      | 31.3 us: 1.03x faster                                            |
| pprint_pformat          | 1.67 sec                                                     | 1.61 sec: 1.03x faster                                           |
| sympy_str               | 337 ms                                                       | 327 ms: 1.03x faster                                             |
| gc_traversal            | 4.15 ms                                                      | 4.03 ms: 1.03x faster                                            |
| aiohttp                 | 986 us                                                       | 958 us: 1.03x faster                                             |
| thrift                  | 931 us                                                       | 909 us: 1.02x faster                                             |
| sympy_integrate         | 25.8 ms                                                      | 25.2 ms: 1.02x faster                                            |
| pyflate                 | 449 ms                                                       | 441 ms: 1.02x faster                                             |
| async_tree_memoization  | 629 ms                                                       | 617 ms: 1.02x faster                                             |
| chaos                   | 74.9 ms                                                      | 73.6 ms: 1.02x faster                                            |
| raytrace                | 309 ms                                                       | 304 ms: 1.02x faster                                             |
| html5lib                | 72.2 ms                                                      | 71.0 ms: 1.02x faster                                            |
| flaskblogging           | 3.88 ms                                                      | 3.82 ms: 1.02x faster                                            |
| float                   | 74.9 ms                                                      | 73.9 ms: 1.01x faster                                            |
| async_generators        | 322 ms                                                       | 318 ms: 1.01x faster                                             |
| logging_simple          | 7.24 us                                                      | 7.16 us: 1.01x faster                                            |
| sqlalchemy_imperative   | 19.8 ms                                                      | 19.6 ms: 1.01x faster                                            |
| logging_silent          | 100 ns                                                       | 99.3 ns: 1.01x faster                                            |
| 2to3                    | 287 ms                                                       | 284 ms: 1.01x faster                                             |
| pickle                  | 9.89 us                                                      | 9.80 us: 1.01x faster                                            |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.03 ms: 1.01x faster                                            |
| telco                   | 6.81 ms                                                      | 6.75 ms: 1.01x faster                                            |
| async_tree_none         | 518 ms                                                       | 513 ms: 1.01x faster                                             |
| python_startup          | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                            |
| docutils                | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                           |
| regex_v8                | 24.4 ms                                                      | 24.3 ms: 1.00x faster                                            |
| python_startup_no_site  | 7.73 ms                                                      | 7.70 ms: 1.00x faster                                            |
| pickle_list             | 3.94 us                                                      | 3.92 us: 1.00x faster                                            |
| pidigits                | 251 ms                                                       | 252 ms: 1.00x slower                                             |
| meteor_contest          | 131 ms                                                       | 131 ms: 1.00x slower                                             |
| asyncio_tcp             | 747 ms                                                       | 751 ms: 1.01x slower                                             |
| xml_etree_generate      | 79.7 ms                                                      | 80.2 ms: 1.01x slower                                            |
| sqlglot_optimize        | 59.0 ms                                                      | 59.4 ms: 1.01x slower                                            |
| pickle_pure_python      | 316 us                                                       | 319 us: 1.01x slower                                             |
| dask                    | 410 ms                                                       | 414 ms: 1.01x slower                                             |
| pathlib                 | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                            |
| sqlglot_normalize       | 122 ms                                                       | 123 ms: 1.01x slower                                             |
| crypto_pyaes            | 83.3 ms                                                      | 84.5 ms: 1.01x slower                                            |
| dulwich_log             | 67.4 ms                                                      | 68.4 ms: 1.02x slower                                            |
| mdp                     | 2.77 sec                                                     | 2.81 sec: 1.02x slower                                           |
| json_dumps              | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                            |
| spectral_norm           | 95.1 ms                                                      | 96.8 ms: 1.02x slower                                            |
| scimark_fft             | 281 ms                                                       | 286 ms: 1.02x slower                                             |
| scimark_sor             | 110 ms                                                       | 112 ms: 1.02x slower                                             |
| deepcopy_reduce         | 3.40 us                                                      | 3.48 us: 1.02x slower                                            |
| generators              | 54.6 ms                                                      | 56.0 ms: 1.02x slower                                            |
| logging_format          | 7.71 us                                                      | 7.95 us: 1.03x slower                                            |
| genshi_text             | 25.5 ms                                                      | 26.3 ms: 1.03x slower                                            |
| go                      | 158 ms                                                       | 166 ms: 1.05x slower                                             |
| django_template         | 39.3 ms                                                      | 41.4 ms: 1.05x slower                                            |
| genshi_xml              | 57.1 ms                                                      | 60.1 ms: 1.05x slower                                            |
| deltablue               | 3.97 ms                                                      | 4.20 ms: 1.06x slower                                            |
| create_gc_cycles        | 1.58 ms                                                      | 1.68 ms: 1.07x slower                                            |
| async_tree_cpu_io_mixed | 753 ms                                                       | 810 ms: 1.08x slower                                             |
| comprehensions          | 25.1 us                                                      | 28.3 us: 1.13x slower                                            |
| fannkuch                | 416 ms                                                       | 496 ms: 1.19x slower                                             |
| sqlglot_transpile       | 1.91 ms                                                      | 2.32 ms: 1.21x slower                                            |
| sqlglot_parse           | 1.51 ms                                                      | 1.97 ms: 1.30x slower                                            |
| Geometric mean          | (ref)                                                        | 1.00x slower                                                     |

Benchmark hidden because not significant (21): richards, xml_etree_parse, mako, unpack_sequence, scimark_monte_carlo, sqlite_synth, unpickle, async_tree_io, unpickle_list, sqlalchemy_declarative, deepcopy, regex_compile, pycparser, unpickle_pure_python, nbody, xml_etree_process, pylint, hexiom, coroutines, deepcopy_memo, bench_thread_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 87.52% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x