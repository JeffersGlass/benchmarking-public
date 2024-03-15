
# Results vs. 3.10.4

- fork: mdboom
- ref: aa_test
- machine: windows-amd64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 215 ms: 1.14x faster                                           |
| chameleon      | 5.79 ms                                                     | 4.78 ms: 1.21x faster                                          |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                         |
| tornado_http   | 108 ms                                                      | 84.9 ms: 1.28x faster                                          |
| Geometric mean | (ref)                                                       | 1.21x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 262 ms: 1.66x faster                                           |
| async_tree_memoization  | 526 ms                                                      | 336 ms: 1.57x faster                                           |
| async_tree_io           | 1.11 sec                                                    | 720 ms: 1.54x faster                                           |
| async_tree_cpu_io_mixed | 638 ms                                                      | 447 ms: 1.43x faster                                           |
| Geometric mean          | (ref)                                                       | 1.55x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.3 ms: 1.23x faster                                          |
| nbody          | 71.3 ms                                                     | 60.7 ms: 1.17x faster                                          |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                           |
| Geometric mean | (ref)                                                       | 1.12x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 80.4 ms: 1.32x faster                                          |
| regex_dna      | 136 ms                                                      | 115 ms: 1.18x faster                                           |
| regex_v8       | 15.4 ms                                                     | 14.4 ms: 1.07x faster                                          |
| regex_effbot   | 1.66 ms                                                     | 1.56 ms: 1.07x faster                                          |
| Geometric mean | (ref)                                                       | 1.16x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                          |
| pickle_pure_python   | 270 us                                                      | 175 us: 1.54x faster                                           |
| unpickle_pure_python | 183 us                                                      | 127 us: 1.44x faster                                           |
| tomli_loads          | 1.67 sec                                                    | 1.30 sec: 1.28x faster                                         |
| xml_etree_process    | 44.5 ms                                                     | 36.1 ms: 1.23x faster                                          |
| xml_etree_generate   | 55.5 ms                                                     | 52.0 ms: 1.07x faster                                          |
| unpickle             | 9.09 us                                                     | 8.63 us: 1.05x faster                                          |
| xml_etree_parse      | 96.8 ms                                                     | 93.1 ms: 1.04x faster                                          |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.03x faster                                          |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.8 ms: 1.02x faster                                          |
| pickle_list          | 2.75 us                                                     | 2.78 us: 1.01x slower                                          |
| pickle_dict          | 17.2 us                                                     | 17.4 us: 1.01x slower                                          |
| unpickle_list        | 2.71 us                                                     | 2.76 us: 1.02x slower                                          |
| pickle               | 6.85 us                                                     | 7.31 us: 1.07x slower                                          |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.1 ms: 1.03x faster                                          |
| python_startup_no_site | 15.5 ms                                                     | 18.1 ms: 1.17x slower                                          |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.71 ms: 1.35x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 69.8 us: 4.81x faster                                          |
| deltablue                | 4.19 ms                                                     | 1.98 ms: 2.12x faster                                          |
| richards_super           | 52.2 ms                                                     | 28.5 ms: 1.83x faster                                          |
| logging_silent           | 94.6 ns                                                     | 54.2 ns: 1.75x faster                                          |
| async_tree_none          | 435 ms                                                      | 262 ms: 1.66x faster                                           |
| json_dumps               | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                          |
| raytrace                 | 273 ms                                                      | 169 ms: 1.61x faster                                           |
| richards                 | 42.4 ms                                                     | 26.4 ms: 1.61x faster                                          |
| sqlglot_parse            | 1.22 ms                                                     | 761 us: 1.60x faster                                           |
| generators               | 32.4 ms                                                     | 20.6 ms: 1.57x faster                                          |
| asyncio_tcp              | 732 ms                                                      | 466 ms: 1.57x faster                                           |
| async_tree_memoization   | 526 ms                                                      | 336 ms: 1.57x faster                                           |
| comprehensions           | 16.5 us                                                     | 10.7 us: 1.54x faster                                          |
| pickle_pure_python       | 270 us                                                      | 175 us: 1.54x faster                                           |
| async_tree_io            | 1.11 sec                                                    | 720 ms: 1.54x faster                                           |
| sqlglot_transpile        | 1.48 ms                                                     | 976 us: 1.51x faster                                           |
| scimark_lu               | 85.8 ms                                                     | 57.2 ms: 1.50x faster                                          |
| chaos                    | 61.7 ms                                                     | 42.2 ms: 1.46x faster                                          |
| go                       | 139 ms                                                      | 95.8 ms: 1.45x faster                                          |
| unpickle_pure_python     | 183 us                                                      | 127 us: 1.44x faster                                           |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 447 ms: 1.43x faster                                           |
| mako                     | 9.03 ms                                                     | 6.71 ms: 1.35x faster                                          |
| scimark_sor              | 106 ms                                                      | 78.9 ms: 1.34x faster                                          |
| crypto_pyaes             | 62.5 ms                                                     | 46.7 ms: 1.34x faster                                          |
| deepcopy_memo            | 28.8 us                                                     | 21.6 us: 1.33x faster                                          |
| pyflate                  | 409 ms                                                      | 309 ms: 1.32x faster                                           |
| regex_compile            | 106 ms                                                      | 80.4 ms: 1.32x faster                                          |
| mypy2                    | 555 ms                                                      | 422 ms: 1.32x faster                                           |
| tomli_loads              | 1.67 sec                                                    | 1.30 sec: 1.28x faster                                         |
| sqlite_synth             | 1.91 us                                                     | 1.49 us: 1.28x faster                                          |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.65 sec: 1.28x faster                                         |
| tornado_http             | 108 ms                                                      | 84.9 ms: 1.28x faster                                          |
| dulwich_log              | 50.5 ms                                                     | 40.3 ms: 1.25x faster                                          |
| coroutines               | 16.0 ms                                                     | 12.8 ms: 1.25x faster                                          |
| pycparser                | 930 ms                                                      | 748 ms: 1.24x faster                                           |
| pprint_pformat           | 1.22 sec                                                    | 983 ms: 1.24x faster                                           |
| dask                     | 313 ms                                                      | 254 ms: 1.23x faster                                           |
| pprint_safe_repr         | 592 ms                                                      | 480 ms: 1.23x faster                                           |
| xml_etree_process        | 44.5 ms                                                     | 36.1 ms: 1.23x faster                                          |
| docutils                 | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                         |
| float                    | 61.7 ms                                                     | 50.3 ms: 1.23x faster                                          |
| sympy_sum                | 107 ms                                                      | 87.9 ms: 1.22x faster                                          |
| chameleon                | 5.79 ms                                                     | 4.78 ms: 1.21x faster                                          |
| spectral_norm            | 77.3 ms                                                     | 64.8 ms: 1.19x faster                                          |
| sympy_integrate          | 15.3 ms                                                     | 12.9 ms: 1.18x faster                                          |
| sympy_str                | 194 ms                                                      | 164 ms: 1.18x faster                                           |
| regex_dna                | 136 ms                                                      | 115 ms: 1.18x faster                                           |
| sqlglot_normalize        | 205 ms                                                      | 174 ms: 1.18x faster                                           |
| sqlglot_optimize         | 39.8 ms                                                     | 33.9 ms: 1.17x faster                                          |
| nbody                    | 71.3 ms                                                     | 60.7 ms: 1.17x faster                                          |
| deepcopy                 | 255 us                                                      | 219 us: 1.17x faster                                           |
| deepcopy_reduce          | 2.20 us                                                     | 1.91 us: 1.15x faster                                          |
| mdp                      | 1.78 sec                                                    | 1.55 sec: 1.14x faster                                         |
| 2to3                     | 246 ms                                                      | 215 ms: 1.14x faster                                           |
| bench_thread_pool        | 958 us                                                      | 847 us: 1.13x faster                                           |
| sympy_expand             | 314 ms                                                      | 281 ms: 1.12x faster                                           |
| nqueens                  | 66.6 ms                                                     | 60.2 ms: 1.11x faster                                          |
| fannkuch                 | 256 ms                                                      | 234 ms: 1.09x faster                                           |
| hexiom                   | 5.74 ms                                                     | 5.29 ms: 1.09x faster                                          |
| create_gc_cycles         | 800 us                                                      | 741 us: 1.08x faster                                           |
| regex_v8                 | 15.4 ms                                                     | 14.4 ms: 1.07x faster                                          |
| xml_etree_generate       | 55.5 ms                                                     | 52.0 ms: 1.07x faster                                          |
| regex_effbot             | 1.66 ms                                                     | 1.56 ms: 1.07x faster                                          |
| logging_format           | 6.76 us                                                     | 6.39 us: 1.06x faster                                          |
| logging_simple           | 6.22 us                                                     | 5.89 us: 1.06x faster                                          |
| unpickle                 | 9.09 us                                                     | 8.63 us: 1.05x faster                                          |
| xml_etree_parse          | 96.8 ms                                                     | 93.1 ms: 1.04x faster                                          |
| python_startup           | 20.6 ms                                                     | 20.1 ms: 1.03x faster                                          |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.03x faster                                          |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.8 ms: 1.02x faster                                          |
| pathlib                  | 75.7 ms                                                     | 74.8 ms: 1.01x faster                                          |
| unpack_sequence          | 39.6 ns                                                     | 39.3 ns: 1.01x faster                                          |
| scimark_monte_carlo      | 57.3 ms                                                     | 56.8 ms: 1.01x faster                                          |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.71 ms: 1.01x faster                                          |
| meteor_contest           | 75.9 ms                                                     | 76.3 ms: 1.01x slower                                          |
| pickle_list              | 2.75 us                                                     | 2.78 us: 1.01x slower                                          |
| pickle_dict              | 17.2 us                                                     | 17.4 us: 1.01x slower                                          |
| unpickle_list            | 2.71 us                                                     | 2.76 us: 1.02x slower                                          |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                           |
| scimark_fft              | 187 ms                                                      | 191 ms: 1.02x slower                                           |
| bench_mp_pool            | 62.0 ms                                                     | 66.2 ms: 1.07x slower                                          |
| pickle                   | 6.85 us                                                     | 7.31 us: 1.07x slower                                          |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                          |
| async_generators         | 222 ms                                                      | 241 ms: 1.09x slower                                           |
| telco                    | 3.94 ms                                                     | 4.59 ms: 1.16x slower                                          |
| python_startup_no_site   | 15.5 ms                                                     | 18.1 ms: 1.17x slower                                          |
| coverage                 | 39.0 ms                                                     | 45.9 ms: 1.18x slower                                          |
| Geometric mean           | (ref)                                                       | 1.23x faster                                                   |

Benchmark hidden because not significant (1): json
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-aaf8974-JIT/bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: unknown