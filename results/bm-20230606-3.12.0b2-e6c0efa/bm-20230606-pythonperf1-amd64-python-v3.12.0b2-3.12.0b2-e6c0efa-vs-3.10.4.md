
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b2
- machine: windows-amd64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 216 ms: 1.14x faster                                            |
| docutils       | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                          |
| tornado_http   | 108 ms                                                      | 88.5 ms: 1.22x faster                                           |
| Geometric mean | (ref)                                                       | 1.17x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 347 ms: 1.51x faster                                            |
| async_tree_io           | 1.11 sec                                                    | 744 ms: 1.49x faster                                            |
| async_tree_none         | 435 ms                                                      | 298 ms: 1.46x faster                                            |
| async_tree_cpu_io_mixed | 638 ms                                                      | 493 ms: 1.29x faster                                            |
| Geometric mean          | (ref)                                                       | 1.44x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 55.2 ms: 1.12x faster                                           |
| nbody          | 71.3 ms                                                     | 68.3 ms: 1.04x faster                                           |
| pidigits       | 149 ms                                                      | 153 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                       | 1.04x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 87.9 ms: 1.21x faster                                           |
| regex_v8       | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                           |
| regex_dna      | 136 ms                                                      | 125 ms: 1.09x faster                                            |
| regex_effbot   | 1.66 ms                                                     | 1.63 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                       | 1.11x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                           |
| pickle_pure_python   | 270 us                                                      | 197 us: 1.37x faster                                            |
| unpickle_pure_python | 183 us                                                      | 135 us: 1.36x faster                                            |
| tomli_loads          | 1.67 sec                                                    | 1.37 sec: 1.22x faster                                          |
| xml_etree_process    | 44.5 ms                                                     | 38.3 ms: 1.16x faster                                           |
| unpickle             | 9.09 us                                                     | 8.48 us: 1.07x faster                                           |
| xml_etree_parse      | 96.8 ms                                                     | 91.6 ms: 1.06x faster                                           |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                           |
| xml_etree_generate   | 55.5 ms                                                     | 57.0 ms: 1.03x slower                                           |
| pickle_list          | 2.75 us                                                     | 2.85 us: 1.03x slower                                           |
| pickle               | 6.85 us                                                     | 7.11 us: 1.04x slower                                           |
| pickle_dict          | 17.2 us                                                     | 18.2 us: 1.06x slower                                           |
| unpickle_list        | 2.71 us                                                     | 2.90 us: 1.07x slower                                           |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                    |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.2 ms: 1.02x faster                                           |
| python_startup_no_site | 15.5 ms                                                     | 17.4 ms: 1.12x slower                                           |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.05 ms: 1.28x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 95.0 us: 3.54x faster                                           |
| deltablue                | 4.19 ms                                                     | 2.08 ms: 2.01x faster                                           |
| richards_super           | 52.2 ms                                                     | 29.2 ms: 1.79x faster                                           |
| richards                 | 42.4 ms                                                     | 25.7 ms: 1.65x faster                                           |
| json_dumps               | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                           |
| logging_silent           | 94.6 ns                                                     | 59.4 ns: 1.59x faster                                           |
| go                       | 139 ms                                                      | 87.8 ms: 1.58x faster                                           |
| asyncio_tcp              | 732 ms                                                      | 478 ms: 1.53x faster                                            |
| sqlglot_parse            | 1.22 ms                                                     | 799 us: 1.52x faster                                            |
| async_tree_memoization   | 526 ms                                                      | 347 ms: 1.51x faster                                            |
| scimark_lu               | 85.8 ms                                                     | 56.8 ms: 1.51x faster                                           |
| async_tree_io            | 1.11 sec                                                    | 744 ms: 1.49x faster                                            |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.46x faster                                           |
| async_tree_none          | 435 ms                                                      | 298 ms: 1.46x faster                                            |
| raytrace                 | 273 ms                                                      | 187 ms: 1.46x faster                                            |
| generators               | 32.4 ms                                                     | 22.4 ms: 1.44x faster                                           |
| chaos                    | 61.7 ms                                                     | 42.8 ms: 1.44x faster                                           |
| hexiom                   | 5.74 ms                                                     | 4.00 ms: 1.44x faster                                           |
| pyflate                  | 409 ms                                                      | 296 ms: 1.38x faster                                            |
| scimark_sor              | 106 ms                                                      | 77.3 ms: 1.37x faster                                           |
| pickle_pure_python       | 270 us                                                      | 197 us: 1.37x faster                                            |
| pycparser                | 930 ms                                                      | 680 ms: 1.37x faster                                            |
| unpickle_pure_python     | 183 us                                                      | 135 us: 1.36x faster                                            |
| scimark_monte_carlo      | 57.3 ms                                                     | 42.6 ms: 1.34x faster                                           |
| crypto_pyaes             | 62.5 ms                                                     | 47.2 ms: 1.33x faster                                           |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 493 ms: 1.29x faster                                            |
| mdp                      | 1.78 sec                                                    | 1.38 sec: 1.29x faster                                          |
| mako                     | 9.03 ms                                                     | 7.05 ms: 1.28x faster                                           |
| tornado_http             | 108 ms                                                      | 88.5 ms: 1.22x faster                                           |
| tomli_loads              | 1.67 sec                                                    | 1.37 sec: 1.22x faster                                          |
| deepcopy_memo            | 28.8 us                                                     | 23.8 us: 1.21x faster                                           |
| regex_compile            | 106 ms                                                      | 87.9 ms: 1.21x faster                                           |
| pprint_pformat           | 1.22 sec                                                    | 1.03 sec: 1.18x faster                                          |
| sqlglot_optimize         | 39.8 ms                                                     | 33.8 ms: 1.18x faster                                           |
| spectral_norm            | 77.3 ms                                                     | 66.0 ms: 1.17x faster                                           |
| pprint_safe_repr         | 592 ms                                                      | 510 ms: 1.16x faster                                            |
| xml_etree_process        | 44.5 ms                                                     | 38.3 ms: 1.16x faster                                           |
| docutils                 | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                          |
| coroutines               | 16.0 ms                                                     | 13.9 ms: 1.15x faster                                           |
| comprehensions           | 16.5 us                                                     | 14.4 us: 1.15x faster                                           |
| dulwich_log              | 50.5 ms                                                     | 44.2 ms: 1.14x faster                                           |
| 2to3                     | 246 ms                                                      | 216 ms: 1.14x faster                                            |
| aiohttp                  | 995 us                                                      | 879 us: 1.13x faster                                            |
| sqlglot_normalize        | 205 ms                                                      | 183 ms: 1.12x faster                                            |
| float                    | 61.7 ms                                                     | 55.2 ms: 1.12x faster                                           |
| regex_v8                 | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                           |
| bench_thread_pool        | 958 us                                                      | 867 us: 1.10x faster                                            |
| regex_dna                | 136 ms                                                      | 125 ms: 1.09x faster                                            |
| nqueens                  | 66.6 ms                                                     | 61.1 ms: 1.09x faster                                           |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.52 ms: 1.08x faster                                           |
| scimark_fft              | 187 ms                                                      | 174 ms: 1.08x faster                                            |
| create_gc_cycles         | 800 us                                                      | 744 us: 1.08x faster                                            |
| unpickle                 | 9.09 us                                                     | 8.48 us: 1.07x faster                                           |
| sqlite_synth             | 1.91 us                                                     | 1.79 us: 1.07x faster                                           |
| fannkuch                 | 256 ms                                                      | 240 ms: 1.07x faster                                            |
| deepcopy                 | 255 us                                                      | 241 us: 1.06x faster                                            |
| xml_etree_parse          | 96.8 ms                                                     | 91.6 ms: 1.06x faster                                           |
| deepcopy_reduce          | 2.20 us                                                     | 2.10 us: 1.05x faster                                           |
| json                     | 3.14 ms                                                     | 2.99 ms: 1.05x faster                                           |
| nbody                    | 71.3 ms                                                     | 68.3 ms: 1.04x faster                                           |
| meteor_contest           | 75.9 ms                                                     | 73.9 ms: 1.03x faster                                           |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                           |
| regex_effbot             | 1.66 ms                                                     | 1.63 ms: 1.02x faster                                           |
| python_startup           | 20.6 ms                                                     | 20.2 ms: 1.02x faster                                           |
| unpack_sequence          | 39.6 ns                                                     | 39.1 ns: 1.01x faster                                           |
| xml_etree_generate       | 55.5 ms                                                     | 57.0 ms: 1.03x slower                                           |
| pidigits                 | 149 ms                                                      | 153 ms: 1.03x slower                                            |
| pickle_list              | 2.75 us                                                     | 2.85 us: 1.03x slower                                           |
| logging_format           | 6.76 us                                                     | 7.01 us: 1.04x slower                                           |
| pickle                   | 6.85 us                                                     | 7.11 us: 1.04x slower                                           |
| logging_simple           | 6.22 us                                                     | 6.54 us: 1.05x slower                                           |
| telco                    | 3.94 ms                                                     | 4.15 ms: 1.05x slower                                           |
| async_generators         | 222 ms                                                      | 233 ms: 1.05x slower                                            |
| pickle_dict              | 17.2 us                                                     | 18.2 us: 1.06x slower                                           |
| unpickle_list            | 2.71 us                                                     | 2.90 us: 1.07x slower                                           |
| gc_traversal             | 1.41 ms                                                     | 1.53 ms: 1.08x slower                                           |
| bench_mp_pool            | 62.0 ms                                                     | 68.0 ms: 1.10x slower                                           |
| pathlib                  | 75.7 ms                                                     | 83.2 ms: 1.10x slower                                           |
| python_startup_no_site   | 15.5 ms                                                     | 17.4 ms: 1.12x slower                                           |
| dask                     | 313 ms                                                      | 373 ms: 1.19x slower                                            |
| coverage                 | 39.0 ms                                                     | 52.5 ms: 1.35x slower                                           |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                    |

Benchmark hidden because not significant (2): asyncio_tcp_ssl, xml_etree_iterparse
Ignored benchmarks (15) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown