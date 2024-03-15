
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b3
- machine: windows-amd64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.00x faster \*
- HPT reliability: 99.54%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 217 ms: 1.01x faster                                            |
| Geometric mean | (ref)                                                       | 1.00x faster                                                    |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io          | 731 ms                                                      | 744 ms: 1.02x slower                                            |
| async_tree_memoization | 339 ms                                                      | 352 ms: 1.04x slower                                            |
| Geometric mean         | (ref)                                                       | 1.02x slower                                                    |

Benchmark hidden because not significant (2): async_tree_none, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 67.6 ms: 1.06x faster                                           |
| float          | 56.8 ms                                                     | 54.0 ms: 1.05x faster                                           |
| pidigits       | 152 ms                                                      | 154 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                       | 1.03x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 122 ms: 1.04x faster                                            |
| regex_v8       | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                           |
| regex_effbot   | 1.62 ms                                                     | 1.61 ms: 1.01x faster                                           |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.86 us: 1.08x faster                                           |
| json_loads           | 13.9 us                                                     | 13.5 us: 1.03x faster                                           |
| pickle_dict          | 18.4 us                                                     | 18.1 us: 1.02x faster                                           |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                           |
| pickle_pure_python   | 195 us                                                      | 194 us: 1.01x faster                                            |
| unpickle_pure_python | 133 us                                                      | 132 us: 1.01x faster                                            |
| pickle_list          | 2.83 us                                                     | 2.84 us: 1.00x slower                                           |
| xml_etree_generate   | 55.8 ms                                                     | 56.2 ms: 1.01x slower                                           |
| xml_etree_process    | 37.7 ms                                                     | 38.1 ms: 1.01x slower                                           |
| tomli_loads          | 1.37 sec                                                    | 1.38 sec: 1.01x slower                                          |
| unpickle             | 8.18 us                                                     | 8.28 us: 1.01x slower                                           |
| json_dumps           | 5.70 ms                                                     | 5.79 ms: 1.02x slower                                           |
| unpickle_list        | 2.75 us                                                     | 2.83 us: 1.03x slower                                           |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                    |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                           |
| python_startup_no_site | 16.2 ms                                                     | 17.1 ms: 1.05x slower                                           |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.88 ms: 1.03x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| richards                 | 28.4 ms                                                     | 26.1 ms: 1.09x faster                                           |
| pickle                   | 7.43 us                                                     | 6.86 us: 1.08x faster                                           |
| richards_super           | 32.1 ms                                                     | 29.7 ms: 1.08x faster                                           |
| nbody                    | 71.9 ms                                                     | 67.6 ms: 1.06x faster                                           |
| scimark_fft              | 184 ms                                                      | 175 ms: 1.06x faster                                            |
| float                    | 56.8 ms                                                     | 54.0 ms: 1.05x faster                                           |
| raytrace                 | 192 ms                                                      | 184 ms: 1.04x faster                                            |
| deltablue                | 2.16 ms                                                     | 2.07 ms: 1.04x faster                                           |
| scimark_lu               | 58.9 ms                                                     | 56.6 ms: 1.04x faster                                           |
| regex_dna                | 126 ms                                                      | 122 ms: 1.04x faster                                            |
| go                       | 91.6 ms                                                     | 88.3 ms: 1.04x faster                                           |
| scimark_sparse_mat_mult  | 2.56 ms                                                     | 2.47 ms: 1.04x faster                                           |
| spectral_norm            | 66.9 ms                                                     | 64.6 ms: 1.04x faster                                           |
| json_loads               | 13.9 us                                                     | 13.5 us: 1.03x faster                                           |
| mako                     | 7.09 ms                                                     | 6.88 ms: 1.03x faster                                           |
| nqueens                  | 62.8 ms                                                     | 61.1 ms: 1.03x faster                                           |
| hexiom                   | 4.10 ms                                                     | 3.99 ms: 1.03x faster                                           |
| scimark_monte_carlo      | 43.7 ms                                                     | 42.6 ms: 1.03x faster                                           |
| async_generators         | 239 ms                                                      | 234 ms: 1.02x faster                                            |
| generators               | 22.5 ms                                                     | 22.0 ms: 1.02x faster                                           |
| logging_silent           | 60.5 ns                                                     | 59.3 ns: 1.02x faster                                           |
| bench_mp_pool            | 69.2 ms                                                     | 67.9 ms: 1.02x faster                                           |
| deepcopy                 | 238 us                                                      | 234 us: 1.02x faster                                            |
| sqlglot_optimize         | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                           |
| crypto_pyaes             | 48.5 ms                                                     | 47.6 ms: 1.02x faster                                           |
| coroutines               | 14.3 ms                                                     | 14.0 ms: 1.02x faster                                           |
| deepcopy_memo            | 23.7 us                                                     | 23.3 us: 1.02x faster                                           |
| pickle_dict              | 18.4 us                                                     | 18.1 us: 1.02x faster                                           |
| regex_v8                 | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                           |
| sqlglot_normalize        | 187 ms                                                      | 184 ms: 1.01x faster                                            |
| fannkuch                 | 247 ms                                                      | 243 ms: 1.01x faster                                            |
| chaos                    | 43.3 ms                                                     | 42.8 ms: 1.01x faster                                           |
| json                     | 3.05 ms                                                     | 3.01 ms: 1.01x faster                                           |
| comprehensions           | 14.1 us                                                     | 14.0 us: 1.01x faster                                           |
| create_gc_cycles         | 752 us                                                      | 744 us: 1.01x faster                                            |
| meteor_contest           | 74.6 ms                                                     | 73.9 ms: 1.01x faster                                           |
| pprint_pformat           | 1.05 sec                                                    | 1.04 sec: 1.01x faster                                          |
| xml_etree_iterparse      | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                           |
| scimark_sor              | 78.8 ms                                                     | 78.1 ms: 1.01x faster                                           |
| sqlglot_transpile        | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                           |
| pickle_pure_python       | 195 us                                                      | 194 us: 1.01x faster                                            |
| unpickle_pure_python     | 133 us                                                      | 132 us: 1.01x faster                                            |
| 2to3                     | 218 ms                                                      | 217 ms: 1.01x faster                                            |
| regex_effbot             | 1.62 ms                                                     | 1.61 ms: 1.01x faster                                           |
| typing_runtime_protocols | 95.1 us                                                     | 94.6 us: 1.01x faster                                           |
| pickle_list              | 2.83 us                                                     | 2.84 us: 1.00x slower                                           |
| xml_etree_generate       | 55.8 ms                                                     | 56.2 ms: 1.01x slower                                           |
| gc_traversal             | 1.52 ms                                                     | 1.53 ms: 1.01x slower                                           |
| pyflate                  | 295 ms                                                      | 297 ms: 1.01x slower                                            |
| pidigits                 | 152 ms                                                      | 154 ms: 1.01x slower                                            |
| xml_etree_process        | 37.7 ms                                                     | 38.1 ms: 1.01x slower                                           |
| tomli_loads              | 1.37 sec                                                    | 1.38 sec: 1.01x slower                                          |
| unpickle                 | 8.18 us                                                     | 8.28 us: 1.01x slower                                           |
| json_dumps               | 5.70 ms                                                     | 5.79 ms: 1.02x slower                                           |
| async_tree_io            | 731 ms                                                      | 744 ms: 1.02x slower                                            |
| logging_simple           | 6.28 us                                                     | 6.44 us: 1.03x slower                                           |
| logging_format           | 6.72 us                                                     | 6.91 us: 1.03x slower                                           |
| pathlib                  | 80.5 ms                                                     | 82.8 ms: 1.03x slower                                           |
| unpickle_list            | 2.75 us                                                     | 2.83 us: 1.03x slower                                           |
| unpack_sequence          | 37.5 ns                                                     | 38.8 ns: 1.03x slower                                           |
| async_tree_memoization   | 339 ms                                                      | 352 ms: 1.04x slower                                            |
| mdp                      | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                          |
| python_startup           | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                           |
| python_startup_no_site   | 16.2 ms                                                     | 17.1 ms: 1.05x slower                                           |
| sqlite_synth             | 1.76 us                                                     | 1.86 us: 1.05x slower                                           |
| coverage                 | 40.8 ms                                                     | 52.8 ms: 1.29x slower                                           |
| dask                     | 263 ms                                                      | 370 ms: 1.41x slower                                            |
| Geometric mean           | (ref)                                                       | 1.00x faster                                                    |

Benchmark hidden because not significant (16): asyncio_tcp_ssl, deepcopy_reduce, telco, dulwich_log, pprint_safe_repr, xml_etree_parse, docutils, sqlglot_parse, regex_compile, pycparser, async_tree_none, aiohttp, tornado_http, async_tree_cpu_io_mixed, bench_thread_pool, asyncio_tcp
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 99.54% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown