
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b4
- machine: windows-amd64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 207 ms: 1.19x faster                                            |
| docutils       | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                          |
| tornado_http   | 108 ms                                                      | 86.3 ms: 1.26x faster                                           |
| Geometric mean | (ref)                                                       | 1.21x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 333 ms: 1.58x faster                                            |
| async_tree_io           | 1.11 sec                                                    | 709 ms: 1.56x faster                                            |
| async_tree_none         | 435 ms                                                      | 287 ms: 1.52x faster                                            |
| async_tree_cpu_io_mixed | 638 ms                                                      | 475 ms: 1.34x faster                                            |
| Geometric mean          | (ref)                                                       | 1.50x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.6 ms: 1.15x faster                                           |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                            |
| nbody          | 71.3 ms                                                     | 74.4 ms: 1.04x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 87.2 ms: 1.22x faster                                           |
| regex_v8       | 15.4 ms                                                     | 13.0 ms: 1.19x faster                                           |
| regex_dna      | 136 ms                                                      | 115 ms: 1.18x faster                                            |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                           |
| Geometric mean | (ref)                                                       | 1.16x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.50 ms: 1.67x faster                                           |
| pickle_pure_python   | 270 us                                                      | 195 us: 1.38x faster                                            |
| unpickle_pure_python | 183 us                                                      | 135 us: 1.36x faster                                            |
| xml_etree_process    | 44.5 ms                                                     | 37.4 ms: 1.19x faster                                           |
| tomli_loads          | 1.67 sec                                                    | 1.41 sec: 1.18x faster                                          |
| unpickle             | 9.09 us                                                     | 8.23 us: 1.10x faster                                           |
| xml_etree_parse      | 96.8 ms                                                     | 91.5 ms: 1.06x faster                                           |
| json_loads           | 14.0 us                                                     | 13.4 us: 1.04x faster                                           |
| xml_etree_generate   | 55.5 ms                                                     | 55.0 ms: 1.01x faster                                           |
| pickle               | 6.85 us                                                     | 7.05 us: 1.03x slower                                           |
| pickle_list          | 2.75 us                                                     | 2.89 us: 1.05x slower                                           |
| unpickle_list        | 2.71 us                                                     | 2.90 us: 1.07x slower                                           |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                           |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                    |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.1 ms: 1.08x faster                                           |
| python_startup_no_site | 15.5 ms                                                     | 16.4 ms: 1.06x slower                                           |
| Geometric mean         | (ref)                                                       | 1.01x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.86 ms: 1.32x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 93.3 us: 3.60x faster                                           |
| deltablue                | 4.19 ms                                                     | 2.10 ms: 1.99x faster                                           |
| richards_super           | 52.2 ms                                                     | 30.2 ms: 1.73x faster                                           |
| json_dumps               | 9.16 ms                                                     | 5.50 ms: 1.67x faster                                           |
| logging_silent           | 94.6 ns                                                     | 59.4 ns: 1.59x faster                                           |
| richards                 | 42.4 ms                                                     | 26.8 ms: 1.58x faster                                           |
| async_tree_memoization   | 526 ms                                                      | 333 ms: 1.58x faster                                            |
| go                       | 139 ms                                                      | 88.2 ms: 1.57x faster                                           |
| async_tree_io            | 1.11 sec                                                    | 709 ms: 1.56x faster                                            |
| asyncio_tcp              | 732 ms                                                      | 474 ms: 1.54x faster                                            |
| async_tree_none          | 435 ms                                                      | 287 ms: 1.52x faster                                            |
| sqlglot_parse            | 1.22 ms                                                     | 802 us: 1.51x faster                                            |
| scimark_lu               | 85.8 ms                                                     | 57.6 ms: 1.49x faster                                           |
| raytrace                 | 273 ms                                                      | 186 ms: 1.47x faster                                            |
| generators               | 32.4 ms                                                     | 22.2 ms: 1.46x faster                                           |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.45x faster                                           |
| chaos                    | 61.7 ms                                                     | 43.3 ms: 1.42x faster                                           |
| pycparser                | 930 ms                                                      | 667 ms: 1.39x faster                                            |
| hexiom                   | 5.74 ms                                                     | 4.14 ms: 1.39x faster                                           |
| pickle_pure_python       | 270 us                                                      | 195 us: 1.38x faster                                            |
| pyflate                  | 409 ms                                                      | 298 ms: 1.37x faster                                            |
| unpickle_pure_python     | 183 us                                                      | 135 us: 1.36x faster                                            |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 475 ms: 1.34x faster                                            |
| crypto_pyaes             | 62.5 ms                                                     | 46.8 ms: 1.34x faster                                           |
| scimark_monte_carlo      | 57.3 ms                                                     | 43.0 ms: 1.33x faster                                           |
| mako                     | 9.03 ms                                                     | 6.86 ms: 1.32x faster                                           |
| scimark_sor              | 106 ms                                                      | 82.6 ms: 1.29x faster                                           |
| tornado_http             | 108 ms                                                      | 86.3 ms: 1.26x faster                                           |
| regex_compile            | 106 ms                                                      | 87.2 ms: 1.22x faster                                           |
| dulwich_log              | 50.5 ms                                                     | 42.1 ms: 1.20x faster                                           |
| mdp                      | 1.78 sec                                                    | 1.49 sec: 1.19x faster                                          |
| docutils                 | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                          |
| xml_etree_process        | 44.5 ms                                                     | 37.4 ms: 1.19x faster                                           |
| spectral_norm            | 77.3 ms                                                     | 65.1 ms: 1.19x faster                                           |
| regex_v8                 | 15.4 ms                                                     | 13.0 ms: 1.19x faster                                           |
| 2to3                     | 246 ms                                                      | 207 ms: 1.19x faster                                            |
| tomli_loads              | 1.67 sec                                                    | 1.41 sec: 1.18x faster                                          |
| regex_dna                | 136 ms                                                      | 115 ms: 1.18x faster                                            |
| sqlglot_optimize         | 39.8 ms                                                     | 33.7 ms: 1.18x faster                                           |
| comprehensions           | 16.5 us                                                     | 14.0 us: 1.18x faster                                           |
| aiohttp                  | 995 us                                                      | 849 us: 1.17x faster                                            |
| pprint_pformat           | 1.22 sec                                                    | 1.05 sec: 1.16x faster                                          |
| deepcopy_memo            | 28.8 us                                                     | 24.9 us: 1.16x faster                                           |
| pprint_safe_repr         | 592 ms                                                      | 514 ms: 1.15x faster                                            |
| float                    | 61.7 ms                                                     | 53.6 ms: 1.15x faster                                           |
| bench_thread_pool        | 958 us                                                      | 836 us: 1.15x faster                                            |
| coroutines               | 16.0 ms                                                     | 14.0 ms: 1.14x faster                                           |
| sqlglot_normalize        | 205 ms                                                      | 181 ms: 1.13x faster                                            |
| create_gc_cycles         | 800 us                                                      | 724 us: 1.10x faster                                            |
| unpickle                 | 9.09 us                                                     | 8.23 us: 1.10x faster                                           |
| deepcopy                 | 255 us                                                      | 231 us: 1.10x faster                                            |
| sqlite_synth             | 1.91 us                                                     | 1.75 us: 1.09x faster                                           |
| deepcopy_reduce          | 2.20 us                                                     | 2.03 us: 1.08x faster                                           |
| nqueens                  | 66.6 ms                                                     | 61.6 ms: 1.08x faster                                           |
| json                     | 3.14 ms                                                     | 2.91 ms: 1.08x faster                                           |
| python_startup           | 20.6 ms                                                     | 19.1 ms: 1.08x faster                                           |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.53 ms: 1.08x faster                                           |
| xml_etree_parse          | 96.8 ms                                                     | 91.5 ms: 1.06x faster                                           |
| scimark_fft              | 187 ms                                                      | 177 ms: 1.06x faster                                            |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                           |
| json_loads               | 14.0 us                                                     | 13.4 us: 1.04x faster                                           |
| fannkuch                 | 256 ms                                                      | 248 ms: 1.03x faster                                            |
| meteor_contest           | 75.9 ms                                                     | 73.8 ms: 1.03x faster                                           |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 2.06 sec: 1.03x faster                                          |
| xml_etree_generate       | 55.5 ms                                                     | 55.0 ms: 1.01x faster                                           |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                            |
| logging_format           | 6.76 us                                                     | 6.88 us: 1.02x slower                                           |
| pickle                   | 6.85 us                                                     | 7.05 us: 1.03x slower                                           |
| pathlib                  | 75.7 ms                                                     | 78.0 ms: 1.03x slower                                           |
| async_generators         | 222 ms                                                      | 230 ms: 1.04x slower                                            |
| logging_simple           | 6.22 us                                                     | 6.46 us: 1.04x slower                                           |
| telco                    | 3.94 ms                                                     | 4.11 ms: 1.04x slower                                           |
| nbody                    | 71.3 ms                                                     | 74.4 ms: 1.04x slower                                           |
| pickle_list              | 2.75 us                                                     | 2.89 us: 1.05x slower                                           |
| bench_mp_pool            | 62.0 ms                                                     | 65.4 ms: 1.05x slower                                           |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.06x slower                                           |
| python_startup_no_site   | 15.5 ms                                                     | 16.4 ms: 1.06x slower                                           |
| unpickle_list            | 2.71 us                                                     | 2.90 us: 1.07x slower                                           |
| pickle_dict              | 17.2 us                                                     | 18.4 us: 1.07x slower                                           |
| unpack_sequence          | 39.6 ns                                                     | 44.7 ns: 1.13x slower                                           |
| dask                     | 313 ms                                                      | 359 ms: 1.15x slower                                            |
| coverage                 | 39.0 ms                                                     | 52.7 ms: 1.35x slower                                           |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                    |

Benchmark hidden because not significant (1): xml_etree_iterparse
Ignored benchmarks (15) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown