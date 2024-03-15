# Results vs. 3.12.0

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.70%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 224 ms: 1.03x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.74 ms: 1.05x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.63 sec: 1.02x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 86.1 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 479 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 467 ms: 1.05x faster                                                        |
| async_tree_none            | 291 ms                                                      | 280 ms: 1.04x faster                                                        |
| async_tree_io              | 731 ms                                                      | 751 ms: 1.03x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 353 ms: 1.04x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_none_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                                        |
| float          | 56.8 ms                                                     | 59.9 ms: 1.05x slower                                                       |
| nbody          | 71.9 ms                                                     | 80.1 ms: 1.11x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| regex_compile  | 87.5 ms                                                     | 99.9 ms: 1.14x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 179 us: 1.09x faster                                                        |
| pickle               | 7.43 us                                                     | 7.24 us: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.70 us: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 93.8 ms: 1.01x slower                                                       |
| pickle_dict          | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 66.9 ms: 1.03x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.49 us: 1.04x slower                                                       |
| pickle_list          | 2.83 us                                                     | 3.14 us: 1.11x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.53 sec: 1.12x slower                                                      |
| unpickle_pure_python | 133 us                                                      | 164 us: 1.24x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.03x slower                                                                |

Benchmark hidden because not significant (2): xml_etree_generate, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 19.9 ms: 1.02x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 17.7 ms: 1.09x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.70 ms: 1.09x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 76.3 us: 1.25x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.71 sec: 1.22x faster                                                      |
| mypy2                      | 509 ms                                                      | 442 ms: 1.15x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 179 us: 1.09x faster                                                        |
| generators                 | 22.5 ms                                                     | 20.7 ms: 1.09x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 55.9 ns: 1.08x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.96 us: 1.07x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 75.9 ms: 1.06x faster                                                       |
| comprehensions             | 14.1 us                                                     | 13.3 us: 1.06x faster                                                       |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 65.5 ms: 1.06x faster                                                       |
| deepcopy                   | 238 us                                                      | 226 us: 1.05x faster                                                        |
| chameleon                  | 4.98 ms                                                     | 4.74 ms: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 479 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 467 ms: 1.05x faster                                                        |
| sqlglot_normalize          | 187 ms                                                      | 179 ms: 1.05x faster                                                        |
| async_tree_none            | 291 ms                                                      | 280 ms: 1.04x faster                                                        |
| json                       | 3.05 ms                                                     | 2.93 ms: 1.04x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 86.1 ms: 1.04x faster                                                       |
| pidigits                   | 152 ms                                                      | 148 ms: 1.03x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.71 us: 1.03x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 23.1 us: 1.03x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.24 us: 1.03x faster                                                       |
| bench_thread_pool          | 857 us                                                      | 836 us: 1.02x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| unpickle_list              | 2.75 us                                                     | 2.70 us: 1.02x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.63 sec: 1.02x faster                                                      |
| dulwich_log                | 44.3 ms                                                     | 43.7 ms: 1.01x faster                                                       |
| sympy_str                  | 175 ms                                                      | 173 ms: 1.01x faster                                                        |
| logging_simple             | 6.28 us                                                     | 6.23 us: 1.01x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.69 us: 1.00x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 48.6 ms: 1.00x slower                                                       |
| async_generators           | 239 ms                                                      | 240 ms: 1.00x slower                                                        |
| xml_etree_parse            | 93.0 ms                                                     | 93.8 ms: 1.01x slower                                                       |
| pickle_dict                | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| raytrace                   | 192 ms                                                      | 194 ms: 1.01x slower                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 1.04 ms: 1.02x slower                                                       |
| sqlglot_parse              | 804 us                                                      | 819 us: 1.02x slower                                                        |
| python_startup             | 19.5 ms                                                     | 19.9 ms: 1.02x slower                                                       |
| sympy_expand               | 284 ms                                                      | 291 ms: 1.02x slower                                                        |
| 2to3                       | 218 ms                                                      | 224 ms: 1.03x slower                                                        |
| async_tree_io              | 731 ms                                                      | 751 ms: 1.03x slower                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 66.9 ms: 1.03x slower                                                       |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                       |
| chaos                      | 43.3 ms                                                     | 44.8 ms: 1.03x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.49 us: 1.04x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 353 ms: 1.04x slower                                                        |
| richards                   | 28.4 ms                                                     | 29.6 ms: 1.04x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 36.0 ms: 1.04x slower                                                       |
| richards_super             | 32.1 ms                                                     | 33.8 ms: 1.05x slower                                                       |
| float                      | 56.8 ms                                                     | 59.9 ms: 1.05x slower                                                       |
| pycparser                  | 699 ms                                                      | 737 ms: 1.06x slower                                                        |
| meteor_contest             | 74.6 ms                                                     | 78.9 ms: 1.06x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.30 ms: 1.06x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 557 ms: 1.09x slower                                                        |
| mako                       | 7.09 ms                                                     | 7.70 ms: 1.09x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 17.7 ms: 1.09x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.15 sec: 1.10x slower                                                      |
| unpack_sequence            | 37.5 ns                                                     | 41.1 ns: 1.10x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 68.9 ms: 1.10x slower                                                       |
| fannkuch                   | 247 ms                                                      | 271 ms: 1.10x slower                                                        |
| scimark_sor                | 78.8 ms                                                     | 86.7 ms: 1.10x slower                                                       |
| pickle_list                | 2.83 us                                                     | 3.14 us: 1.11x slower                                                       |
| nbody                      | 71.9 ms                                                     | 80.1 ms: 1.11x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.54 sec: 1.12x slower                                                      |
| tomli_loads                | 1.37 sec                                                    | 1.53 sec: 1.12x slower                                                      |
| scimark_fft                | 184 ms                                                      | 209 ms: 1.13x slower                                                        |
| regex_compile              | 87.5 ms                                                     | 99.9 ms: 1.14x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.6 ms: 1.14x slower                                                       |
| go                         | 91.6 ms                                                     | 105 ms: 1.15x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.83 ms: 1.17x slower                                                       |
| pyflate                    | 295 ms                                                      | 363 ms: 1.23x slower                                                        |
| unpickle_pure_python       | 133 us                                                      | 164 us: 1.24x slower                                                        |
| spectral_norm              | 66.9 ms                                                     | 82.9 ms: 1.24x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 54.4 ms: 1.24x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.21 ms: 1.26x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.44 ms: 1.33x slower                                                       |
| scimark_lu                 | 58.9 ms                                                     | 79.7 ms: 1.35x slower                                                       |
| dask                       | 263 ms                                                      | 361 ms: 1.38x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.03x slower                                                                |

Benchmark hidden because not significant (9): async_tree_memoization_tg, asyncio_tcp, create_gc_cycles, gc_traversal, sympy_sum, xml_etree_generate, xml_etree_process, async_tree_none_tg, async_tree_io_tg
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.70% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown