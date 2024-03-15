
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0rc2
- machine: windows-amd64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 216 ms: 1.14x faster                                              |
| docutils       | 1.92 sec                                                    | 1.65 sec: 1.17x faster                                            |
| tornado_http   | 108 ms                                                      | 88.4 ms: 1.23x faster                                             |
| Geometric mean | (ref)                                                       | 1.18x faster                                                      |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 339 ms: 1.55x faster                                              |
| async_tree_io           | 1.11 sec                                                    | 722 ms: 1.53x faster                                              |
| async_tree_none         | 435 ms                                                      | 291 ms: 1.50x faster                                              |
| async_tree_cpu_io_mixed | 638 ms                                                      | 480 ms: 1.33x faster                                              |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                      |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.4 ms: 1.13x faster                                             |
| nbody          | 71.3 ms                                                     | 69.0 ms: 1.03x faster                                             |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                              |
| Geometric mean | (ref)                                                       | 1.05x faster                                                      |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 87.5 ms: 1.21x faster                                             |
| regex_dna      | 136 ms                                                      | 119 ms: 1.15x faster                                              |
| regex_v8       | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                             |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                             |
| Geometric mean | (ref)                                                       | 1.13x faster                                                      |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                             |
| pickle_pure_python   | 270 us                                                      | 191 us: 1.41x faster                                              |
| unpickle_pure_python | 183 us                                                      | 130 us: 1.40x faster                                              |
| tomli_loads          | 1.67 sec                                                    | 1.37 sec: 1.22x faster                                            |
| xml_etree_process    | 44.5 ms                                                     | 37.9 ms: 1.17x faster                                             |
| unpickle             | 9.09 us                                                     | 8.05 us: 1.13x faster                                             |
| xml_etree_parse      | 96.8 ms                                                     | 89.7 ms: 1.08x faster                                             |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.8 ms: 1.03x faster                                             |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                             |
| unpickle_list        | 2.71 us                                                     | 2.65 us: 1.02x faster                                             |
| pickle               | 6.85 us                                                     | 6.97 us: 1.02x slower                                             |
| pickle_dict          | 17.2 us                                                     | 18.3 us: 1.07x slower                                             |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                      |

Benchmark hidden because not significant (2): xml_etree_generate, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.3 ms: 1.07x faster                                             |
| python_startup_no_site | 15.5 ms                                                     | 16.3 ms: 1.05x slower                                             |
| Geometric mean         | (ref)                                                       | 1.01x faster                                                      |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.00 ms: 1.29x faster                                             |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-pythonperf1-amd64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 96.2 us: 3.49x faster                                             |
| deltablue                | 4.19 ms                                                     | 2.13 ms: 1.97x faster                                             |
| richards_super           | 52.2 ms                                                     | 29.7 ms: 1.76x faster                                             |
| richards                 | 42.4 ms                                                     | 26.0 ms: 1.63x faster                                             |
| json_dumps               | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                             |
| go                       | 139 ms                                                      | 87.0 ms: 1.60x faster                                             |
| logging_silent           | 94.6 ns                                                     | 60.3 ns: 1.57x faster                                             |
| async_tree_memoization   | 526 ms                                                      | 339 ms: 1.55x faster                                              |
| async_tree_io            | 1.11 sec                                                    | 722 ms: 1.53x faster                                              |
| asyncio_tcp              | 732 ms                                                      | 480 ms: 1.52x faster                                              |
| sqlglot_parse            | 1.22 ms                                                     | 808 us: 1.50x faster                                              |
| scimark_lu               | 85.8 ms                                                     | 57.2 ms: 1.50x faster                                             |
| async_tree_none          | 435 ms                                                      | 291 ms: 1.50x faster                                              |
| chaos                    | 61.7 ms                                                     | 42.6 ms: 1.45x faster                                             |
| sqlglot_transpile        | 1.48 ms                                                     | 1.02 ms: 1.44x faster                                             |
| raytrace                 | 273 ms                                                      | 190 ms: 1.44x faster                                              |
| hexiom                   | 5.74 ms                                                     | 4.04 ms: 1.42x faster                                             |
| pickle_pure_python       | 270 us                                                      | 191 us: 1.41x faster                                              |
| unpickle_pure_python     | 183 us                                                      | 130 us: 1.40x faster                                              |
| pyflate                  | 409 ms                                                      | 293 ms: 1.40x faster                                              |
| scimark_sor              | 106 ms                                                      | 77.1 ms: 1.38x faster                                             |
| pycparser                | 930 ms                                                      | 681 ms: 1.37x faster                                              |
| generators               | 32.4 ms                                                     | 24.2 ms: 1.34x faster                                             |
| scimark_monte_carlo      | 57.3 ms                                                     | 42.8 ms: 1.34x faster                                             |
| crypto_pyaes             | 62.5 ms                                                     | 46.9 ms: 1.33x faster                                             |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 480 ms: 1.33x faster                                              |
| mako                     | 9.03 ms                                                     | 7.00 ms: 1.29x faster                                             |
| mdp                      | 1.78 sec                                                    | 1.39 sec: 1.28x faster                                            |
| spectral_norm            | 77.3 ms                                                     | 62.7 ms: 1.23x faster                                             |
| tornado_http             | 108 ms                                                      | 88.4 ms: 1.23x faster                                             |
| deepcopy_memo            | 28.8 us                                                     | 23.6 us: 1.22x faster                                             |
| tomli_loads              | 1.67 sec                                                    | 1.37 sec: 1.22x faster                                            |
| regex_compile            | 106 ms                                                      | 87.5 ms: 1.21x faster                                             |
| dulwich_log              | 50.5 ms                                                     | 42.8 ms: 1.18x faster                                             |
| xml_etree_process        | 44.5 ms                                                     | 37.9 ms: 1.17x faster                                             |
| pprint_pformat           | 1.22 sec                                                    | 1.04 sec: 1.17x faster                                            |
| docutils                 | 1.92 sec                                                    | 1.65 sec: 1.17x faster                                            |
| pprint_safe_repr         | 592 ms                                                      | 509 ms: 1.16x faster                                              |
| sqlglot_optimize         | 39.8 ms                                                     | 34.5 ms: 1.15x faster                                             |
| aiohttp                  | 995 us                                                      | 863 us: 1.15x faster                                              |
| regex_dna                | 136 ms                                                      | 119 ms: 1.15x faster                                              |
| 2to3                     | 246 ms                                                      | 216 ms: 1.14x faster                                              |
| float                    | 61.7 ms                                                     | 54.4 ms: 1.13x faster                                             |
| unpickle                 | 9.09 us                                                     | 8.05 us: 1.13x faster                                             |
| regex_v8                 | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                             |
| bench_thread_pool        | 958 us                                                      | 857 us: 1.12x faster                                              |
| create_gc_cycles         | 800 us                                                      | 718 us: 1.11x faster                                              |
| sqlite_synth             | 1.91 us                                                     | 1.74 us: 1.10x faster                                             |
| sqlglot_normalize        | 205 ms                                                      | 187 ms: 1.10x faster                                              |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.50 ms: 1.09x faster                                             |
| comprehensions           | 16.5 us                                                     | 15.3 us: 1.08x faster                                             |
| xml_etree_parse          | 96.8 ms                                                     | 89.7 ms: 1.08x faster                                             |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.96 sec: 1.08x faster                                            |
| python_startup           | 20.6 ms                                                     | 19.3 ms: 1.07x faster                                             |
| scimark_fft              | 187 ms                                                      | 176 ms: 1.06x faster                                              |
| deepcopy                 | 255 us                                                      | 241 us: 1.06x faster                                              |
| json                     | 3.14 ms                                                     | 2.99 ms: 1.05x faster                                             |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                             |
| nqueens                  | 66.6 ms                                                     | 63.9 ms: 1.04x faster                                             |
| meteor_contest           | 75.9 ms                                                     | 73.1 ms: 1.04x faster                                             |
| unpack_sequence          | 39.6 ns                                                     | 38.3 ns: 1.03x faster                                             |
| xml_etree_iterparse      | 65.0 ms                                                     | 62.8 ms: 1.03x faster                                             |
| nbody                    | 71.3 ms                                                     | 69.0 ms: 1.03x faster                                             |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                             |
| fannkuch                 | 256 ms                                                      | 249 ms: 1.03x faster                                              |
| deepcopy_reduce          | 2.20 us                                                     | 2.15 us: 1.02x faster                                             |
| unpickle_list            | 2.71 us                                                     | 2.65 us: 1.02x faster                                             |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                              |
| pickle                   | 6.85 us                                                     | 6.97 us: 1.02x slower                                             |
| pathlib                  | 75.7 ms                                                     | 78.3 ms: 1.04x slower                                             |
| python_startup_no_site   | 15.5 ms                                                     | 16.3 ms: 1.05x slower                                             |
| telco                    | 3.94 ms                                                     | 4.19 ms: 1.06x slower                                             |
| pickle_dict              | 17.2 us                                                     | 18.3 us: 1.07x slower                                             |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                             |
| async_generators         | 222 ms                                                      | 238 ms: 1.08x slower                                              |
| bench_mp_pool            | 62.0 ms                                                     | 67.3 ms: 1.08x slower                                             |
| dask                     | 313 ms                                                      | 363 ms: 1.16x slower                                              |
| coroutines               | 16.0 ms                                                     | 19.0 ms: 1.19x slower                                             |
| coverage                 | 39.0 ms                                                     | 50.2 ms: 1.29x slower                                             |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                      |

Benchmark hidden because not significant (4): logging_format, xml_etree_generate, pickle_list, logging_simple
Ignored benchmarks (15) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown