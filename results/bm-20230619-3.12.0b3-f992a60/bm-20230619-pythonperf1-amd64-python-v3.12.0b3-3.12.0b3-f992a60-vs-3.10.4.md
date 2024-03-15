
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b3
- machine: windows-amd64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 217 ms: 1.13x faster                                            |
| docutils       | 1.92 sec                                                    | 1.66 sec: 1.16x faster                                          |
| tornado_http   | 108 ms                                                      | 90.2 ms: 1.20x faster                                           |
| Geometric mean | (ref)                                                       | 1.16x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 352 ms: 1.50x faster                                            |
| async_tree_io           | 1.11 sec                                                    | 744 ms: 1.49x faster                                            |
| async_tree_none         | 435 ms                                                      | 292 ms: 1.49x faster                                            |
| async_tree_cpu_io_mixed | 638 ms                                                      | 493 ms: 1.29x faster                                            |
| Geometric mean          | (ref)                                                       | 1.44x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.0 ms: 1.14x faster                                           |
| nbody          | 71.3 ms                                                     | 67.6 ms: 1.05x faster                                           |
| pidigits       | 149 ms                                                      | 154 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                       | 1.05x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 87.5 ms: 1.21x faster                                           |
| regex_dna      | 136 ms                                                      | 122 ms: 1.12x faster                                            |
| regex_v8       | 15.4 ms                                                     | 14.0 ms: 1.10x faster                                           |
| regex_effbot   | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                           |
| Geometric mean | (ref)                                                       | 1.11x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.79 ms: 1.58x faster                                           |
| pickle_pure_python   | 270 us                                                      | 194 us: 1.39x faster                                            |
| unpickle_pure_python | 183 us                                                      | 132 us: 1.39x faster                                            |
| tomli_loads          | 1.67 sec                                                    | 1.38 sec: 1.21x faster                                          |
| xml_etree_process    | 44.5 ms                                                     | 38.1 ms: 1.17x faster                                           |
| unpickle             | 9.09 us                                                     | 8.28 us: 1.10x faster                                           |
| xml_etree_parse      | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                           |
| json_loads           | 14.0 us                                                     | 13.5 us: 1.04x faster                                           |
| xml_etree_generate   | 55.5 ms                                                     | 56.2 ms: 1.01x slower                                           |
| pickle_list          | 2.75 us                                                     | 2.84 us: 1.03x slower                                           |
| unpickle_list        | 2.71 us                                                     | 2.83 us: 1.04x slower                                           |
| pickle_dict          | 17.2 us                                                     | 18.1 us: 1.06x slower                                           |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                    |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 17.1 ms: 1.10x slower                                           |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.88 ms: 1.31x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 94.6 us: 3.55x faster                                           |
| deltablue                | 4.19 ms                                                     | 2.07 ms: 2.02x faster                                           |
| richards_super           | 52.2 ms                                                     | 29.7 ms: 1.76x faster                                           |
| richards                 | 42.4 ms                                                     | 26.1 ms: 1.63x faster                                           |
| logging_silent           | 94.6 ns                                                     | 59.3 ns: 1.60x faster                                           |
| json_dumps               | 9.16 ms                                                     | 5.79 ms: 1.58x faster                                           |
| go                       | 139 ms                                                      | 88.3 ms: 1.57x faster                                           |
| scimark_lu               | 85.8 ms                                                     | 56.6 ms: 1.52x faster                                           |
| sqlglot_parse            | 1.22 ms                                                     | 802 us: 1.51x faster                                            |
| async_tree_memoization   | 526 ms                                                      | 352 ms: 1.50x faster                                            |
| async_tree_io            | 1.11 sec                                                    | 744 ms: 1.49x faster                                            |
| async_tree_none          | 435 ms                                                      | 292 ms: 1.49x faster                                            |
| raytrace                 | 273 ms                                                      | 184 ms: 1.48x faster                                            |
| asyncio_tcp              | 732 ms                                                      | 498 ms: 1.47x faster                                            |
| generators               | 32.4 ms                                                     | 22.0 ms: 1.47x faster                                           |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.46x faster                                           |
| chaos                    | 61.7 ms                                                     | 42.8 ms: 1.44x faster                                           |
| hexiom                   | 5.74 ms                                                     | 3.99 ms: 1.44x faster                                           |
| pickle_pure_python       | 270 us                                                      | 194 us: 1.39x faster                                            |
| unpickle_pure_python     | 183 us                                                      | 132 us: 1.39x faster                                            |
| pyflate                  | 409 ms                                                      | 297 ms: 1.38x faster                                            |
| scimark_sor              | 106 ms                                                      | 78.1 ms: 1.36x faster                                           |
| scimark_monte_carlo      | 57.3 ms                                                     | 42.6 ms: 1.34x faster                                           |
| pycparser                | 930 ms                                                      | 699 ms: 1.33x faster                                            |
| crypto_pyaes             | 62.5 ms                                                     | 47.6 ms: 1.31x faster                                           |
| mako                     | 9.03 ms                                                     | 6.88 ms: 1.31x faster                                           |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 493 ms: 1.29x faster                                            |
| mdp                      | 1.78 sec                                                    | 1.43 sec: 1.24x faster                                          |
| deepcopy_memo            | 28.8 us                                                     | 23.3 us: 1.23x faster                                           |
| regex_compile            | 106 ms                                                      | 87.5 ms: 1.21x faster                                           |
| tomli_loads              | 1.67 sec                                                    | 1.38 sec: 1.21x faster                                          |
| tornado_http             | 108 ms                                                      | 90.2 ms: 1.20x faster                                           |
| spectral_norm            | 77.3 ms                                                     | 64.6 ms: 1.20x faster                                           |
| comprehensions           | 16.5 us                                                     | 14.0 us: 1.18x faster                                           |
| pprint_pformat           | 1.22 sec                                                    | 1.04 sec: 1.18x faster                                          |
| sqlglot_optimize         | 39.8 ms                                                     | 33.9 ms: 1.17x faster                                           |
| xml_etree_process        | 44.5 ms                                                     | 38.1 ms: 1.17x faster                                           |
| docutils                 | 1.92 sec                                                    | 1.66 sec: 1.16x faster                                          |
| pprint_safe_repr         | 592 ms                                                      | 511 ms: 1.16x faster                                            |
| dulwich_log              | 50.5 ms                                                     | 44.1 ms: 1.14x faster                                           |
| float                    | 61.7 ms                                                     | 54.0 ms: 1.14x faster                                           |
| coroutines               | 16.0 ms                                                     | 14.0 ms: 1.14x faster                                           |
| 2to3                     | 246 ms                                                      | 217 ms: 1.13x faster                                            |
| aiohttp                  | 995 us                                                      | 887 us: 1.12x faster                                            |
| regex_dna                | 136 ms                                                      | 122 ms: 1.12x faster                                            |
| sqlglot_normalize        | 205 ms                                                      | 184 ms: 1.11x faster                                            |
| bench_thread_pool        | 958 us                                                      | 866 us: 1.11x faster                                            |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.47 ms: 1.10x faster                                           |
| regex_v8                 | 15.4 ms                                                     | 14.0 ms: 1.10x faster                                           |
| unpickle                 | 9.09 us                                                     | 8.28 us: 1.10x faster                                           |
| deepcopy                 | 255 us                                                      | 234 us: 1.09x faster                                            |
| nqueens                  | 66.6 ms                                                     | 61.1 ms: 1.09x faster                                           |
| create_gc_cycles         | 800 us                                                      | 744 us: 1.08x faster                                            |
| scimark_fft              | 187 ms                                                      | 175 ms: 1.07x faster                                            |
| deepcopy_reduce          | 2.20 us                                                     | 2.08 us: 1.06x faster                                           |
| nbody                    | 71.3 ms                                                     | 67.6 ms: 1.05x faster                                           |
| fannkuch                 | 256 ms                                                      | 243 ms: 1.05x faster                                            |
| xml_etree_parse          | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                           |
| json                     | 3.14 ms                                                     | 3.01 ms: 1.04x faster                                           |
| json_loads               | 14.0 us                                                     | 13.5 us: 1.04x faster                                           |
| regex_effbot             | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                           |
| sqlite_synth             | 1.91 us                                                     | 1.86 us: 1.03x faster                                           |
| meteor_contest           | 75.9 ms                                                     | 73.9 ms: 1.03x faster                                           |
| unpack_sequence          | 39.6 ns                                                     | 38.8 ns: 1.02x faster                                           |
| xml_etree_generate       | 55.5 ms                                                     | 56.2 ms: 1.01x slower                                           |
| logging_format           | 6.76 us                                                     | 6.91 us: 1.02x slower                                           |
| pidigits                 | 149 ms                                                      | 154 ms: 1.03x slower                                            |
| pickle_list              | 2.75 us                                                     | 2.84 us: 1.03x slower                                           |
| logging_simple           | 6.22 us                                                     | 6.44 us: 1.04x slower                                           |
| telco                    | 3.94 ms                                                     | 4.11 ms: 1.04x slower                                           |
| unpickle_list            | 2.71 us                                                     | 2.83 us: 1.04x slower                                           |
| pickle_dict              | 17.2 us                                                     | 18.1 us: 1.06x slower                                           |
| async_generators         | 222 ms                                                      | 234 ms: 1.06x slower                                            |
| gc_traversal             | 1.41 ms                                                     | 1.53 ms: 1.09x slower                                           |
| bench_mp_pool            | 62.0 ms                                                     | 67.9 ms: 1.09x slower                                           |
| pathlib                  | 75.7 ms                                                     | 82.8 ms: 1.09x slower                                           |
| python_startup_no_site   | 15.5 ms                                                     | 17.1 ms: 1.10x slower                                           |
| dask                     | 313 ms                                                      | 370 ms: 1.18x slower                                            |
| coverage                 | 39.0 ms                                                     | 52.8 ms: 1.35x slower                                           |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                    |

Benchmark hidden because not significant (4): asyncio_tcp_ssl, python_startup, xml_etree_iterparse, pickle
Ignored benchmarks (15) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown