
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b1
- machine: windows-amd64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 218 ms: 1.13x faster                                            |
| docutils       | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                          |
| tornado_http   | 108 ms                                                      | 98.2 ms: 1.10x faster                                           |
| Geometric mean | (ref)                                                       | 1.13x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 351 ms: 1.50x faster                                            |
| async_tree_io           | 1.11 sec                                                    | 765 ms: 1.45x faster                                            |
| async_tree_none         | 435 ms                                                      | 309 ms: 1.41x faster                                            |
| async_tree_cpu_io_mixed | 638 ms                                                      | 494 ms: 1.29x faster                                            |
| Geometric mean          | (ref)                                                       | 1.41x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.5 ms: 1.09x faster                                           |
| nbody          | 71.3 ms                                                     | 69.0 ms: 1.03x faster                                           |
| pidigits       | 149 ms                                                      | 153 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                       | 1.03x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 89.3 ms: 1.19x faster                                           |
| regex_v8       | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                           |
| regex_dna      | 136 ms                                                      | 126 ms: 1.08x faster                                            |
| regex_effbot   | 1.66 ms                                                     | 1.62 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                       | 1.10x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.68 ms: 1.61x faster                                           |
| pickle_pure_python   | 270 us                                                      | 196 us: 1.38x faster                                            |
| unpickle_pure_python | 183 us                                                      | 137 us: 1.33x faster                                            |
| tomli_loads          | 1.67 sec                                                    | 1.39 sec: 1.20x faster                                          |
| xml_etree_process    | 44.5 ms                                                     | 38.6 ms: 1.15x faster                                           |
| unpickle             | 9.09 us                                                     | 8.47 us: 1.07x faster                                           |
| xml_etree_parse      | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                           |
| json_loads           | 14.0 us                                                     | 13.8 us: 1.02x faster                                           |
| xml_etree_iterparse  | 65.0 ms                                                     | 66.2 ms: 1.02x slower                                           |
| xml_etree_generate   | 55.5 ms                                                     | 56.6 ms: 1.02x slower                                           |
| pickle               | 6.85 us                                                     | 7.00 us: 1.02x slower                                           |
| pickle_list          | 2.75 us                                                     | 2.86 us: 1.04x slower                                           |
| unpickle_list        | 2.71 us                                                     | 2.92 us: 1.07x slower                                           |
| pickle_dict          | 17.2 us                                                     | 19.2 us: 1.12x slower                                           |
| Geometric mean       | (ref)                                                       | 1.09x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 17.8 ms: 1.15x slower                                           |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.24 ms: 1.25x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 94.7 us: 3.55x faster                                           |
| deltablue                | 4.19 ms                                                     | 2.20 ms: 1.90x faster                                           |
| richards_super           | 52.2 ms                                                     | 29.1 ms: 1.79x faster                                           |
| richards                 | 42.4 ms                                                     | 25.5 ms: 1.66x faster                                           |
| json_dumps               | 9.16 ms                                                     | 5.68 ms: 1.61x faster                                           |
| logging_silent           | 94.6 ns                                                     | 60.1 ns: 1.58x faster                                           |
| go                       | 139 ms                                                      | 88.2 ms: 1.57x faster                                           |
| sqlglot_parse            | 1.22 ms                                                     | 800 us: 1.52x faster                                            |
| async_tree_memoization   | 526 ms                                                      | 351 ms: 1.50x faster                                            |
| async_tree_io            | 1.11 sec                                                    | 765 ms: 1.45x faster                                            |
| sqlglot_transpile        | 1.48 ms                                                     | 1.02 ms: 1.45x faster                                           |
| scimark_lu               | 85.8 ms                                                     | 60.0 ms: 1.43x faster                                           |
| raytrace                 | 273 ms                                                      | 192 ms: 1.42x faster                                            |
| generators               | 32.4 ms                                                     | 23.0 ms: 1.41x faster                                           |
| async_tree_none          | 435 ms                                                      | 309 ms: 1.41x faster                                            |
| hexiom                   | 5.74 ms                                                     | 4.09 ms: 1.40x faster                                           |
| chaos                    | 61.7 ms                                                     | 44.3 ms: 1.39x faster                                           |
| pickle_pure_python       | 270 us                                                      | 196 us: 1.38x faster                                            |
| pyflate                  | 409 ms                                                      | 298 ms: 1.37x faster                                            |
| scimark_monte_carlo      | 57.3 ms                                                     | 42.9 ms: 1.34x faster                                           |
| unpickle_pure_python     | 183 us                                                      | 137 us: 1.33x faster                                            |
| pycparser                | 930 ms                                                      | 700 ms: 1.33x faster                                            |
| crypto_pyaes             | 62.5 ms                                                     | 47.4 ms: 1.32x faster                                           |
| scimark_sor              | 106 ms                                                      | 80.6 ms: 1.32x faster                                           |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 494 ms: 1.29x faster                                            |
| mdp                      | 1.78 sec                                                    | 1.40 sec: 1.27x faster                                          |
| mako                     | 9.03 ms                                                     | 7.24 ms: 1.25x faster                                           |
| deepcopy_memo            | 28.8 us                                                     | 23.7 us: 1.21x faster                                           |
| tomli_loads              | 1.67 sec                                                    | 1.39 sec: 1.20x faster                                          |
| regex_compile            | 106 ms                                                      | 89.3 ms: 1.19x faster                                           |
| spectral_norm            | 77.3 ms                                                     | 66.3 ms: 1.17x faster                                           |
| pprint_pformat           | 1.22 sec                                                    | 1.06 sec: 1.15x faster                                          |
| xml_etree_process        | 44.5 ms                                                     | 38.6 ms: 1.15x faster                                           |
| docutils                 | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                          |
| pprint_safe_repr         | 592 ms                                                      | 517 ms: 1.15x faster                                            |
| comprehensions           | 16.5 us                                                     | 14.4 us: 1.14x faster                                           |
| sqlglot_optimize         | 39.8 ms                                                     | 35.0 ms: 1.14x faster                                           |
| 2to3                     | 246 ms                                                      | 218 ms: 1.13x faster                                            |
| dulwich_log              | 50.5 ms                                                     | 45.3 ms: 1.11x faster                                           |
| regex_v8                 | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                           |
| coroutines               | 16.0 ms                                                     | 14.4 ms: 1.11x faster                                           |
| tornado_http             | 108 ms                                                      | 98.2 ms: 1.10x faster                                           |
| sqlglot_normalize        | 205 ms                                                      | 187 ms: 1.10x faster                                            |
| float                    | 61.7 ms                                                     | 56.5 ms: 1.09x faster                                           |
| deepcopy                 | 255 us                                                      | 236 us: 1.08x faster                                            |
| regex_dna                | 136 ms                                                      | 126 ms: 1.08x faster                                            |
| nqueens                  | 66.6 ms                                                     | 61.6 ms: 1.08x faster                                           |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.52 ms: 1.08x faster                                           |
| unpickle                 | 9.09 us                                                     | 8.47 us: 1.07x faster                                           |
| aiohttp                  | 995 us                                                      | 928 us: 1.07x faster                                            |
| sqlite_synth             | 1.91 us                                                     | 1.78 us: 1.07x faster                                           |
| bench_thread_pool        | 958 us                                                      | 895 us: 1.07x faster                                            |
| asyncio_tcp              | 732 ms                                                      | 686 ms: 1.07x faster                                            |
| json                     | 3.14 ms                                                     | 2.98 ms: 1.05x faster                                           |
| scimark_fft              | 187 ms                                                      | 178 ms: 1.05x faster                                            |
| deepcopy_reduce          | 2.20 us                                                     | 2.10 us: 1.05x faster                                           |
| create_gc_cycles         | 800 us                                                      | 766 us: 1.04x faster                                            |
| fannkuch                 | 256 ms                                                      | 246 ms: 1.04x faster                                            |
| nbody                    | 71.3 ms                                                     | 69.0 ms: 1.03x faster                                           |
| xml_etree_parse          | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                           |
| unpack_sequence          | 39.6 ns                                                     | 38.7 ns: 1.02x faster                                           |
| regex_effbot             | 1.66 ms                                                     | 1.62 ms: 1.02x faster                                           |
| json_loads               | 14.0 us                                                     | 13.8 us: 1.02x faster                                           |
| meteor_contest           | 75.9 ms                                                     | 75.2 ms: 1.01x faster                                           |
| xml_etree_iterparse      | 65.0 ms                                                     | 66.2 ms: 1.02x slower                                           |
| xml_etree_generate       | 55.5 ms                                                     | 56.6 ms: 1.02x slower                                           |
| pickle                   | 6.85 us                                                     | 7.00 us: 1.02x slower                                           |
| pidigits                 | 149 ms                                                      | 153 ms: 1.03x slower                                            |
| pickle_list              | 2.75 us                                                     | 2.86 us: 1.04x slower                                           |
| async_generators         | 222 ms                                                      | 237 ms: 1.07x slower                                            |
| telco                    | 3.94 ms                                                     | 4.23 ms: 1.07x slower                                           |
| unpickle_list            | 2.71 us                                                     | 2.92 us: 1.07x slower                                           |
| logging_format           | 6.76 us                                                     | 7.28 us: 1.08x slower                                           |
| gc_traversal             | 1.41 ms                                                     | 1.53 ms: 1.09x slower                                           |
| logging_simple           | 6.22 us                                                     | 6.77 us: 1.09x slower                                           |
| pickle_dict              | 17.2 us                                                     | 19.2 us: 1.12x slower                                           |
| bench_mp_pool            | 62.0 ms                                                     | 70.0 ms: 1.13x slower                                           |
| pathlib                  | 75.7 ms                                                     | 85.4 ms: 1.13x slower                                           |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 2.39 sec: 1.13x slower                                          |
| python_startup_no_site   | 15.5 ms                                                     | 17.8 ms: 1.15x slower                                           |
| dask                     | 313 ms                                                      | 382 ms: 1.22x slower                                            |
| coverage                 | 39.0 ms                                                     | 50.9 ms: 1.31x slower                                           |
| Geometric mean           | (ref)                                                       | 1.16x faster                                                    |

Benchmark hidden because not significant (1): python_startup
Ignored benchmarks (15) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown