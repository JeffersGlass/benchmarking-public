# Results vs. 3.12.0

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.01x faster \*
- HPT reliability: 97.75%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 226 ms: 1.04x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.77 ms: 1.04x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 85.2 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                        |
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.05x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 351 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 758 ms: 1.02x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 60.2 ms: 1.19x faster                                                       |
| float          | 56.8 ms                                                     | 49.5 ms: 1.15x faster                                                       |
| pidigits       | 152 ms                                                      | 150 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 116 ms: 1.09x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.55 ms: 1.04x faster                                                       |
| regex_compile  | 87.5 ms                                                     | 90.7 ms: 1.04x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 176 us: 1.11x faster                                                        |
| tomli_loads          | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 17.6 us: 1.05x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 54.3 ms: 1.03x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.56 ms: 1.02x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.9 ms: 1.02x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.8 ms: 1.02x faster                                                       |
| pickle               | 7.43 us                                                     | 7.33 us: 1.01x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.73 us: 1.01x faster                                                       |
| unpickle             | 8.18 us                                                     | 8.46 us: 1.03x slower                                                       |
| pickle_list          | 2.83 us                                                     | 2.94 us: 1.04x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 139 us: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (2): json_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 24.3 ms: 1.25x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 22.2 ms: 1.36x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.31x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.12 ms: 1.16x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.9 us: 1.34x faster                                                       |
| comprehensions             | 14.1 us                                                     | 11.0 us: 1.28x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.70 sec: 1.23x faster                                                      |
| nbody                      | 71.9 ms                                                     | 60.2 ms: 1.19x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 57.0 ms: 1.17x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.12 ms: 1.16x faster                                                       |
| mypy2                      | 509 ms                                                      | 441 ms: 1.16x faster                                                        |
| float                      | 56.8 ms                                                     | 49.5 ms: 1.15x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.29 ms: 1.12x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.11x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 176 us: 1.11x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 55.4 ns: 1.09x faster                                                       |
| regex_dna                  | 126 ms                                                      | 116 ms: 1.09x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 44.5 ms: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                        |
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 40.8 ms: 1.09x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.94 us: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                        |
| deepcopy                   | 238 us                                                      | 222 us: 1.07x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 22.1 us: 1.07x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 75.2 ms: 1.07x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 176 ms: 1.06x faster                                                        |
| logging_simple             | 6.28 us                                                     | 5.90 us: 1.06x faster                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| raytrace                   | 192 ms                                                      | 182 ms: 1.06x faster                                                        |
| generators                 | 22.5 ms                                                     | 21.3 ms: 1.06x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.37 us: 1.05x faster                                                       |
| sympy_str                  | 175 ms                                                      | 166 ms: 1.05x faster                                                        |
| chaos                      | 43.3 ms                                                     | 41.3 ms: 1.05x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 85.2 ms: 1.05x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.06 ms: 1.05x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 17.6 us: 1.05x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.05x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 351 ms: 1.04x faster                                                        |
| chameleon                  | 4.98 ms                                                     | 4.77 ms: 1.04x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.55 ms: 1.04x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 87.9 ms: 1.04x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                      |
| xml_etree_generate         | 55.8 ms                                                     | 54.3 ms: 1.03x faster                                                       |
| scimark_fft                | 184 ms                                                      | 180 ms: 1.03x faster                                                        |
| pycparser                  | 699 ms                                                      | 681 ms: 1.03x faster                                                        |
| asyncio_tcp                | 487 ms                                                      | 475 ms: 1.03x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.56 ms: 1.02x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 36.9 ms: 1.02x faster                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.8 ms: 1.02x faster                                                       |
| pidigits                   | 152 ms                                                      | 150 ms: 1.02x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 758 ms: 1.02x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 73.4 ms: 1.02x faster                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.02x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 740 us: 1.02x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.33 us: 1.01x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 796 us: 1.01x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.73 us: 1.01x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 518 ms: 1.01x slower                                                        |
| sympy_expand               | 284 ms                                                      | 287 ms: 1.01x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 35.0 ms: 1.01x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.07 sec: 1.02x slower                                                      |
| pyflate                    | 295 ms                                                      | 301 ms: 1.02x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.4 ms: 1.03x slower                                                       |
| async_generators           | 239 ms                                                      | 247 ms: 1.03x slower                                                        |
| unpickle                   | 8.18 us                                                     | 8.46 us: 1.03x slower                                                       |
| regex_compile              | 87.5 ms                                                     | 90.7 ms: 1.04x slower                                                       |
| 2to3                       | 218 ms                                                      | 226 ms: 1.04x slower                                                        |
| pickle_list                | 2.83 us                                                     | 2.94 us: 1.04x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 65.3 ms: 1.04x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 139 us: 1.04x slower                                                        |
| fannkuch                   | 247 ms                                                      | 261 ms: 1.06x slower                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 73.4 ms: 1.06x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 46.6 ms: 1.07x slower                                                       |
| richards_super             | 32.1 ms                                                     | 34.2 ms: 1.07x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.48 sec: 1.08x slower                                                      |
| richards                   | 28.4 ms                                                     | 30.8 ms: 1.09x slower                                                       |
| go                         | 91.6 ms                                                     | 99.5 ms: 1.09x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 87.3 ms: 1.11x slower                                                       |
| coverage                   | 40.8 ms                                                     | 45.7 ms: 1.12x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.70 ms: 1.14x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.04 ms: 1.23x slower                                                       |
| python_startup             | 19.5 ms                                                     | 24.3 ms: 1.25x slower                                                       |
| scimark_lu                 | 58.9 ms                                                     | 74.0 ms: 1.26x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 22.2 ms: 1.36x slower                                                       |
| dask                       | 263 ms                                                      | 360 ms: 1.37x slower                                                        |
| unpack_sequence            | 37.5 ns                                                     | 57.1 ns: 1.52x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (7): bench_thread_pool, json, async_tree_io, sqlglot_transpile, json_loads, xml_etree_parse, async_tree_memoization
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 97.75% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown