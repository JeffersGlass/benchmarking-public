
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b2
- machine: windows-amd64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.00x slower \*
- HPT reliability: 95.44%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 216 ms: 1.01x faster                                            |
| tornado_http   | 89.5 ms                                                     | 88.5 ms: 1.01x faster                                           |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io          | 731 ms                                                      | 744 ms: 1.02x slower                                            |
| async_tree_none        | 291 ms                                                      | 298 ms: 1.02x slower                                            |
| async_tree_memoization | 339 ms                                                      | 347 ms: 1.02x slower                                            |
| Geometric mean         | (ref)                                                       | 1.02x slower                                                    |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 68.3 ms: 1.05x faster                                           |
| float          | 56.8 ms                                                     | 55.2 ms: 1.03x faster                                           |
| pidigits       | 152 ms                                                      | 153 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| regex_dna      | 126 ms                                                      | 125 ms: 1.01x faster                                            |
| regex_compile  | 87.5 ms                                                     | 87.9 ms: 1.00x slower                                           |
| regex_effbot   | 1.62 ms                                                     | 1.63 ms: 1.00x slower                                           |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 7.11 us: 1.05x faster                                           |
| json_dumps           | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                           |
| xml_etree_parse      | 93.0 ms                                                     | 91.6 ms: 1.02x faster                                           |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                           |
| pickle_dict          | 18.4 us                                                     | 18.2 us: 1.01x faster                                           |
| pickle_pure_python   | 195 us                                                      | 197 us: 1.01x slower                                            |
| pickle_list          | 2.83 us                                                     | 2.85 us: 1.01x slower                                           |
| unpickle_pure_python | 133 us                                                      | 135 us: 1.01x slower                                            |
| xml_etree_process    | 37.7 ms                                                     | 38.3 ms: 1.02x slower                                           |
| xml_etree_generate   | 55.8 ms                                                     | 57.0 ms: 1.02x slower                                           |
| unpickle             | 8.18 us                                                     | 8.48 us: 1.04x slower                                           |
| unpickle_list        | 2.75 us                                                     | 2.90 us: 1.05x slower                                           |
| Geometric mean       | (ref)                                                       | 1.00x slower                                                    |

Benchmark hidden because not significant (2): xml_etree_iterparse, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.2 ms: 1.04x slower                                           |
| python_startup_no_site | 16.2 ms                                                     | 17.4 ms: 1.07x slower                                           |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                    |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| richards                | 28.4 ms                                                     | 25.7 ms: 1.10x faster                                           |
| richards_super          | 32.1 ms                                                     | 29.2 ms: 1.10x faster                                           |
| scimark_fft             | 184 ms                                                      | 174 ms: 1.06x faster                                            |
| nbody                   | 71.9 ms                                                     | 68.3 ms: 1.05x faster                                           |
| pickle                  | 7.43 us                                                     | 7.11 us: 1.05x faster                                           |
| go                      | 91.6 ms                                                     | 87.8 ms: 1.04x faster                                           |
| deltablue               | 2.16 ms                                                     | 2.08 ms: 1.04x faster                                           |
| scimark_lu              | 58.9 ms                                                     | 56.8 ms: 1.04x faster                                           |
| float                   | 56.8 ms                                                     | 55.2 ms: 1.03x faster                                           |
| nqueens                 | 62.8 ms                                                     | 61.1 ms: 1.03x faster                                           |
| raytrace                | 192 ms                                                      | 187 ms: 1.03x faster                                            |
| fannkuch                | 247 ms                                                      | 240 ms: 1.03x faster                                            |
| crypto_pyaes            | 48.5 ms                                                     | 47.2 ms: 1.03x faster                                           |
| pycparser               | 699 ms                                                      | 680 ms: 1.03x faster                                            |
| scimark_monte_carlo     | 43.7 ms                                                     | 42.6 ms: 1.03x faster                                           |
| coroutines              | 14.3 ms                                                     | 13.9 ms: 1.03x faster                                           |
| async_generators        | 239 ms                                                      | 233 ms: 1.03x faster                                            |
| hexiom                  | 4.10 ms                                                     | 4.00 ms: 1.02x faster                                           |
| sqlglot_normalize       | 187 ms                                                      | 183 ms: 1.02x faster                                            |
| regex_v8                | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| sqlglot_optimize        | 34.5 ms                                                     | 33.8 ms: 1.02x faster                                           |
| scimark_sor             | 78.8 ms                                                     | 77.3 ms: 1.02x faster                                           |
| logging_silent          | 60.5 ns                                                     | 59.4 ns: 1.02x faster                                           |
| json_dumps              | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                           |
| json                    | 3.05 ms                                                     | 2.99 ms: 1.02x faster                                           |
| bench_mp_pool           | 69.2 ms                                                     | 68.0 ms: 1.02x faster                                           |
| xml_etree_parse         | 93.0 ms                                                     | 91.6 ms: 1.02x faster                                           |
| spectral_norm           | 66.9 ms                                                     | 66.0 ms: 1.01x faster                                           |
| regex_dna               | 126 ms                                                      | 125 ms: 1.01x faster                                            |
| json_loads              | 13.9 us                                                     | 13.7 us: 1.01x faster                                           |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.52 ms: 1.01x faster                                           |
| pickle_dict             | 18.4 us                                                     | 18.2 us: 1.01x faster                                           |
| sqlglot_transpile       | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                           |
| 2to3                    | 218 ms                                                      | 216 ms: 1.01x faster                                            |
| tornado_http            | 89.5 ms                                                     | 88.5 ms: 1.01x faster                                           |
| chaos                   | 43.3 ms                                                     | 42.8 ms: 1.01x faster                                           |
| create_gc_cycles        | 752 us                                                      | 744 us: 1.01x faster                                            |
| pprint_pformat          | 1.05 sec                                                    | 1.03 sec: 1.01x faster                                          |
| meteor_contest          | 74.6 ms                                                     | 73.9 ms: 1.01x faster                                           |
| sqlglot_parse           | 804 us                                                      | 799 us: 1.01x faster                                            |
| pprint_safe_repr        | 513 ms                                                      | 510 ms: 1.01x faster                                            |
| mdp                     | 1.37 sec                                                    | 1.38 sec: 1.00x slower                                          |
| deepcopy_memo           | 23.7 us                                                     | 23.8 us: 1.00x slower                                           |
| regex_compile           | 87.5 ms                                                     | 87.9 ms: 1.00x slower                                           |
| pyflate                 | 295 ms                                                      | 296 ms: 1.00x slower                                            |
| regex_effbot            | 1.62 ms                                                     | 1.63 ms: 1.00x slower                                           |
| pickle_pure_python      | 195 us                                                      | 197 us: 1.01x slower                                            |
| pidigits                | 152 ms                                                      | 153 ms: 1.01x slower                                            |
| pickle_list             | 2.83 us                                                     | 2.85 us: 1.01x slower                                           |
| unpickle_pure_python    | 133 us                                                      | 135 us: 1.01x slower                                            |
| deepcopy                | 238 us                                                      | 241 us: 1.01x slower                                            |
| sqlite_synth            | 1.76 us                                                     | 1.79 us: 1.02x slower                                           |
| xml_etree_process       | 37.7 ms                                                     | 38.3 ms: 1.02x slower                                           |
| comprehensions          | 14.1 us                                                     | 14.4 us: 1.02x slower                                           |
| async_tree_io           | 731 ms                                                      | 744 ms: 1.02x slower                                            |
| xml_etree_generate      | 55.8 ms                                                     | 57.0 ms: 1.02x slower                                           |
| async_tree_none         | 291 ms                                                      | 298 ms: 1.02x slower                                            |
| async_tree_memoization  | 339 ms                                                      | 347 ms: 1.02x slower                                            |
| pathlib                 | 80.5 ms                                                     | 83.2 ms: 1.03x slower                                           |
| unpickle                | 8.18 us                                                     | 8.48 us: 1.04x slower                                           |
| python_startup          | 19.5 ms                                                     | 20.2 ms: 1.04x slower                                           |
| logging_simple          | 6.28 us                                                     | 6.54 us: 1.04x slower                                           |
| logging_format          | 6.72 us                                                     | 7.01 us: 1.04x slower                                           |
| unpack_sequence         | 37.5 ns                                                     | 39.1 ns: 1.04x slower                                           |
| unpickle_list           | 2.75 us                                                     | 2.90 us: 1.05x slower                                           |
| python_startup_no_site  | 16.2 ms                                                     | 17.4 ms: 1.07x slower                                           |
| coverage                | 40.8 ms                                                     | 52.5 ms: 1.29x slower                                           |
| dask                    | 263 ms                                                      | 373 ms: 1.42x slower                                            |
| Geometric mean          | (ref)                                                       | 1.00x slower                                                    |

Benchmark hidden because not significant (15): asyncio_tcp, mako, aiohttp, asyncio_tcp_ssl, generators, xml_etree_iterparse, typing_runtime_protocols, dulwich_log, tomli_loads, deepcopy_reduce, gc_traversal, docutils, telco, async_tree_cpu_io_mixed, bench_thread_pool
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 95.44% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown