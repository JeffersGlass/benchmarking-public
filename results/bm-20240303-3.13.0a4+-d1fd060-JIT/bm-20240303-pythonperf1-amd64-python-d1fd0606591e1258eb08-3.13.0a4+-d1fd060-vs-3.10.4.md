# Results vs. 3.10.4

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 226 ms: 1.09x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.77 ms: 1.21x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                      |
| tornado_http   | 108 ms                                                      | 85.2 ms: 1.27x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 725 ms: 1.53x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 450 ms: 1.42x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.53x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 49.5 ms: 1.25x faster                                                       |
| nbody          | 71.3 ms                                                     | 60.2 ms: 1.19x faster                                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 116 ms: 1.18x faster                                                        |
| regex_compile  | 106 ms                                                      | 90.7 ms: 1.17x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.55 ms: 1.07x faster                                                       |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.56 ms: 1.65x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 176 us: 1.53x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 139 us: 1.32x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.29 sec: 1.30x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.9 ms: 1.21x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.46 us: 1.07x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 93.6 ms: 1.03x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 54.3 ms: 1.02x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.8 ms: 1.02x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.9 us: 1.01x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 17.6 us: 1.02x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.94 us: 1.07x slower                                                       |
| pickle               | 6.85 us                                                     | 7.33 us: 1.07x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.12x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 24.3 ms: 1.18x slower                                                       |
| python_startup_no_site | 15.5 ms                                                     | 22.2 ms: 1.43x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.30x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.12 ms: 1.48x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.9 us: 4.74x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.06 ms: 2.03x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.4 ns: 1.71x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.56 ms: 1.65x faster                                                       |
| async_tree_none          | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 475 ms: 1.54x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 176 us: 1.53x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 725 ms: 1.53x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 796 us: 1.53x faster                                                        |
| richards_super           | 52.2 ms                                                     | 34.2 ms: 1.53x faster                                                       |
| generators               | 32.4 ms                                                     | 21.3 ms: 1.52x faster                                                       |
| raytrace                 | 273 ms                                                      | 182 ms: 1.50x faster                                                        |
| chaos                    | 61.7 ms                                                     | 41.3 ms: 1.50x faster                                                       |
| comprehensions           | 16.5 us                                                     | 11.0 us: 1.50x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.12 ms: 1.48x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.02 ms: 1.45x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 450 ms: 1.42x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 44.5 ms: 1.40x faster                                                       |
| go                       | 139 ms                                                      | 99.5 ms: 1.40x faster                                                       |
| richards                 | 42.4 ms                                                     | 30.8 ms: 1.38x faster                                                       |
| pycparser                | 930 ms                                                      | 681 ms: 1.37x faster                                                        |
| pyflate                  | 409 ms                                                      | 301 ms: 1.36x faster                                                        |
| spectral_norm            | 77.3 ms                                                     | 57.0 ms: 1.36x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 139 us: 1.32x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 22.1 us: 1.30x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.29 sec: 1.30x faster                                                      |
| tornado_http             | 108 ms                                                      | 85.2 ms: 1.27x faster                                                       |
| mypy2                    | 555 ms                                                      | 441 ms: 1.26x faster                                                        |
| float                    | 61.7 ms                                                     | 49.5 ms: 1.25x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.70 sec: 1.24x faster                                                      |
| dulwich_log              | 50.5 ms                                                     | 40.8 ms: 1.24x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 46.6 ms: 1.23x faster                                                       |
| sympy_sum                | 107 ms                                                      | 87.9 ms: 1.22x faster                                                       |
| scimark_sor              | 106 ms                                                      | 87.3 ms: 1.22x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.77 ms: 1.21x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 36.9 ms: 1.21x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.48 sec: 1.20x faster                                                      |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.29 ms: 1.19x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                      |
| nbody                    | 71.3 ms                                                     | 60.2 ms: 1.19x faster                                                       |
| regex_dna                | 136 ms                                                      | 116 ms: 1.18x faster                                                        |
| regex_compile            | 106 ms                                                      | 90.7 ms: 1.17x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 176 ms: 1.17x faster                                                        |
| sympy_str                | 194 ms                                                      | 166 ms: 1.17x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 74.0 ms: 1.16x faster                                                       |
| deepcopy                 | 255 us                                                      | 222 us: 1.15x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 836 us: 1.15x faster                                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.4 ms: 1.14x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 518 ms: 1.14x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.07 sec: 1.14x faster                                                      |
| deepcopy_reduce          | 2.20 us                                                     | 1.94 us: 1.14x faster                                                       |
| hexiom                   | 5.74 ms                                                     | 5.04 ms: 1.14x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 35.0 ms: 1.14x faster                                                       |
| sympy_expand             | 314 ms                                                      | 287 ms: 1.10x faster                                                        |
| 2to3                     | 246 ms                                                      | 226 ms: 1.09x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 740 us: 1.08x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.46 us: 1.07x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.55 ms: 1.07x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.37 us: 1.06x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.90 us: 1.05x faster                                                       |
| json                     | 3.14 ms                                                     | 3.00 ms: 1.04x faster                                                       |
| scimark_fft              | 187 ms                                                      | 180 ms: 1.04x faster                                                        |
| xml_etree_parse          | 96.8 ms                                                     | 93.6 ms: 1.03x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 73.4 ms: 1.03x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 54.3 ms: 1.02x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 65.3 ms: 1.02x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.8 ms: 1.02x faster                                                       |
| pathlib                  | 75.7 ms                                                     | 75.2 ms: 1.01x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.9 us: 1.01x faster                                                       |
| fannkuch                 | 256 ms                                                      | 261 ms: 1.02x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 17.6 us: 1.02x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.50 ms: 1.06x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.94 us: 1.07x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.33 us: 1.07x slower                                                       |
| async_generators         | 222 ms                                                      | 247 ms: 1.12x slower                                                        |
| dask                     | 313 ms                                                      | 360 ms: 1.15x slower                                                        |
| coverage                 | 39.0 ms                                                     | 45.7 ms: 1.17x slower                                                       |
| python_startup           | 20.6 ms                                                     | 24.3 ms: 1.18x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 73.4 ms: 1.18x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.70 ms: 1.19x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 22.2 ms: 1.43x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 57.1 ns: 1.44x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                                |

Benchmark hidden because not significant (3): regex_v8, pidigits, unpickle_list
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: unknown