
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b3
- machine: linux-x86_64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.01x slower \*
- HPT reliability: 62.95%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 283 ms: 1.01x faster                                             |
| tornado_http   | 121 ms                                                       | 118 ms: 1.03x faster                                             |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 704 ms: 1.01x slower                                             |
| async_tree_memoization  | 544 ms                                                       | 551 ms: 1.01x slower                                             |
| async_tree_none         | 452 ms                                                       | 457 ms: 1.01x slower                                             |
| async_tree_io           | 1.04 sec                                                     | 1.06 sec: 1.01x slower                                           |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 84.2 ms: 1.05x faster                                            |
| pidigits       | 265 ms                                                       | 260 ms: 1.02x faster                                             |
| float          | 76.6 ms                                                      | 78.8 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.48 ms: 1.03x faster                                            |
| regex_v8       | 23.6 ms                                                      | 23.9 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                        | 1.00x faster                                                     |

Benchmark hidden because not significant (2): regex_dna, regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|---------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle              | 10.5 us                                                      | 10.3 us: 1.02x faster                                            |
| unpickle            | 14.8 us                                                      | 14.6 us: 1.01x faster                                            |
| xml_etree_generate  | 86.1 ms                                                      | 85.3 ms: 1.01x faster                                            |
| tomli_loads         | 2.16 sec                                                     | 2.17 sec: 1.00x slower                                           |
| json_loads          | 24.4 us                                                      | 24.7 us: 1.02x slower                                            |
| json_dumps          | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                            |
| pickle_pure_python  | 318 us                                                       | 326 us: 1.02x slower                                             |
| xml_etree_iterparse | 103 ms                                                       | 106 ms: 1.03x slower                                             |
| pickle_dict         | 32.5 us                                                      | 33.6 us: 1.03x slower                                            |
| xml_etree_parse     | 144 ms                                                       | 150 ms: 1.04x slower                                             |
| Geometric mean      | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (4): unpickle_pure_python, xml_etree_process, unpickle_list, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.43 ms: 1.02x faster                                            |
| python_startup         | 11.6 ms                                                      | 11.4 ms: 1.02x faster                                            |
| Geometric mean         | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpack_sequence         | 53.2 ns                                                      | 49.4 ns: 1.08x faster                                            |
| logging_format          | 7.48 us                                                      | 7.13 us: 1.05x faster                                            |
| nbody                   | 88.0 ms                                                      | 84.2 ms: 1.05x faster                                            |
| logging_simple          | 6.71 us                                                      | 6.49 us: 1.03x faster                                            |
| mdp                     | 2.57 sec                                                     | 2.49 sec: 1.03x faster                                           |
| go                      | 150 ms                                                       | 145 ms: 1.03x faster                                             |
| hexiom                  | 5.96 ms                                                      | 5.79 ms: 1.03x faster                                            |
| logging_silent          | 94.4 ns                                                      | 91.8 ns: 1.03x faster                                            |
| coroutines              | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                            |
| meteor_contest          | 128 ms                                                       | 125 ms: 1.03x faster                                             |
| regex_effbot            | 3.57 ms                                                      | 3.48 ms: 1.03x faster                                            |
| tornado_http            | 121 ms                                                       | 118 ms: 1.03x faster                                             |
| python_startup_no_site  | 8.64 ms                                                      | 8.43 ms: 1.02x faster                                            |
| richards                | 45.7 ms                                                      | 44.7 ms: 1.02x faster                                            |
| pickle                  | 10.5 us                                                      | 10.3 us: 1.02x faster                                            |
| async_generators        | 390 ms                                                       | 382 ms: 1.02x faster                                             |
| generators              | 37.4 ms                                                      | 36.7 ms: 1.02x faster                                            |
| scimark_lu              | 98.8 ms                                                      | 96.7 ms: 1.02x faster                                            |
| fannkuch                | 350 ms                                                       | 343 ms: 1.02x faster                                             |
| pidigits                | 265 ms                                                       | 260 ms: 1.02x faster                                             |
| python_startup          | 11.6 ms                                                      | 11.4 ms: 1.02x faster                                            |
| sqlite_synth            | 2.77 us                                                      | 2.72 us: 1.02x faster                                            |
| scimark_sor             | 109 ms                                                       | 107 ms: 1.02x faster                                             |
| scimark_monte_carlo     | 69.0 ms                                                      | 67.8 ms: 1.02x faster                                            |
| pprint_pformat          | 1.65 sec                                                     | 1.63 sec: 1.02x faster                                           |
| asyncio_tcp_ssl         | 1.59 sec                                                     | 1.56 sec: 1.02x faster                                           |
| unpickle                | 14.8 us                                                      | 14.6 us: 1.01x faster                                            |
| comprehensions          | 21.9 us                                                      | 21.7 us: 1.01x faster                                            |
| richards_super          | 51.3 ms                                                      | 50.8 ms: 1.01x faster                                            |
| pprint_safe_repr        | 807 ms                                                       | 799 ms: 1.01x faster                                             |
| xml_etree_generate      | 86.1 ms                                                      | 85.3 ms: 1.01x faster                                            |
| chaos                   | 64.0 ms                                                      | 63.4 ms: 1.01x faster                                            |
| 2to3                    | 285 ms                                                       | 283 ms: 1.01x faster                                             |
| deltablue               | 3.24 ms                                                      | 3.21 ms: 1.01x faster                                            |
| nqueens                 | 89.9 ms                                                      | 90.2 ms: 1.00x slower                                            |
| sqlglot_normalize       | 116 ms                                                       | 116 ms: 1.00x slower                                             |
| tomli_loads             | 2.16 sec                                                     | 2.17 sec: 1.00x slower                                           |
| raytrace                | 298 ms                                                       | 300 ms: 1.01x slower                                             |
| crypto_pyaes            | 80.3 ms                                                      | 80.9 ms: 1.01x slower                                            |
| scimark_fft             | 301 ms                                                       | 304 ms: 1.01x slower                                             |
| sqlglot_parse           | 1.38 ms                                                      | 1.39 ms: 1.01x slower                                            |
| dulwich_log             | 65.4 ms                                                      | 66.1 ms: 1.01x slower                                            |
| regex_v8                | 23.6 ms                                                      | 23.9 ms: 1.01x slower                                            |
| sqlglot_transpile       | 1.78 ms                                                      | 1.80 ms: 1.01x slower                                            |
| async_tree_cpu_io_mixed | 696 ms                                                       | 704 ms: 1.01x slower                                             |
| deepcopy_reduce         | 3.37 us                                                      | 3.41 us: 1.01x slower                                            |
| json                    | 5.12 ms                                                      | 5.18 ms: 1.01x slower                                            |
| async_tree_memoization  | 544 ms                                                       | 551 ms: 1.01x slower                                             |
| async_tree_none         | 452 ms                                                       | 457 ms: 1.01x slower                                             |
| async_tree_io           | 1.04 sec                                                     | 1.06 sec: 1.01x slower                                           |
| json_loads              | 24.4 us                                                      | 24.7 us: 1.02x slower                                            |
| telco                   | 6.96 ms                                                      | 7.07 ms: 1.02x slower                                            |
| deepcopy_memo           | 36.8 us                                                      | 37.4 us: 1.02x slower                                            |
| pathlib                 | 18.9 ms                                                      | 19.2 ms: 1.02x slower                                            |
| json_dumps              | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                            |
| spectral_norm           | 91.6 ms                                                      | 93.4 ms: 1.02x slower                                            |
| deepcopy                | 368 us                                                       | 376 us: 1.02x slower                                             |
| pickle_pure_python      | 318 us                                                       | 326 us: 1.02x slower                                             |
| float                   | 76.6 ms                                                      | 78.8 ms: 1.03x slower                                            |
| create_gc_cycles        | 1.59 ms                                                      | 1.64 ms: 1.03x slower                                            |
| xml_etree_iterparse     | 103 ms                                                       | 106 ms: 1.03x slower                                             |
| pycparser               | 1.23 sec                                                     | 1.27 sec: 1.03x slower                                           |
| pickle_dict             | 32.5 us                                                      | 33.6 us: 1.03x slower                                            |
| xml_etree_parse         | 144 ms                                                       | 150 ms: 1.04x slower                                             |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.43 ms: 1.05x slower                                            |
| bench_mp_pool           | 4.76 ms                                                      | 5.05 ms: 1.06x slower                                            |
| gc_traversal            | 3.48 ms                                                      | 4.06 ms: 1.17x slower                                            |
| coverage                | 66.7 ms                                                      | 89.0 ms: 1.33x slower                                            |
| dask                    | 392 ms                                                       | 562 ms: 1.43x slower                                             |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (13): unpickle_pure_python, asyncio_tcp, xml_etree_process, regex_dna, unpickle_list, sqlglot_optimize, regex_compile, pyflate, pickle_list, docutils, typing_runtime_protocols, bench_thread_pool, mako
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 62.95% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x