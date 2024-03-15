
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0rc2
- machine: windows-amd64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.00x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 216 ms: 1.01x faster                                              |
| docutils       | 1.66 sec                                                    | 1.65 sec: 1.01x faster                                            |
| tornado_http   | 89.5 ms                                                     | 88.4 ms: 1.01x faster                                             |
| Geometric mean | (ref)                                                       | 1.01x faster                                                      |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 480 ms: 1.02x faster                                              |
| async_tree_io           | 731 ms                                                      | 722 ms: 1.01x faster                                              |
| Geometric mean          | (ref)                                                       | 1.01x faster                                                      |

Benchmark hidden because not significant (2): async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.4 ms: 1.04x faster                                             |
| nbody          | 71.9 ms                                                     | 69.0 ms: 1.04x faster                                             |
| pidigits       | 152 ms                                                      | 150 ms: 1.02x faster                                              |
| Geometric mean | (ref)                                                       | 1.03x faster                                                      |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.07x faster                                              |
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                             |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                             |
| Geometric mean | (ref)                                                       | 1.03x faster                                                      |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.97 us: 1.07x faster                                             |
| unpickle_list        | 2.75 us                                                     | 2.65 us: 1.04x faster                                             |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.8 ms: 1.04x faster                                             |
| xml_etree_parse      | 93.0 ms                                                     | 89.7 ms: 1.04x faster                                             |
| pickle_list          | 2.83 us                                                     | 2.75 us: 1.03x faster                                             |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                             |
| pickle_pure_python   | 195 us                                                      | 191 us: 1.02x faster                                              |
| unpickle_pure_python | 133 us                                                      | 130 us: 1.02x faster                                              |
| unpickle             | 8.18 us                                                     | 8.05 us: 1.02x faster                                             |
| xml_etree_generate   | 55.8 ms                                                     | 55.4 ms: 1.01x faster                                             |
| json_dumps           | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                             |
| pickle_dict          | 18.4 us                                                     | 18.3 us: 1.00x faster                                             |
| xml_etree_process    | 37.7 ms                                                     | 37.9 ms: 1.01x slower                                             |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                      |

Benchmark hidden because not significant (1): tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| python_startup | 19.5 ms                                                     | 19.3 ms: 1.01x faster                                             |
| Geometric mean | (ref)                                                       | 1.00x faster                                                      |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.00 ms: 1.01x faster                                             |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| richards                 | 28.4 ms                                                     | 26.0 ms: 1.09x faster                                             |
| richards_super           | 32.1 ms                                                     | 29.7 ms: 1.08x faster                                             |
| asyncio_tcp_ssl          | 2.10 sec                                                    | 1.96 sec: 1.07x faster                                            |
| pickle                   | 7.43 us                                                     | 6.97 us: 1.07x faster                                             |
| spectral_norm            | 66.9 ms                                                     | 62.7 ms: 1.07x faster                                             |
| regex_dna                | 126 ms                                                      | 119 ms: 1.07x faster                                              |
| go                       | 91.6 ms                                                     | 87.0 ms: 1.05x faster                                             |
| create_gc_cycles         | 752 us                                                      | 718 us: 1.05x faster                                              |
| scimark_fft              | 184 ms                                                      | 176 ms: 1.05x faster                                              |
| float                    | 56.8 ms                                                     | 54.4 ms: 1.04x faster                                             |
| nbody                    | 71.9 ms                                                     | 69.0 ms: 1.04x faster                                             |
| regex_v8                 | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                             |
| unpickle_list            | 2.75 us                                                     | 2.65 us: 1.04x faster                                             |
| xml_etree_iterparse      | 65.2 ms                                                     | 62.8 ms: 1.04x faster                                             |
| xml_etree_parse          | 93.0 ms                                                     | 89.7 ms: 1.04x faster                                             |
| dulwich_log              | 44.3 ms                                                     | 42.8 ms: 1.04x faster                                             |
| crypto_pyaes             | 48.5 ms                                                     | 46.9 ms: 1.03x faster                                             |
| scimark_lu               | 58.9 ms                                                     | 57.2 ms: 1.03x faster                                             |
| bench_mp_pool            | 69.2 ms                                                     | 67.3 ms: 1.03x faster                                             |
| pathlib                  | 80.5 ms                                                     | 78.3 ms: 1.03x faster                                             |
| pycparser                | 699 ms                                                      | 681 ms: 1.03x faster                                              |
| pickle_list              | 2.83 us                                                     | 2.75 us: 1.03x faster                                             |
| aiohttp                  | 884 us                                                      | 863 us: 1.03x faster                                              |
| regex_effbot             | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                             |
| json_loads               | 13.9 us                                                     | 13.6 us: 1.02x faster                                             |
| scimark_monte_carlo      | 43.7 ms                                                     | 42.8 ms: 1.02x faster                                             |
| scimark_sparse_mat_mult  | 2.56 ms                                                     | 2.50 ms: 1.02x faster                                             |
| meteor_contest           | 74.6 ms                                                     | 73.1 ms: 1.02x faster                                             |
| scimark_sor              | 78.8 ms                                                     | 77.1 ms: 1.02x faster                                             |
| pickle_pure_python       | 195 us                                                      | 191 us: 1.02x faster                                              |
| unpickle_pure_python     | 133 us                                                      | 130 us: 1.02x faster                                              |
| json                     | 3.05 ms                                                     | 2.99 ms: 1.02x faster                                             |
| async_tree_cpu_io_mixed  | 489 ms                                                      | 480 ms: 1.02x faster                                              |
| unpickle                 | 8.18 us                                                     | 8.05 us: 1.02x faster                                             |
| chaos                    | 43.3 ms                                                     | 42.6 ms: 1.02x faster                                             |
| hexiom                   | 4.10 ms                                                     | 4.04 ms: 1.02x faster                                             |
| pidigits                 | 152 ms                                                      | 150 ms: 1.02x faster                                              |
| deltablue                | 2.16 ms                                                     | 2.13 ms: 1.01x faster                                             |
| tornado_http             | 89.5 ms                                                     | 88.4 ms: 1.01x faster                                             |
| mako                     | 7.09 ms                                                     | 7.00 ms: 1.01x faster                                             |
| async_tree_io            | 731 ms                                                      | 722 ms: 1.01x faster                                              |
| raytrace                 | 192 ms                                                      | 190 ms: 1.01x faster                                              |
| python_startup           | 19.5 ms                                                     | 19.3 ms: 1.01x faster                                             |
| sqlite_synth             | 1.76 us                                                     | 1.74 us: 1.01x faster                                             |
| 2to3                     | 218 ms                                                      | 216 ms: 1.01x faster                                              |
| gc_traversal             | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                             |
| docutils                 | 1.66 sec                                                    | 1.65 sec: 1.01x faster                                            |
| pprint_safe_repr         | 513 ms                                                      | 509 ms: 1.01x faster                                              |
| xml_etree_generate       | 55.8 ms                                                     | 55.4 ms: 1.01x faster                                             |
| json_dumps               | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                             |
| logging_simple           | 6.28 us                                                     | 6.24 us: 1.01x faster                                             |
| pyflate                  | 295 ms                                                      | 293 ms: 1.01x faster                                              |
| async_generators         | 239 ms                                                      | 238 ms: 1.00x faster                                              |
| pickle_dict              | 18.4 us                                                     | 18.3 us: 1.00x faster                                             |
| deepcopy_memo            | 23.7 us                                                     | 23.6 us: 1.00x faster                                             |
| xml_etree_process        | 37.7 ms                                                     | 37.9 ms: 1.01x slower                                             |
| fannkuch                 | 247 ms                                                      | 249 ms: 1.01x slower                                              |
| deepcopy                 | 238 us                                                      | 241 us: 1.01x slower                                              |
| typing_runtime_protocols | 95.1 us                                                     | 96.2 us: 1.01x slower                                             |
| mdp                      | 1.37 sec                                                    | 1.39 sec: 1.01x slower                                            |
| telco                    | 4.13 ms                                                     | 4.19 ms: 1.01x slower                                             |
| nqueens                  | 62.8 ms                                                     | 63.9 ms: 1.02x slower                                             |
| unpack_sequence          | 37.5 ns                                                     | 38.3 ns: 1.02x slower                                             |
| deepcopy_reduce          | 2.09 us                                                     | 2.15 us: 1.03x slower                                             |
| generators               | 22.5 ms                                                     | 24.2 ms: 1.07x slower                                             |
| comprehensions           | 14.1 us                                                     | 15.3 us: 1.08x slower                                             |
| coverage                 | 40.8 ms                                                     | 50.2 ms: 1.23x slower                                             |
| coroutines               | 14.3 ms                                                     | 19.0 ms: 1.33x slower                                             |
| dask                     | 263 ms                                                      | 363 ms: 1.38x slower                                              |
| Geometric mean           | (ref)                                                       | 1.00x faster                                                      |

Benchmark hidden because not significant (14): asyncio_tcp, async_tree_none, pprint_pformat, logging_silent, async_tree_memoization, sqlglot_optimize, sqlglot_transpile, regex_compile, bench_thread_pool, sqlglot_normalize, python_startup_no_site, logging_format, sqlglot_parse, tomli_loads
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown