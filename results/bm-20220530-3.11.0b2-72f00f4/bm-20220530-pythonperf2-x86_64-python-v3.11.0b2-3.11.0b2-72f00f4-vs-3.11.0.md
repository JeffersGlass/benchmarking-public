
# Results vs. 3.11.0

- fork: python
- ref: v3.11.0b2
- machine: linux-x86_64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.01x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 282 ms: 1.02x faster                                             |
| chameleon      | 7.92 ms                                                      | 7.52 ms: 1.05x faster                                            |
| docutils       | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                           |
| html5lib       | 72.2 ms                                                      | 70.5 ms: 1.02x faster                                            |
| tornado_http   | 124 ms                                                       | 117 ms: 1.06x faster                                             |
| Geometric mean | (ref)                                                        | 1.03x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 609 ms: 1.03x faster                                             |
| async_tree_cpu_io_mixed | 753 ms                                                       | 740 ms: 1.02x faster                                             |
| async_tree_none         | 518 ms                                                       | 511 ms: 1.01x faster                                             |
| Geometric mean          | (ref)                                                        | 1.02x faster                                                     |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 73.8 ms: 1.02x faster                                            |
| nbody          | 92.9 ms                                                      | 96.9 ms: 1.04x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.11 ms: 1.07x faster                                            |
| regex_v8       | 24.4 ms                                                      | 24.1 ms: 1.01x faster                                            |
| regex_dna      | 227 ms                                                       | 227 ms: 1.00x faster                                             |
| regex_compile  | 156 ms                                                       | 157 ms: 1.00x slower                                             |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 25.1 us: 1.15x faster                                            |
| pickle_dict          | 32.3 us                                                      | 30.4 us: 1.06x faster                                            |
| pickle_list          | 3.94 us                                                      | 3.86 us: 1.02x faster                                            |
| unpickle_pure_python | 238 us                                                       | 234 us: 1.02x faster                                             |
| pickle               | 9.89 us                                                      | 9.77 us: 1.01x faster                                            |
| xml_etree_parse      | 155 ms                                                       | 153 ms: 1.01x faster                                             |
| xml_etree_generate   | 79.7 ms                                                      | 79.0 ms: 1.01x faster                                            |
| pickle_pure_python   | 316 us                                                       | 320 us: 1.01x slower                                             |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                     |

Benchmark hidden because not significant (5): xml_etree_iterparse, unpickle_list, xml_etree_process, unpickle, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                            |
| python_startup_no_site | 7.73 ms                                                      | 7.70 ms: 1.00x faster                                            |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| genshi_text    | 25.5 ms                                                      | 24.4 ms: 1.04x faster                                            |
| genshi_xml     | 57.1 ms                                                      | 56.0 ms: 1.02x faster                                            |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmark hidden because not significant (2): mako, django_template

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_loads              | 28.9 us                                                      | 25.1 us: 1.15x faster                                            |
| json                    | 5.58 ms                                                      | 5.16 ms: 1.08x faster                                            |
| regex_effbot            | 3.34 ms                                                      | 3.11 ms: 1.07x faster                                            |
| pickle_dict             | 32.3 us                                                      | 30.4 us: 1.06x faster                                            |
| pprint_pformat          | 1.67 sec                                                     | 1.57 sec: 1.06x faster                                           |
| tornado_http            | 124 ms                                                       | 117 ms: 1.06x faster                                             |
| pprint_safe_repr        | 805 ms                                                       | 759 ms: 1.06x faster                                             |
| chameleon               | 7.92 ms                                                      | 7.52 ms: 1.05x faster                                            |
| gc_traversal            | 4.15 ms                                                      | 3.94 ms: 1.05x faster                                            |
| nqueens                 | 103 ms                                                       | 97.7 ms: 1.05x faster                                            |
| sympy_sum               | 186 ms                                                       | 177 ms: 1.05x faster                                             |
| genshi_text             | 25.5 ms                                                      | 24.4 ms: 1.04x faster                                            |
| aiohttp                 | 986 us                                                       | 944 us: 1.04x faster                                             |
| pyflate                 | 449 ms                                                       | 431 ms: 1.04x faster                                             |
| gunicorn                | 966 us                                                       | 929 us: 1.04x faster                                             |
| chaos                   | 74.9 ms                                                      | 72.1 ms: 1.04x faster                                            |
| sympy_expand            | 553 ms                                                       | 533 ms: 1.04x faster                                             |
| scimark_monte_carlo     | 69.8 ms                                                      | 67.5 ms: 1.03x faster                                            |
| async_tree_memoization  | 629 ms                                                       | 609 ms: 1.03x faster                                             |
| bench_mp_pool           | 4.70 ms                                                      | 4.55 ms: 1.03x faster                                            |
| sympy_str               | 337 ms                                                       | 327 ms: 1.03x faster                                             |
| sympy_integrate         | 25.8 ms                                                      | 25.0 ms: 1.03x faster                                            |
| async_generators        | 322 ms                                                       | 313 ms: 1.03x faster                                             |
| scimark_lu              | 114 ms                                                       | 111 ms: 1.03x faster                                             |
| html5lib                | 72.2 ms                                                      | 70.5 ms: 1.02x faster                                            |
| richards                | 49.7 ms                                                      | 48.5 ms: 1.02x faster                                            |
| go                      | 158 ms                                                       | 154 ms: 1.02x faster                                             |
| pickle_list             | 3.94 us                                                      | 3.86 us: 1.02x faster                                            |
| genshi_xml              | 57.1 ms                                                      | 56.0 ms: 1.02x faster                                            |
| scimark_sor             | 110 ms                                                       | 108 ms: 1.02x faster                                             |
| sqlalchemy_imperative   | 19.8 ms                                                      | 19.4 ms: 1.02x faster                                            |
| unpickle_pure_python    | 238 us                                                       | 234 us: 1.02x faster                                             |
| spectral_norm           | 95.1 ms                                                      | 93.4 ms: 1.02x faster                                            |
| async_tree_cpu_io_mixed | 753 ms                                                       | 740 ms: 1.02x faster                                             |
| deepcopy_memo           | 37.5 us                                                      | 36.9 us: 1.02x faster                                            |
| 2to3                    | 287 ms                                                       | 282 ms: 1.02x faster                                             |
| float                   | 74.9 ms                                                      | 73.8 ms: 1.02x faster                                            |
| raytrace                | 309 ms                                                       | 305 ms: 1.01x faster                                             |
| deepcopy                | 391 us                                                       | 385 us: 1.01x faster                                             |
| logging_silent          | 100 ns                                                       | 98.9 ns: 1.01x faster                                            |
| async_tree_none         | 518 ms                                                       | 511 ms: 1.01x faster                                             |
| pickle                  | 9.89 us                                                      | 9.77 us: 1.01x faster                                            |
| unpack_sequence         | 45.7 ns                                                      | 45.1 ns: 1.01x faster                                            |
| regex_v8                | 24.4 ms                                                      | 24.1 ms: 1.01x faster                                            |
| meteor_contest          | 131 ms                                                       | 129 ms: 1.01x faster                                             |
| sqlalchemy_declarative  | 154 ms                                                       | 153 ms: 1.01x faster                                             |
| xml_etree_parse         | 155 ms                                                       | 153 ms: 1.01x faster                                             |
| xml_etree_generate      | 79.7 ms                                                      | 79.0 ms: 1.01x faster                                            |
| python_startup          | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                            |
| docutils                | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                           |
| python_startup_no_site  | 7.73 ms                                                      | 7.70 ms: 1.00x faster                                            |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.05 ms: 1.00x faster                                            |
| regex_dna               | 227 ms                                                       | 227 ms: 1.00x faster                                             |
| regex_compile           | 156 ms                                                       | 157 ms: 1.00x slower                                             |
| pathlib                 | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                            |
| generators              | 54.6 ms                                                      | 55.2 ms: 1.01x slower                                            |
| scimark_fft             | 281 ms                                                       | 284 ms: 1.01x slower                                             |
| sqlglot_optimize        | 59.0 ms                                                      | 59.7 ms: 1.01x slower                                            |
| logging_format          | 7.71 us                                                      | 7.81 us: 1.01x slower                                            |
| pickle_pure_python      | 316 us                                                       | 320 us: 1.01x slower                                             |
| sqlglot_normalize       | 122 ms                                                       | 124 ms: 1.02x slower                                             |
| deepcopy_reduce         | 3.40 us                                                      | 3.47 us: 1.02x slower                                            |
| telco                   | 6.81 ms                                                      | 6.99 ms: 1.03x slower                                            |
| mdp                     | 2.77 sec                                                     | 2.85 sec: 1.03x slower                                           |
| create_gc_cycles        | 1.58 ms                                                      | 1.64 ms: 1.04x slower                                            |
| nbody                   | 92.9 ms                                                      | 96.9 ms: 1.04x slower                                            |
| fannkuch                | 416 ms                                                       | 447 ms: 1.08x slower                                             |
| comprehensions          | 25.1 us                                                      | 27.9 us: 1.11x slower                                            |
| sqlglot_transpile       | 1.91 ms                                                      | 2.29 ms: 1.20x slower                                            |
| sqlglot_parse           | 1.51 ms                                                      | 1.95 ms: 1.29x slower                                            |
| Geometric mean          | (ref)                                                        | 1.01x faster                                                     |

Benchmark hidden because not significant (22): xml_etree_iterparse, pylint, pycparser, mako, unpickle_list, async_tree_io, logging_simple, dulwich_log, asyncio_tcp, xml_etree_process, unpickle, dask, pidigits, hexiom, bench_thread_pool, deltablue, crypto_pyaes, thrift, json_dumps, django_template, coroutines, sqlite_synth
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x