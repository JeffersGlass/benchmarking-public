
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b4
- machine: linux-x86_64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.01x slower \*
- HPT reliability: 55.42%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 285 ms: 1.00x faster                                             |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                           |
| Geometric mean | (ref)                                                        | 1.00x faster                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io          | 1.04 sec                                                     | 1.06 sec: 1.01x slower                                           |
| async_tree_memoization | 544 ms                                                       | 551 ms: 1.01x slower                                             |
| async_tree_none        | 452 ms                                                       | 458 ms: 1.01x slower                                             |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 85.5 ms: 1.03x faster                                            |
| pidigits       | 265 ms                                                       | 260 ms: 1.02x faster                                             |
| float          | 76.6 ms                                                      | 77.8 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                            |
| regex_dna      | 239 ms                                                       | 236 ms: 1.01x faster                                             |
| regex_compile  | 144 ms                                                       | 144 ms: 1.00x faster                                             |
| regex_v8       | 23.6 ms                                                      | 23.7 ms: 1.00x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 10.4 us: 1.01x faster                                            |
| xml_etree_generate   | 86.1 ms                                                      | 85.2 ms: 1.01x faster                                            |
| unpickle             | 14.8 us                                                      | 14.6 us: 1.01x faster                                            |
| unpickle_pure_python | 210 us                                                       | 207 us: 1.01x faster                                             |
| xml_etree_process    | 58.4 ms                                                      | 58.2 ms: 1.00x faster                                            |
| json_dumps           | 10.2 ms                                                      | 10.2 ms: 1.00x faster                                            |
| tomli_loads          | 2.16 sec                                                     | 2.18 sec: 1.01x slower                                           |
| unpickle_list        | 4.66 us                                                      | 4.74 us: 1.02x slower                                            |
| pickle_dict          | 32.5 us                                                      | 33.2 us: 1.02x slower                                            |
| json_loads           | 24.4 us                                                      | 25.1 us: 1.03x slower                                            |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                             |
| xml_etree_parse      | 144 ms                                                       | 151 ms: 1.05x slower                                             |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (2): pickle_pure_python, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.52 ms: 1.01x faster                                            |
| python_startup         | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                            |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 9.88 ms: 1.01x faster                                            |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpack_sequence         | 53.2 ns                                                      | 50.2 ns: 1.06x faster                                            |
| generators              | 37.4 ms                                                      | 36.2 ms: 1.03x faster                                            |
| richards                | 45.7 ms                                                      | 44.4 ms: 1.03x faster                                            |
| go                      | 150 ms                                                       | 145 ms: 1.03x faster                                             |
| nbody                   | 88.0 ms                                                      | 85.5 ms: 1.03x faster                                            |
| pprint_pformat          | 1.65 sec                                                     | 1.62 sec: 1.02x faster                                           |
| logging_format          | 7.48 us                                                      | 7.31 us: 1.02x faster                                            |
| chaos                   | 64.0 ms                                                      | 62.5 ms: 1.02x faster                                            |
| scimark_lu              | 98.8 ms                                                      | 96.5 ms: 1.02x faster                                            |
| fannkuch                | 350 ms                                                       | 342 ms: 1.02x faster                                             |
| pprint_safe_repr        | 807 ms                                                       | 789 ms: 1.02x faster                                             |
| mdp                     | 2.57 sec                                                     | 2.51 sec: 1.02x faster                                           |
| pidigits                | 265 ms                                                       | 260 ms: 1.02x faster                                             |
| regex_effbot            | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                            |
| hexiom                  | 5.96 ms                                                      | 5.84 ms: 1.02x faster                                            |
| scimark_sor             | 109 ms                                                       | 107 ms: 1.02x faster                                             |
| deepcopy_memo           | 36.8 us                                                      | 36.2 us: 1.02x faster                                            |
| deltablue               | 3.24 ms                                                      | 3.19 ms: 1.02x faster                                            |
| python_startup_no_site  | 8.64 ms                                                      | 8.52 ms: 1.01x faster                                            |
| mako                    | 10.0 ms                                                      | 9.88 ms: 1.01x faster                                            |
| regex_dna               | 239 ms                                                       | 236 ms: 1.01x faster                                             |
| pickle                  | 10.5 us                                                      | 10.4 us: 1.01x faster                                            |
| xml_etree_generate      | 86.1 ms                                                      | 85.2 ms: 1.01x faster                                            |
| unpickle                | 14.8 us                                                      | 14.6 us: 1.01x faster                                            |
| unpickle_pure_python    | 210 us                                                       | 207 us: 1.01x faster                                             |
| logging_simple          | 6.71 us                                                      | 6.64 us: 1.01x faster                                            |
| asyncio_tcp_ssl         | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                           |
| python_startup          | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                            |
| sqlite_synth            | 2.77 us                                                      | 2.75 us: 1.01x faster                                            |
| richards_super          | 51.3 ms                                                      | 51.0 ms: 1.01x faster                                            |
| meteor_contest          | 128 ms                                                       | 127 ms: 1.01x faster                                             |
| xml_etree_process       | 58.4 ms                                                      | 58.2 ms: 1.00x faster                                            |
| regex_compile           | 144 ms                                                       | 144 ms: 1.00x faster                                             |
| 2to3                    | 285 ms                                                       | 285 ms: 1.00x faster                                             |
| json_dumps              | 10.2 ms                                                      | 10.2 ms: 1.00x faster                                            |
| pathlib                 | 18.9 ms                                                      | 19.0 ms: 1.00x slower                                            |
| docutils                | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                           |
| regex_v8                | 23.6 ms                                                      | 23.7 ms: 1.00x slower                                            |
| scimark_monte_carlo     | 69.0 ms                                                      | 69.3 ms: 1.00x slower                                            |
| raytrace                | 298 ms                                                       | 300 ms: 1.01x slower                                             |
| sqlglot_transpile       | 1.78 ms                                                      | 1.79 ms: 1.01x slower                                            |
| crypto_pyaes            | 80.3 ms                                                      | 81.1 ms: 1.01x slower                                            |
| tomli_loads             | 2.16 sec                                                     | 2.18 sec: 1.01x slower                                           |
| deepcopy                | 368 us                                                       | 372 us: 1.01x slower                                             |
| gc_traversal            | 3.48 ms                                                      | 3.52 ms: 1.01x slower                                            |
| async_tree_io           | 1.04 sec                                                     | 1.06 sec: 1.01x slower                                           |
| async_tree_memoization  | 544 ms                                                       | 551 ms: 1.01x slower                                             |
| json                    | 5.12 ms                                                      | 5.19 ms: 1.01x slower                                            |
| asyncio_tcp             | 378 ms                                                       | 383 ms: 1.01x slower                                             |
| async_tree_none         | 452 ms                                                       | 458 ms: 1.01x slower                                             |
| sqlglot_parse           | 1.38 ms                                                      | 1.40 ms: 1.01x slower                                            |
| dulwich_log             | 65.4 ms                                                      | 66.3 ms: 1.01x slower                                            |
| float                   | 76.6 ms                                                      | 77.8 ms: 1.01x slower                                            |
| unpickle_list           | 4.66 us                                                      | 4.74 us: 1.02x slower                                            |
| pickle_dict             | 32.5 us                                                      | 33.2 us: 1.02x slower                                            |
| telco                   | 6.96 ms                                                      | 7.13 ms: 1.02x slower                                            |
| coroutines              | 23.0 ms                                                      | 23.7 ms: 1.03x slower                                            |
| json_loads              | 24.4 us                                                      | 25.1 us: 1.03x slower                                            |
| xml_etree_iterparse     | 103 ms                                                       | 107 ms: 1.04x slower                                             |
| create_gc_cycles        | 1.59 ms                                                      | 1.65 ms: 1.04x slower                                            |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.36 ms: 1.04x slower                                            |
| pyflate                 | 439 ms                                                       | 457 ms: 1.04x slower                                             |
| xml_etree_parse         | 144 ms                                                       | 151 ms: 1.05x slower                                             |
| bench_mp_pool           | 4.76 ms                                                      | 5.44 ms: 1.14x slower                                            |
| coverage                | 66.7 ms                                                      | 91.3 ms: 1.37x slower                                            |
| dask                    | 392 ms                                                       | 558 ms: 1.42x slower                                             |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (16): tornado_http, logging_silent, bench_thread_pool, sqlglot_normalize, spectral_norm, typing_runtime_protocols, nqueens, sqlglot_optimize, pycparser, async_generators, comprehensions, pickle_pure_python, deepcopy_reduce, pickle_list, scimark_fft, async_tree_cpu_io_mixed
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 55.42% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x