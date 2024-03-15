
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b1
- machine: windows-amd64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.96%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| docutils       | 1.66 sec                                                    | 1.67 sec: 1.01x slower                                          |
| tornado_http   | 89.5 ms                                                     | 98.2 ms: 1.10x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization | 339 ms                                                      | 351 ms: 1.04x slower                                            |
| async_tree_io          | 731 ms                                                      | 765 ms: 1.05x slower                                            |
| async_tree_none        | 291 ms                                                      | 309 ms: 1.06x slower                                            |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 69.0 ms: 1.04x faster                                           |
| pidigits       | 152 ms                                                      | 153 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| regex_compile  | 87.5 ms                                                     | 89.3 ms: 1.02x slower                                           |
| Geometric mean | (ref)                                                       | 1.00x faster                                                    |

Benchmark hidden because not significant (2): regex_dna, regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 7.00 us: 1.06x faster                                           |
| json_loads           | 13.9 us                                                     | 13.8 us: 1.01x faster                                           |
| xml_etree_parse      | 93.0 ms                                                     | 93.8 ms: 1.01x slower                                           |
| pickle_list          | 2.83 us                                                     | 2.86 us: 1.01x slower                                           |
| xml_etree_generate   | 55.8 ms                                                     | 56.6 ms: 1.01x slower                                           |
| tomli_loads          | 1.37 sec                                                    | 1.39 sec: 1.02x slower                                          |
| xml_etree_iterparse  | 65.2 ms                                                     | 66.2 ms: 1.02x slower                                           |
| xml_etree_process    | 37.7 ms                                                     | 38.6 ms: 1.02x slower                                           |
| unpickle_pure_python | 133 us                                                      | 137 us: 1.03x slower                                            |
| unpickle             | 8.18 us                                                     | 8.47 us: 1.04x slower                                           |
| pickle_dict          | 18.4 us                                                     | 19.2 us: 1.04x slower                                           |
| unpickle_list        | 2.75 us                                                     | 2.92 us: 1.06x slower                                           |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                    |

Benchmark hidden because not significant (2): json_dumps, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                           |
| python_startup_no_site | 16.2 ms                                                     | 17.8 ms: 1.09x slower                                           |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.24 ms: 1.02x slower                                           |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| richards                | 28.4 ms                                                     | 25.5 ms: 1.11x faster                                           |
| richards_super          | 32.1 ms                                                     | 29.1 ms: 1.10x faster                                           |
| pickle                  | 7.43 us                                                     | 7.00 us: 1.06x faster                                           |
| nbody                   | 71.9 ms                                                     | 69.0 ms: 1.04x faster                                           |
| go                      | 91.6 ms                                                     | 88.2 ms: 1.04x faster                                           |
| scimark_fft             | 184 ms                                                      | 178 ms: 1.03x faster                                            |
| regex_v8                | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| json                    | 3.05 ms                                                     | 2.98 ms: 1.02x faster                                           |
| crypto_pyaes            | 48.5 ms                                                     | 47.4 ms: 1.02x faster                                           |
| scimark_monte_carlo     | 43.7 ms                                                     | 42.9 ms: 1.02x faster                                           |
| nqueens                 | 62.8 ms                                                     | 61.6 ms: 1.02x faster                                           |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.52 ms: 1.01x faster                                           |
| async_generators        | 239 ms                                                      | 237 ms: 1.01x faster                                            |
| deepcopy                | 238 us                                                      | 236 us: 1.01x faster                                            |
| spectral_norm           | 66.9 ms                                                     | 66.3 ms: 1.01x faster                                           |
| json_loads              | 13.9 us                                                     | 13.8 us: 1.01x faster                                           |
| logging_silent          | 60.5 ns                                                     | 60.1 ns: 1.01x faster                                           |
| sqlglot_parse           | 804 us                                                      | 800 us: 1.01x faster                                            |
| fannkuch                | 247 ms                                                      | 246 ms: 1.00x faster                                            |
| pprint_safe_repr        | 513 ms                                                      | 517 ms: 1.01x slower                                            |
| docutils                | 1.66 sec                                                    | 1.67 sec: 1.01x slower                                          |
| pidigits                | 152 ms                                                      | 153 ms: 1.01x slower                                            |
| xml_etree_parse         | 93.0 ms                                                     | 93.8 ms: 1.01x slower                                           |
| meteor_contest          | 74.6 ms                                                     | 75.2 ms: 1.01x slower                                           |
| pprint_pformat          | 1.05 sec                                                    | 1.06 sec: 1.01x slower                                          |
| pickle_list             | 2.83 us                                                     | 2.86 us: 1.01x slower                                           |
| bench_mp_pool           | 69.2 ms                                                     | 70.0 ms: 1.01x slower                                           |
| pyflate                 | 295 ms                                                      | 298 ms: 1.01x slower                                            |
| coroutines              | 14.3 ms                                                     | 14.4 ms: 1.01x slower                                           |
| xml_etree_generate      | 55.8 ms                                                     | 56.6 ms: 1.01x slower                                           |
| sqlite_synth            | 1.76 us                                                     | 1.78 us: 1.01x slower                                           |
| sqlglot_optimize        | 34.5 ms                                                     | 35.0 ms: 1.01x slower                                           |
| tomli_loads             | 1.37 sec                                                    | 1.39 sec: 1.02x slower                                          |
| xml_etree_iterparse     | 65.2 ms                                                     | 66.2 ms: 1.02x slower                                           |
| mdp                     | 1.37 sec                                                    | 1.40 sec: 1.02x slower                                          |
| create_gc_cycles        | 752 us                                                      | 766 us: 1.02x slower                                            |
| scimark_lu              | 58.9 ms                                                     | 60.0 ms: 1.02x slower                                           |
| deltablue               | 2.16 ms                                                     | 2.20 ms: 1.02x slower                                           |
| generators              | 22.5 ms                                                     | 23.0 ms: 1.02x slower                                           |
| regex_compile           | 87.5 ms                                                     | 89.3 ms: 1.02x slower                                           |
| comprehensions          | 14.1 us                                                     | 14.4 us: 1.02x slower                                           |
| mako                    | 7.09 ms                                                     | 7.24 ms: 1.02x slower                                           |
| xml_etree_process       | 37.7 ms                                                     | 38.6 ms: 1.02x slower                                           |
| chaos                   | 43.3 ms                                                     | 44.3 ms: 1.02x slower                                           |
| scimark_sor             | 78.8 ms                                                     | 80.6 ms: 1.02x slower                                           |
| dulwich_log             | 44.3 ms                                                     | 45.3 ms: 1.02x slower                                           |
| telco                   | 4.13 ms                                                     | 4.23 ms: 1.03x slower                                           |
| unpickle_pure_python    | 133 us                                                      | 137 us: 1.03x slower                                            |
| unpack_sequence         | 37.5 ns                                                     | 38.7 ns: 1.03x slower                                           |
| unpickle                | 8.18 us                                                     | 8.47 us: 1.04x slower                                           |
| async_tree_memoization  | 339 ms                                                      | 351 ms: 1.04x slower                                            |
| pickle_dict             | 18.4 us                                                     | 19.2 us: 1.04x slower                                           |
| bench_thread_pool       | 857 us                                                      | 895 us: 1.04x slower                                            |
| async_tree_io           | 731 ms                                                      | 765 ms: 1.05x slower                                            |
| aiohttp                 | 884 us                                                      | 928 us: 1.05x slower                                            |
| async_tree_none         | 291 ms                                                      | 309 ms: 1.06x slower                                            |
| unpickle_list           | 2.75 us                                                     | 2.92 us: 1.06x slower                                           |
| pathlib                 | 80.5 ms                                                     | 85.4 ms: 1.06x slower                                           |
| python_startup          | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                           |
| logging_simple          | 6.28 us                                                     | 6.77 us: 1.08x slower                                           |
| logging_format          | 6.72 us                                                     | 7.28 us: 1.08x slower                                           |
| python_startup_no_site  | 16.2 ms                                                     | 17.8 ms: 1.09x slower                                           |
| tornado_http            | 89.5 ms                                                     | 98.2 ms: 1.10x slower                                           |
| asyncio_tcp_ssl         | 2.10 sec                                                    | 2.39 sec: 1.14x slower                                          |
| coverage                | 40.8 ms                                                     | 50.9 ms: 1.25x slower                                           |
| asyncio_tcp             | 487 ms                                                      | 686 ms: 1.41x slower                                            |
| dask                    | 263 ms                                                      | 382 ms: 1.46x slower                                            |
| Geometric mean          | (ref)                                                       | 1.02x slower                                                    |

Benchmark hidden because not significant (16): float, regex_dna, typing_runtime_protocols, sqlglot_transpile, json_dumps, hexiom, raytrace, sqlglot_normalize, deepcopy_memo, pickle_pure_python, 2to3, pycparser, regex_effbot, deepcopy_reduce, gc_traversal, async_tree_cpu_io_mixed
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 99.96% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown