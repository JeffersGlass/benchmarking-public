# Results vs. 3.10.4

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 213 ms: 1.15x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.79 ms: 1.21x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.55 sec: 1.24x faster                                                      |
| tornado_http   | 108 ms                                                      | 83.4 ms: 1.30x faster                                                       |
| Geometric mean | (ref)                                                       | 1.22x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 451 ms: 1.41x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 52.9 ms: 1.17x faster                                                       |
| nbody          | 71.3 ms                                                     | 69.7 ms: 1.02x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 77.5 ms: 1.37x faster                                                       |
| regex_dna      | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 15.3 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.58 ms: 1.64x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 181 us: 1.49x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 127 us: 1.44x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 36.0 ms: 1.23x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.44 sec: 1.16x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.28 us: 1.10x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.2 ms: 1.06x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 93.4 ms: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.6 ms: 1.02x faster                                                       |
| pickle               | 6.85 us                                                     | 7.14 us: 1.04x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.97 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.0 ms: 1.03x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 17.8 ms: 1.14x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.48 ms: 1.39x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 72.7 us: 4.62x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.02 ms: 2.08x faster                                                       |
| richards_super           | 52.2 ms                                                     | 30.3 ms: 1.72x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 56.1 ns: 1.69x faster                                                       |
| raytrace                 | 273 ms                                                      | 164 ms: 1.67x faster                                                        |
| go                       | 139 ms                                                      | 84.7 ms: 1.64x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.58 ms: 1.64x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 52.5 ms: 1.63x faster                                                       |
| async_tree_none          | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 749 us: 1.62x faster                                                        |
| chaos                    | 61.7 ms                                                     | 39.1 ms: 1.58x faster                                                       |
| richards                 | 42.4 ms                                                     | 27.0 ms: 1.57x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| comprehensions           | 16.5 us                                                     | 10.7 us: 1.53x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 479 ms: 1.53x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 3.76 ms: 1.53x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 967 us: 1.53x faster                                                        |
| generators               | 32.4 ms                                                     | 21.2 ms: 1.52x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 41.8 ms: 1.50x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 181 us: 1.49x faster                                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 39.6 ms: 1.44x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 127 us: 1.44x faster                                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 451 ms: 1.41x faster                                                        |
| pyflate                  | 409 ms                                                      | 290 ms: 1.41x faster                                                        |
| mako                     | 9.03 ms                                                     | 6.48 ms: 1.39x faster                                                       |
| scimark_sor              | 106 ms                                                      | 76.6 ms: 1.39x faster                                                       |
| regex_compile            | 106 ms                                                      | 77.5 ms: 1.37x faster                                                       |
| mypy2                    | 555 ms                                                      | 413 ms: 1.34x faster                                                        |
| sympy_sum                | 107 ms                                                      | 81.1 ms: 1.32x faster                                                       |
| pycparser                | 930 ms                                                      | 714 ms: 1.30x faster                                                        |
| tornado_http             | 108 ms                                                      | 83.4 ms: 1.30x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 22.4 us: 1.29x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.39 sec: 1.28x faster                                                      |
| spectral_norm            | 77.3 ms                                                     | 60.8 ms: 1.27x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 12.1 ms: 1.27x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 39.9 ms: 1.27x faster                                                       |
| sympy_str                | 194 ms                                                      | 155 ms: 1.26x faster                                                        |
| docutils                 | 1.92 sec                                                    | 1.55 sec: 1.24x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 36.0 ms: 1.23x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.23x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.79 ms: 1.21x faster                                                       |
| sympy_expand             | 314 ms                                                      | 262 ms: 1.20x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.76 sec: 1.20x faster                                                      |
| pprint_pformat           | 1.22 sec                                                    | 1.02 sec: 1.20x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 499 ms: 1.19x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 33.7 ms: 1.18x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 57.1 ms: 1.17x faster                                                       |
| float                    | 61.7 ms                                                     | 52.9 ms: 1.17x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.44 sec: 1.16x faster                                                      |
| bench_thread_pool        | 958 us                                                      | 830 us: 1.15x faster                                                        |
| 2to3                     | 246 ms                                                      | 213 ms: 1.15x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 179 ms: 1.15x faster                                                        |
| regex_dna                | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.41 ms: 1.13x faster                                                       |
| deepcopy                 | 255 us                                                      | 227 us: 1.13x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 2.00 us: 1.10x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.28 us: 1.10x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 735 us: 1.09x faster                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 52.2 ms: 1.06x faster                                                       |
| fannkuch                 | 256 ms                                                      | 241 ms: 1.06x faster                                                        |
| scimark_fft              | 187 ms                                                      | 177 ms: 1.06x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.40 us: 1.06x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.95 us: 1.05x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 73.1 ms: 1.04x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 93.4 ms: 1.04x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.0 ms: 1.03x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.6 ms: 1.02x faster                                                       |
| nbody                    | 71.3 ms                                                     | 69.7 ms: 1.02x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.02x faster                                                        |
| unpack_sequence          | 39.6 ns                                                     | 39.3 ns: 1.01x faster                                                       |
| pathlib                  | 75.7 ms                                                     | 75.2 ms: 1.01x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 15.3 ms: 1.01x faster                                                       |
| async_generators         | 222 ms                                                      | 228 ms: 1.03x slower                                                        |
| bench_mp_pool            | 62.0 ms                                                     | 64.1 ms: 1.03x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.14 us: 1.04x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.4 us: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.97 us: 1.08x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 17.8 ms: 1.14x slower                                                       |
| dask                     | 313 ms                                                      | 359 ms: 1.15x slower                                                        |
| coverage                 | 39.0 ms                                                     | 47.0 ms: 1.21x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.85 ms: 1.23x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.24x faster                                                                |

Benchmark hidden because not significant (2): unpickle_list, json
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown