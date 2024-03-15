# Results vs. 3.12.0

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 213 ms: 1.02x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.79 ms: 1.04x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.55 sec: 1.07x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 83.4 ms: 1.07x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 451 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 469 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 348 ms: 1.05x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 760 ms: 1.01x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 52.9 ms: 1.07x faster                                                       |
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| nbody          | 71.9 ms                                                     | 69.7 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 77.5 ms: 1.13x faster                                                       |
| regex_dna      | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 181 us: 1.08x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 52.2 ms: 1.07x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                       |
| unpickle_pure_python | 133 us                                                      | 127 us: 1.05x faster                                                        |
| pickle               | 7.43 us                                                     | 7.14 us: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.6 ms: 1.03x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.58 ms: 1.02x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.71 us: 1.01x faster                                                       |
| unpickle             | 8.18 us                                                     | 8.28 us: 1.01x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                      |
| pickle_list          | 2.83 us                                                     | 2.97 us: 1.05x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (2): pickle_dict, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.0 ms: 1.03x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 17.8 ms: 1.09x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.48 ms: 1.09x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| comprehensions             | 14.1 us                                                     | 10.7 us: 1.31x faster                                                       |
| typing_runtime_protocols   | 95.1 us                                                     | 72.7 us: 1.31x faster                                                       |
| mypy2                      | 509 ms                                                      | 413 ms: 1.23x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.76 sec: 1.19x faster                                                      |
| raytrace                   | 192 ms                                                      | 164 ms: 1.17x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 41.8 ms: 1.16x faster                                                       |
| sympy_str                  | 175 ms                                                      | 155 ms: 1.13x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 77.5 ms: 1.13x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 81.1 ms: 1.13x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 52.5 ms: 1.12x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 39.9 ms: 1.11x faster                                                       |
| chaos                      | 43.3 ms                                                     | 39.1 ms: 1.11x faster                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 39.6 ms: 1.10x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 60.8 ms: 1.10x faster                                                       |
| nqueens                    | 62.8 ms                                                     | 57.1 ms: 1.10x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.48 ms: 1.09x faster                                                       |
| hexiom                     | 4.10 ms                                                     | 3.76 ms: 1.09x faster                                                       |
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 451 ms: 1.08x faster                                                        |
| sympy_expand               | 284 ms                                                      | 262 ms: 1.08x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 181 us: 1.08x faster                                                        |
| go                         | 91.6 ms                                                     | 84.7 ms: 1.08x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 64.1 ms: 1.08x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 56.1 ns: 1.08x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.55 sec: 1.07x faster                                                      |
| sympy_integrate            | 13.0 ms                                                     | 12.1 ms: 1.07x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 749 us: 1.07x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 83.4 ms: 1.07x faster                                                       |
| float                      | 56.8 ms                                                     | 52.9 ms: 1.07x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.02 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 469 ms: 1.07x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 75.2 ms: 1.07x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 52.2 ms: 1.07x faster                                                       |
| generators                 | 22.5 ms                                                     | 21.2 ms: 1.06x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.41 ms: 1.06x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 22.4 us: 1.06x faster                                                       |
| richards_super             | 32.1 ms                                                     | 30.3 ms: 1.06x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 967 us: 1.06x faster                                                        |
| logging_simple             | 6.28 us                                                     | 5.95 us: 1.06x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 348 ms: 1.05x faster                                                        |
| richards                   | 28.4 ms                                                     | 27.0 ms: 1.05x faster                                                       |
| deepcopy                   | 238 us                                                      | 227 us: 1.05x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.40 us: 1.05x faster                                                       |
| async_generators           | 239 ms                                                      | 228 ms: 1.05x faster                                                        |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 2.00 us: 1.05x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                       |
| unpickle_pure_python       | 133 us                                                      | 127 us: 1.05x faster                                                        |
| sqlglot_normalize          | 187 ms                                                      | 179 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 273 ms: 1.04x faster                                                        |
| scimark_fft                | 184 ms                                                      | 177 ms: 1.04x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.14 us: 1.04x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.79 ms: 1.04x faster                                                       |
| pidigits                   | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| nbody                      | 71.9 ms                                                     | 69.7 ms: 1.03x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 499 ms: 1.03x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 76.6 ms: 1.03x faster                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.6 ms: 1.03x faster                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.02 sec: 1.03x faster                                                      |
| fannkuch                   | 247 ms                                                      | 241 ms: 1.03x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.7 ms: 1.02x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 735 us: 1.02x faster                                                        |
| 2to3                       | 218 ms                                                      | 213 ms: 1.02x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 73.1 ms: 1.02x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.58 ms: 1.02x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| pyflate                    | 295 ms                                                      | 290 ms: 1.02x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.71 us: 1.01x faster                                                       |
| async_tree_io_tg           | 771 ms                                                      | 760 ms: 1.01x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                                       |
| unpickle                   | 8.18 us                                                     | 8.28 us: 1.01x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.39 sec: 1.01x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.0 ms: 1.03x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 39.3 ns: 1.05x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                      |
| pickle_list                | 2.83 us                                                     | 2.97 us: 1.05x slower                                                       |
| json                       | 3.05 ms                                                     | 3.28 ms: 1.08x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 17.8 ms: 1.09x slower                                                       |
| coverage                   | 40.8 ms                                                     | 47.0 ms: 1.15x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.85 ms: 1.17x slower                                                       |
| dask                       | 263 ms                                                      | 359 ms: 1.37x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (7): bench_thread_pool, asyncio_tcp, pickle_dict, async_tree_io, xml_etree_parse, async_tree_memoization, pycparser
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown