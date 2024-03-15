
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0rc1
- machine: windows-amd64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 211 ms: 1.17x faster                                              |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                            |
| tornado_http   | 108 ms                                                      | 87.2 ms: 1.24x faster                                             |
| Geometric mean | (ref)                                                       | 1.20x faster                                                      |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 331 ms: 1.59x faster                                              |
| async_tree_io           | 1.11 sec                                                    | 701 ms: 1.58x faster                                              |
| async_tree_none         | 435 ms                                                      | 286 ms: 1.52x faster                                              |
| async_tree_cpu_io_mixed | 638 ms                                                      | 471 ms: 1.35x faster                                              |
| Geometric mean          | (ref)                                                       | 1.51x faster                                                      |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.8 ms: 1.15x faster                                             |
| nbody          | 71.3 ms                                                     | 68.7 ms: 1.04x faster                                             |
| pidigits       | 149 ms                                                      | 147 ms: 1.02x faster                                              |
| Geometric mean | (ref)                                                       | 1.07x faster                                                      |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 85.8 ms: 1.24x faster                                             |
| regex_dna      | 136 ms                                                      | 121 ms: 1.12x faster                                              |
| regex_v8       | 15.4 ms                                                     | 13.8 ms: 1.12x faster                                             |
| regex_effbot   | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                             |
| Geometric mean | (ref)                                                       | 1.13x faster                                                      |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                             |
| pickle_pure_python   | 270 us                                                      | 191 us: 1.41x faster                                              |
| unpickle_pure_python | 183 us                                                      | 133 us: 1.38x faster                                              |
| tomli_loads          | 1.67 sec                                                    | 1.35 sec: 1.24x faster                                            |
| xml_etree_process    | 44.5 ms                                                     | 37.6 ms: 1.18x faster                                             |
| unpickle             | 9.09 us                                                     | 8.38 us: 1.08x faster                                             |
| xml_etree_parse      | 96.8 ms                                                     | 91.3 ms: 1.06x faster                                             |
| json_loads           | 14.0 us                                                     | 13.5 us: 1.04x faster                                             |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.1 ms: 1.03x faster                                             |
| xml_etree_generate   | 55.5 ms                                                     | 55.1 ms: 1.01x faster                                             |
| pickle               | 6.85 us                                                     | 6.98 us: 1.02x slower                                             |
| unpickle_list        | 2.71 us                                                     | 2.79 us: 1.03x slower                                             |
| pickle_list          | 2.75 us                                                     | 2.87 us: 1.04x slower                                             |
| pickle_dict          | 17.2 us                                                     | 18.3 us: 1.06x slower                                             |
| Geometric mean       | (ref)                                                       | 1.12x faster                                                      |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.7 ms: 1.10x faster                                             |
| python_startup_no_site | 15.5 ms                                                     | 16.1 ms: 1.04x slower                                             |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                      |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.82 ms: 1.32x faster                                             |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf1-amd64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 93.3 us: 3.60x faster                                             |
| deltablue                | 4.19 ms                                                     | 2.13 ms: 1.96x faster                                             |
| richards_super           | 52.2 ms                                                     | 29.5 ms: 1.77x faster                                             |
| json_dumps               | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                             |
| richards                 | 42.4 ms                                                     | 26.1 ms: 1.62x faster                                             |
| go                       | 139 ms                                                      | 86.3 ms: 1.61x faster                                             |
| async_tree_memoization   | 526 ms                                                      | 331 ms: 1.59x faster                                              |
| async_tree_io            | 1.11 sec                                                    | 701 ms: 1.58x faster                                              |
| logging_silent           | 94.6 ns                                                     | 60.0 ns: 1.58x faster                                             |
| asyncio_tcp              | 732 ms                                                      | 470 ms: 1.56x faster                                              |
| async_tree_none          | 435 ms                                                      | 286 ms: 1.52x faster                                              |
| sqlglot_parse            | 1.22 ms                                                     | 800 us: 1.52x faster                                              |
| scimark_lu               | 85.8 ms                                                     | 57.1 ms: 1.50x faster                                             |
| raytrace                 | 273 ms                                                      | 184 ms: 1.48x faster                                              |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.46x faster                                             |
| hexiom                   | 5.74 ms                                                     | 3.98 ms: 1.44x faster                                             |
| chaos                    | 61.7 ms                                                     | 42.8 ms: 1.44x faster                                             |
| generators               | 32.4 ms                                                     | 22.5 ms: 1.44x faster                                             |
| pickle_pure_python       | 270 us                                                      | 191 us: 1.41x faster                                              |
| pyflate                  | 409 ms                                                      | 292 ms: 1.40x faster                                              |
| pycparser                | 930 ms                                                      | 670 ms: 1.39x faster                                              |
| unpickle_pure_python     | 183 us                                                      | 133 us: 1.38x faster                                              |
| scimark_monte_carlo      | 57.3 ms                                                     | 41.5 ms: 1.38x faster                                             |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 471 ms: 1.35x faster                                              |
| scimark_sor              | 106 ms                                                      | 78.7 ms: 1.35x faster                                             |
| crypto_pyaes             | 62.5 ms                                                     | 46.9 ms: 1.33x faster                                             |
| mako                     | 9.03 ms                                                     | 6.82 ms: 1.32x faster                                             |
| deepcopy_memo            | 28.8 us                                                     | 22.9 us: 1.26x faster                                             |
| mdp                      | 1.78 sec                                                    | 1.43 sec: 1.25x faster                                            |
| tornado_http             | 108 ms                                                      | 87.2 ms: 1.24x faster                                             |
| tomli_loads              | 1.67 sec                                                    | 1.35 sec: 1.24x faster                                            |
| regex_compile            | 106 ms                                                      | 85.8 ms: 1.24x faster                                             |
| spectral_norm            | 77.3 ms                                                     | 64.4 ms: 1.20x faster                                             |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                            |
| pprint_pformat           | 1.22 sec                                                    | 1.02 sec: 1.19x faster                                            |
| dulwich_log              | 50.5 ms                                                     | 42.5 ms: 1.19x faster                                             |
| sqlglot_optimize         | 39.8 ms                                                     | 33.5 ms: 1.19x faster                                             |
| xml_etree_process        | 44.5 ms                                                     | 37.6 ms: 1.18x faster                                             |
| pprint_safe_repr         | 592 ms                                                      | 504 ms: 1.17x faster                                              |
| comprehensions           | 16.5 us                                                     | 14.1 us: 1.17x faster                                             |
| aiohttp                  | 995 us                                                      | 854 us: 1.17x faster                                              |
| 2to3                     | 246 ms                                                      | 211 ms: 1.17x faster                                              |
| float                    | 61.7 ms                                                     | 53.8 ms: 1.15x faster                                             |
| sqlglot_normalize        | 205 ms                                                      | 180 ms: 1.14x faster                                              |
| coroutines               | 16.0 ms                                                     | 14.0 ms: 1.14x faster                                             |
| unpack_sequence          | 39.6 ns                                                     | 35.1 ns: 1.13x faster                                             |
| bench_thread_pool        | 958 us                                                      | 852 us: 1.12x faster                                              |
| regex_dna                | 136 ms                                                      | 121 ms: 1.12x faster                                              |
| regex_v8                 | 15.4 ms                                                     | 13.8 ms: 1.12x faster                                             |
| create_gc_cycles         | 800 us                                                      | 717 us: 1.12x faster                                              |
| deepcopy                 | 255 us                                                      | 229 us: 1.11x faster                                              |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.90 sec: 1.11x faster                                            |
| sqlite_synth             | 1.91 us                                                     | 1.73 us: 1.10x faster                                             |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.47 ms: 1.10x faster                                             |
| python_startup           | 20.6 ms                                                     | 18.7 ms: 1.10x faster                                             |
| fannkuch                 | 256 ms                                                      | 236 ms: 1.09x faster                                              |
| unpickle                 | 9.09 us                                                     | 8.38 us: 1.08x faster                                             |
| nqueens                  | 66.6 ms                                                     | 61.6 ms: 1.08x faster                                             |
| scimark_fft              | 187 ms                                                      | 174 ms: 1.08x faster                                              |
| json                     | 3.14 ms                                                     | 2.91 ms: 1.08x faster                                             |
| xml_etree_parse          | 96.8 ms                                                     | 91.3 ms: 1.06x faster                                             |
| deepcopy_reduce          | 2.20 us                                                     | 2.08 us: 1.06x faster                                             |
| json_loads               | 14.0 us                                                     | 13.5 us: 1.04x faster                                             |
| meteor_contest           | 75.9 ms                                                     | 73.1 ms: 1.04x faster                                             |
| nbody                    | 71.3 ms                                                     | 68.7 ms: 1.04x faster                                             |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.1 ms: 1.03x faster                                             |
| regex_effbot             | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                             |
| pidigits                 | 149 ms                                                      | 147 ms: 1.02x faster                                              |
| xml_etree_generate       | 55.5 ms                                                     | 55.1 ms: 1.01x faster                                             |
| telco                    | 3.94 ms                                                     | 3.98 ms: 1.01x slower                                             |
| pickle                   | 6.85 us                                                     | 6.98 us: 1.02x slower                                             |
| logging_simple           | 6.22 us                                                     | 6.37 us: 1.02x slower                                             |
| unpickle_list            | 2.71 us                                                     | 2.79 us: 1.03x slower                                             |
| pathlib                  | 75.7 ms                                                     | 78.1 ms: 1.03x slower                                             |
| async_generators         | 222 ms                                                      | 229 ms: 1.03x slower                                              |
| python_startup_no_site   | 15.5 ms                                                     | 16.1 ms: 1.04x slower                                             |
| pickle_list              | 2.75 us                                                     | 2.87 us: 1.04x slower                                             |
| gc_traversal             | 1.41 ms                                                     | 1.47 ms: 1.04x slower                                             |
| pickle_dict              | 17.2 us                                                     | 18.3 us: 1.06x slower                                             |
| bench_mp_pool            | 62.0 ms                                                     | 66.3 ms: 1.07x slower                                             |
| dask                     | 313 ms                                                      | 361 ms: 1.15x slower                                              |
| coverage                 | 39.0 ms                                                     | 52.1 ms: 1.34x slower                                             |
| Geometric mean           | (ref)                                                       | 1.21x faster                                                      |

Benchmark hidden because not significant (1): logging_format
Ignored benchmarks (15) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown