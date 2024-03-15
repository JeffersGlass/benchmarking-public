
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.16x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 225 ms: 1.09x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.28 ms: 1.10x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.63 sec: 1.18x faster                                                      |
| tornado_http   | 108 ms                                                      | 88.0 ms: 1.23x faster                                                       |
| Geometric mean | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 275 ms: 1.58x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 354 ms: 1.49x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 754 ms: 1.47x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 471 ms: 1.35x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.47x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                                       |
| nbody          | 71.3 ms                                                     | 83.0 ms: 1.16x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 85.3 ms: 1.24x faster                                                       |
| regex_dna      | 136 ms                                                      | 129 ms: 1.06x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.63 ms: 1.02x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 18.5 ms: 1.20x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.78 ms: 1.58x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 185 us: 1.46x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 143 us: 1.28x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.60 us: 1.06x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 93.5 ms: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.9 us: 1.01x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 56.7 ms: 1.02x slower                                                       |
| pickle               | 6.85 us                                                     | 7.09 us: 1.04x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.82 us: 1.04x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 67.7 ms: 1.04x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.93 us: 1.07x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.7 us: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.09x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.44 ms: 1.21x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 74.2 us: 4.53x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 56.8 ns: 1.67x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.7 ms: 1.65x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.78 ms: 1.58x faster                                                       |
| async_tree_none          | 435 ms                                                      | 275 ms: 1.58x faster                                                        |
| deltablue                | 4.19 ms                                                     | 2.64 ms: 1.58x faster                                                       |
| raytrace                 | 273 ms                                                      | 176 ms: 1.56x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 478 ms: 1.53x faster                                                        |
| go                       | 139 ms                                                      | 91.1 ms: 1.52x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 797 us: 1.52x faster                                                        |
| richards                 | 42.4 ms                                                     | 28.1 ms: 1.51x faster                                                       |
| generators               | 32.4 ms                                                     | 21.7 ms: 1.49x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 354 ms: 1.49x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 754 ms: 1.47x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 58.4 ms: 1.47x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 185 us: 1.46x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.02 ms: 1.45x faster                                                       |
| chaos                    | 61.7 ms                                                     | 44.5 ms: 1.39x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 471 ms: 1.35x faster                                                        |
| pycparser                | 930 ms                                                      | 707 ms: 1.32x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 48.2 ms: 1.30x faster                                                       |
| mypy2                    | 555 ms                                                      | 432 ms: 1.29x faster                                                        |
| scimark_sor              | 106 ms                                                      | 83.0 ms: 1.28x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 143 us: 1.28x faster                                                        |
| pyflate                  | 409 ms                                                      | 324 ms: 1.26x faster                                                        |
| comprehensions           | 16.5 us                                                     | 13.1 us: 1.26x faster                                                       |
| regex_compile            | 106 ms                                                      | 85.3 ms: 1.24x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 23.3 us: 1.23x faster                                                       |
| tornado_http             | 108 ms                                                      | 88.0 ms: 1.23x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.46 sec: 1.22x faster                                                      |
| mako                     | 9.03 ms                                                     | 7.44 ms: 1.21x faster                                                       |
| sympy_sum                | 107 ms                                                      | 88.2 ms: 1.21x faster                                                       |
| hexiom                   | 5.74 ms                                                     | 4.79 ms: 1.20x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.60 us: 1.20x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.4 ms: 1.19x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 48.0 ms: 1.19x faster                                                       |
| dask                     | 313 ms                                                      | 264 ms: 1.18x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                                      |
| docutils                 | 1.92 sec                                                    | 1.63 sec: 1.18x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 43.6 ms: 1.16x faster                                                       |
| sympy_str                | 194 ms                                                      | 168 ms: 1.16x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.86 sec: 1.13x faster                                                      |
| sqlglot_optimize         | 39.8 ms                                                     | 35.1 ms: 1.13x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.5 ms: 1.13x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 853 us: 1.12x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.09 sec: 1.12x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 529 ms: 1.12x faster                                                        |
| sympy_expand             | 314 ms                                                      | 282 ms: 1.12x faster                                                        |
| deepcopy                 | 255 us                                                      | 230 us: 1.11x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 187 ms: 1.10x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 2.01 us: 1.10x faster                                                       |
| chameleon                | 5.79 ms                                                     | 5.28 ms: 1.10x faster                                                       |
| 2to3                     | 246 ms                                                      | 225 ms: 1.09x faster                                                        |
| float                    | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 745 us: 1.07x faster                                                        |
| json                     | 3.14 ms                                                     | 2.95 ms: 1.06x faster                                                       |
| regex_dna                | 136 ms                                                      | 129 ms: 1.06x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.60 us: 1.06x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 63.8 ms: 1.04x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 93.5 ms: 1.04x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.63 ms: 1.02x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.9 us: 1.01x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.27 us: 1.01x slower                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 56.7 ms: 1.02x slower                                                       |
| logging_format           | 6.76 us                                                     | 6.92 us: 1.02x slower                                                       |
| meteor_contest           | 75.9 ms                                                     | 78.0 ms: 1.03x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.09 us: 1.04x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.82 us: 1.04x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 67.7 ms: 1.04x slower                                                       |
| async_generators         | 222 ms                                                      | 235 ms: 1.06x slower                                                        |
| spectral_norm            | 77.3 ms                                                     | 82.2 ms: 1.06x slower                                                       |
| fannkuch                 | 256 ms                                                      | 272 ms: 1.06x slower                                                        |
| pickle_list              | 2.75 us                                                     | 2.93 us: 1.07x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 81.0 ms: 1.07x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.7 us: 1.09x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 43.2 ns: 1.09x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.54 ms: 1.10x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 68.2 ms: 1.10x slower                                                       |
| scimark_fft              | 187 ms                                                      | 211 ms: 1.13x slower                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.14 ms: 1.15x slower                                                       |
| nbody                    | 71.3 ms                                                     | 83.0 ms: 1.16x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                       |
| regex_v8                 | 15.4 ms                                                     | 18.5 ms: 1.20x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.73 ms: 1.20x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.5 ms: 1.22x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.16x faster                                                                |

Benchmark hidden because not significant (2): pidigits, python_startup
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown