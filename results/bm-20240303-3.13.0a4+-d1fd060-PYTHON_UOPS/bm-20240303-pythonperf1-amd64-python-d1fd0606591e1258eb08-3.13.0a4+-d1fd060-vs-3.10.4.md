# Results vs. 3.10.4

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.15x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 224 ms: 1.10x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.74 ms: 1.22x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.63 sec: 1.17x faster                                                      |
| tornado_http   | 108 ms                                                      | 86.1 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 280 ms: 1.56x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 353 ms: 1.49x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 751 ms: 1.48x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 467 ms: 1.37x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.47x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 59.9 ms: 1.03x faster                                                       |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 80.1 ms: 1.12x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| regex_compile  | 106 ms                                                      | 99.9 ms: 1.06x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.8 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 179 us: 1.51x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.7 ms: 1.18x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 164 us: 1.11x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.53 sec: 1.09x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.49 us: 1.07x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 55.8 ms: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 66.9 ms: 1.03x slower                                                       |
| pickle               | 6.85 us                                                     | 7.24 us: 1.06x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.14 us: 1.14x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.08x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.9 ms: 1.03x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 17.7 ms: 1.14x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.70 ms: 1.17x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 76.3 us: 4.40x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.30 ms: 1.82x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.9 ns: 1.69x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                                       |
| generators               | 32.4 ms                                                     | 20.7 ms: 1.56x faster                                                       |
| async_tree_none          | 435 ms                                                      | 280 ms: 1.56x faster                                                        |
| richards_super           | 52.2 ms                                                     | 33.8 ms: 1.55x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 484 ms: 1.51x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 179 us: 1.51x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 353 ms: 1.49x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 819 us: 1.48x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 751 ms: 1.48x faster                                                        |
| richards                 | 42.4 ms                                                     | 29.6 ms: 1.43x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.04 ms: 1.42x faster                                                       |
| raytrace                 | 273 ms                                                      | 194 ms: 1.41x faster                                                        |
| chaos                    | 61.7 ms                                                     | 44.8 ms: 1.38x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 467 ms: 1.37x faster                                                        |
| go                       | 139 ms                                                      | 105 ms: 1.32x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 48.6 ms: 1.29x faster                                                       |
| pycparser                | 930 ms                                                      | 737 ms: 1.26x faster                                                        |
| tornado_http             | 108 ms                                                      | 86.1 ms: 1.26x faster                                                       |
| mypy2                    | 555 ms                                                      | 442 ms: 1.26x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 23.1 us: 1.25x faster                                                       |
| comprehensions           | 16.5 us                                                     | 13.3 us: 1.24x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.71 sec: 1.23x faster                                                      |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                       |
| scimark_sor              | 106 ms                                                      | 86.7 ms: 1.23x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.74 ms: 1.22x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.7 ms: 1.18x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.63 sec: 1.17x faster                                                      |
| sympy_sum                | 107 ms                                                      | 91.2 ms: 1.17x faster                                                       |
| mako                     | 9.03 ms                                                     | 7.70 ms: 1.17x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.54 sec: 1.16x faster                                                      |
| dulwich_log              | 50.5 ms                                                     | 43.7 ms: 1.16x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 179 ms: 1.15x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 836 us: 1.15x faster                                                        |
| regex_dna                | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| deepcopy                 | 255 us                                                      | 226 us: 1.13x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.96 us: 1.13x faster                                                       |
| pyflate                  | 409 ms                                                      | 363 ms: 1.13x faster                                                        |
| sympy_str                | 194 ms                                                      | 173 ms: 1.12x faster                                                        |
| sqlite_synth             | 1.91 us                                                     | 1.71 us: 1.12x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 164 us: 1.11x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 36.0 ms: 1.10x faster                                                       |
| 2to3                     | 246 ms                                                      | 224 ms: 1.10x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.53 sec: 1.09x faster                                                      |
| sympy_expand             | 314 ms                                                      | 291 ms: 1.08x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 79.7 ms: 1.08x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 747 us: 1.07x faster                                                        |
| json                     | 3.14 ms                                                     | 2.93 ms: 1.07x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.49 us: 1.07x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.15 sec: 1.06x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 557 ms: 1.06x faster                                                        |
| regex_compile            | 106 ms                                                      | 99.9 ms: 1.06x faster                                                       |
| hexiom                   | 5.74 ms                                                     | 5.44 ms: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 54.4 ms: 1.05x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.8 ms: 1.05x faster                                                       |
| python_startup           | 20.6 ms                                                     | 19.9 ms: 1.03x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| float                    | 61.7 ms                                                     | 59.9 ms: 1.03x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.69 us: 1.01x faster                                                       |
| pidigits                 | 149 ms                                                      | 148 ms: 1.01x faster                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 55.8 ms: 1.01x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 66.9 ms: 1.03x slower                                                       |
| nqueens                  | 66.6 ms                                                     | 68.9 ms: 1.03x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 41.1 ns: 1.04x slower                                                       |
| meteor_contest           | 75.9 ms                                                     | 78.9 ms: 1.04x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 65.5 ms: 1.06x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.24 us: 1.06x slower                                                       |
| fannkuch                 | 256 ms                                                      | 271 ms: 1.06x slower                                                        |
| spectral_norm            | 77.3 ms                                                     | 82.9 ms: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| async_generators         | 222 ms                                                      | 240 ms: 1.08x slower                                                        |
| scimark_fft              | 187 ms                                                      | 209 ms: 1.11x slower                                                        |
| nbody                    | 71.3 ms                                                     | 80.1 ms: 1.12x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 17.7 ms: 1.14x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.14 us: 1.14x slower                                                       |
| dask                     | 313 ms                                                      | 361 ms: 1.16x slower                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.21 ms: 1.18x slower                                                       |
| coverage                 | 39.0 ms                                                     | 46.6 ms: 1.20x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.83 ms: 1.23x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.15x faster                                                                |

Benchmark hidden because not significant (3): unpickle_list, logging_simple, pathlib
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown