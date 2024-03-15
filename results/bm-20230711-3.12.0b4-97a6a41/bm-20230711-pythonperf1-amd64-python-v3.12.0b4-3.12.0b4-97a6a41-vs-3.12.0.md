
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b4
- machine: windows-amd64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.01x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 207 ms: 1.05x faster                                            |
| docutils       | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                          |
| tornado_http   | 89.5 ms                                                     | 86.3 ms: 1.04x faster                                           |
| Geometric mean | (ref)                                                       | 1.04x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io           | 731 ms                                                      | 709 ms: 1.03x faster                                            |
| async_tree_cpu_io_mixed | 489 ms                                                      | 475 ms: 1.03x faster                                            |
| async_tree_memoization  | 339 ms                                                      | 333 ms: 1.02x faster                                            |
| async_tree_none         | 291 ms                                                      | 287 ms: 1.02x faster                                            |
| Geometric mean          | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.6 ms: 1.06x faster                                           |
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                            |
| nbody          | 71.9 ms                                                     | 74.4 ms: 1.03x slower                                           |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 115 ms: 1.10x faster                                            |
| regex_v8       | 14.2 ms                                                     | 13.0 ms: 1.09x faster                                           |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                           |
| regex_compile  | 87.5 ms                                                     | 87.2 ms: 1.00x faster                                           |
| Geometric mean | (ref)                                                       | 1.05x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 7.05 us: 1.05x faster                                           |
| json_dumps           | 5.70 ms                                                     | 5.50 ms: 1.04x faster                                           |
| json_loads           | 13.9 us                                                     | 13.4 us: 1.03x faster                                           |
| xml_etree_parse      | 93.0 ms                                                     | 91.5 ms: 1.02x faster                                           |
| xml_etree_generate   | 55.8 ms                                                     | 55.0 ms: 1.01x faster                                           |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                           |
| xml_etree_process    | 37.7 ms                                                     | 37.4 ms: 1.01x faster                                           |
| unpickle_pure_python | 133 us                                                      | 135 us: 1.01x slower                                            |
| pickle_list          | 2.83 us                                                     | 2.89 us: 1.02x slower                                           |
| tomli_loads          | 1.37 sec                                                    | 1.41 sec: 1.03x slower                                          |
| unpickle_list        | 2.75 us                                                     | 2.90 us: 1.06x slower                                           |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                    |

Benchmark hidden because not significant (3): pickle_pure_python, pickle_dict, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup | 19.5 ms                                                     | 19.1 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                       | 1.00x faster                                                    |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.86 ms: 1.03x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna                | 126 ms                                                      | 115 ms: 1.10x faster                                            |
| regex_v8                 | 14.2 ms                                                     | 13.0 ms: 1.09x faster                                           |
| richards_super           | 32.1 ms                                                     | 30.2 ms: 1.06x faster                                           |
| float                    | 56.8 ms                                                     | 53.6 ms: 1.06x faster                                           |
| richards                 | 28.4 ms                                                     | 26.8 ms: 1.06x faster                                           |
| bench_mp_pool            | 69.2 ms                                                     | 65.4 ms: 1.06x faster                                           |
| pickle                   | 7.43 us                                                     | 7.05 us: 1.05x faster                                           |
| dulwich_log              | 44.3 ms                                                     | 42.1 ms: 1.05x faster                                           |
| 2to3                     | 218 ms                                                      | 207 ms: 1.05x faster                                            |
| json                     | 3.05 ms                                                     | 2.91 ms: 1.05x faster                                           |
| pycparser                | 699 ms                                                      | 667 ms: 1.05x faster                                            |
| async_generators         | 239 ms                                                      | 230 ms: 1.04x faster                                            |
| aiohttp                  | 884 us                                                      | 849 us: 1.04x faster                                            |
| scimark_fft              | 184 ms                                                      | 177 ms: 1.04x faster                                            |
| create_gc_cycles         | 752 us                                                      | 724 us: 1.04x faster                                            |
| go                       | 91.6 ms                                                     | 88.2 ms: 1.04x faster                                           |
| tornado_http             | 89.5 ms                                                     | 86.3 ms: 1.04x faster                                           |
| raytrace                 | 192 ms                                                      | 186 ms: 1.04x faster                                            |
| crypto_pyaes             | 48.5 ms                                                     | 46.8 ms: 1.04x faster                                           |
| json_dumps               | 5.70 ms                                                     | 5.50 ms: 1.04x faster                                           |
| json_loads               | 13.9 us                                                     | 13.4 us: 1.03x faster                                           |
| mako                     | 7.09 ms                                                     | 6.86 ms: 1.03x faster                                           |
| docutils                 | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                          |
| async_tree_io            | 731 ms                                                      | 709 ms: 1.03x faster                                            |
| pathlib                  | 80.5 ms                                                     | 78.0 ms: 1.03x faster                                           |
| async_tree_cpu_io_mixed  | 489 ms                                                      | 475 ms: 1.03x faster                                            |
| sqlglot_normalize        | 187 ms                                                      | 181 ms: 1.03x faster                                            |
| deepcopy_reduce          | 2.09 us                                                     | 2.03 us: 1.03x faster                                           |
| spectral_norm            | 66.9 ms                                                     | 65.1 ms: 1.03x faster                                           |
| deepcopy                 | 238 us                                                      | 231 us: 1.03x faster                                            |
| asyncio_tcp              | 487 ms                                                      | 474 ms: 1.03x faster                                            |
| regex_effbot             | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                           |
| deltablue                | 2.16 ms                                                     | 2.10 ms: 1.03x faster                                           |
| gc_traversal             | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                           |
| sqlglot_optimize         | 34.5 ms                                                     | 33.7 ms: 1.02x faster                                           |
| scimark_lu               | 58.9 ms                                                     | 57.6 ms: 1.02x faster                                           |
| nqueens                  | 62.8 ms                                                     | 61.6 ms: 1.02x faster                                           |
| typing_runtime_protocols | 95.1 us                                                     | 93.3 us: 1.02x faster                                           |
| async_tree_memoization   | 339 ms                                                      | 333 ms: 1.02x faster                                            |
| python_startup           | 19.5 ms                                                     | 19.1 ms: 1.02x faster                                           |
| logging_silent           | 60.5 ns                                                     | 59.4 ns: 1.02x faster                                           |
| xml_etree_parse          | 93.0 ms                                                     | 91.5 ms: 1.02x faster                                           |
| scimark_monte_carlo      | 43.7 ms                                                     | 43.0 ms: 1.02x faster                                           |
| generators               | 22.5 ms                                                     | 22.2 ms: 1.02x faster                                           |
| coroutines               | 14.3 ms                                                     | 14.0 ms: 1.02x faster                                           |
| async_tree_none          | 291 ms                                                      | 287 ms: 1.02x faster                                            |
| xml_etree_generate       | 55.8 ms                                                     | 55.0 ms: 1.01x faster                                           |
| pidigits                 | 152 ms                                                      | 150 ms: 1.01x faster                                            |
| meteor_contest           | 74.6 ms                                                     | 73.8 ms: 1.01x faster                                           |
| scimark_sparse_mat_mult  | 2.56 ms                                                     | 2.53 ms: 1.01x faster                                           |
| xml_etree_iterparse      | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                           |
| comprehensions           | 14.1 us                                                     | 14.0 us: 1.01x faster                                           |
| xml_etree_process        | 37.7 ms                                                     | 37.4 ms: 1.01x faster                                           |
| sqlglot_transpile        | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                           |
| sqlite_synth             | 1.76 us                                                     | 1.75 us: 1.01x faster                                           |
| telco                    | 4.13 ms                                                     | 4.11 ms: 1.01x faster                                           |
| regex_compile            | 87.5 ms                                                     | 87.2 ms: 1.00x faster                                           |
| fannkuch                 | 247 ms                                                      | 248 ms: 1.01x slower                                            |
| hexiom                   | 4.10 ms                                                     | 4.14 ms: 1.01x slower                                           |
| pyflate                  | 295 ms                                                      | 298 ms: 1.01x slower                                            |
| unpickle_pure_python     | 133 us                                                      | 135 us: 1.01x slower                                            |
| pickle_list              | 2.83 us                                                     | 2.89 us: 1.02x slower                                           |
| logging_format           | 6.72 us                                                     | 6.88 us: 1.03x slower                                           |
| logging_simple           | 6.28 us                                                     | 6.46 us: 1.03x slower                                           |
| tomli_loads              | 1.37 sec                                                    | 1.41 sec: 1.03x slower                                          |
| nbody                    | 71.9 ms                                                     | 74.4 ms: 1.03x slower                                           |
| scimark_sor              | 78.8 ms                                                     | 82.6 ms: 1.05x slower                                           |
| deepcopy_memo            | 23.7 us                                                     | 24.9 us: 1.05x slower                                           |
| unpickle_list            | 2.75 us                                                     | 2.90 us: 1.06x slower                                           |
| mdp                      | 1.37 sec                                                    | 1.49 sec: 1.09x slower                                          |
| unpack_sequence          | 37.5 ns                                                     | 44.7 ns: 1.19x slower                                           |
| coverage                 | 40.8 ms                                                     | 52.7 ms: 1.29x slower                                           |
| dask                     | 263 ms                                                      | 359 ms: 1.37x slower                                            |
| Geometric mean           | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (10): bench_thread_pool, asyncio_tcp_ssl, pickle_pure_python, sqlglot_parse, chaos, pickle_dict, pprint_safe_repr, pprint_pformat, unpickle, python_startup_no_site
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown