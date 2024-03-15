# Results vs. base

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 213 ms                                                                                                                 | 224 ms: 1.05x slower                                                                                                               |
| chameleon      | 4.79 ms                                                                                                                | 4.74 ms: 1.01x faster                                                                                                              |
| docutils       | 1.55 sec                                                                                                               | 1.63 sec: 1.06x slower                                                                                                             |
| tornado_http   | 83.4 ms                                                                                                                | 86.1 ms: 1.03x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.03x slower                                                                                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 469 ms                                                                                                                 | 479 ms: 1.02x slower                                                                                                               |
| async_tree_io_tg           | 760 ms                                                                                                                 | 777 ms: 1.02x slower                                                                                                               |
| async_tree_io              | 733 ms                                                                                                                 | 751 ms: 1.02x slower                                                                                                               |
| async_tree_memoization     | 342 ms                                                                                                                 | 353 ms: 1.03x slower                                                                                                               |
| async_tree_cpu_io_mixed    | 451 ms                                                                                                                 | 467 ms: 1.04x slower                                                                                                               |
| async_tree_memoization_tg  | 348 ms                                                                                                                 | 361 ms: 1.04x slower                                                                                                               |
| async_tree_none            | 268 ms                                                                                                                 | 280 ms: 1.04x slower                                                                                                               |
| async_tree_none_tg         | 273 ms                                                                                                                 | 285 ms: 1.04x slower                                                                                                               |
| Geometric mean             | (ref)                                                                                                                  | 1.03x slower                                                                                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 147 ms                                                                                                                 | 148 ms: 1.01x slower                                                                                                               |
| float          | 52.9 ms                                                                                                                | 59.9 ms: 1.13x slower                                                                                                              |
| nbody          | 69.7 ms                                                                                                                | 80.1 ms: 1.15x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.09x slower                                                                                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| regex_v8       | 15.3 ms                                                                                                                | 14.8 ms: 1.04x faster                                                                                                              |
| regex_effbot   | 1.59 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                              |
| regex_dna      | 121 ms                                                                                                                 | 119 ms: 1.01x faster                                                                                                               |
| regex_compile  | 77.5 ms                                                                                                                | 99.9 ms: 1.29x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.05x slower                                                                                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pickle_pure_python   | 181 us                                                                                                                 | 179 us: 1.01x faster                                                                                                               |
| json_loads           | 13.7 us                                                                                                                | 13.6 us: 1.01x faster                                                                                                              |
| pickle_dict          | 18.4 us                                                                                                                | 18.6 us: 1.01x slower                                                                                                              |
| json_dumps           | 5.58 ms                                                                                                                | 5.66 ms: 1.01x slower                                                                                                              |
| pickle               | 7.14 us                                                                                                                | 7.24 us: 1.01x slower                                                                                                              |
| unpickle             | 8.28 us                                                                                                                | 8.49 us: 1.03x slower                                                                                                              |
| xml_etree_process    | 36.0 ms                                                                                                                | 37.7 ms: 1.05x slower                                                                                                              |
| xml_etree_iterparse  | 63.6 ms                                                                                                                | 66.9 ms: 1.05x slower                                                                                                              |
| pickle_list          | 2.97 us                                                                                                                | 3.14 us: 1.06x slower                                                                                                              |
| tomli_loads          | 1.44 sec                                                                                                               | 1.53 sec: 1.07x slower                                                                                                             |
| xml_etree_generate   | 52.2 ms                                                                                                                | 55.8 ms: 1.07x slower                                                                                                              |
| unpickle_pure_python | 127 us                                                                                                                 | 164 us: 1.29x slower                                                                                                               |
| Geometric mean       | (ref)                                                                                                                  | 1.04x slower                                                                                                                       |

Benchmark hidden because not significant (2): unpickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup_no_site, python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.48 ms                                                                                                                | 7.70 ms: 1.19x slower                                                                                                              |

All benchmarks:
===============

| Benchmark                  | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-PYTHON_UOPS/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| json                       | 3.28 ms                                                                                                                | 2.93 ms: 1.12x faster                                                                                                              |
| regex_v8                   | 15.3 ms                                                                                                                | 14.8 ms: 1.04x faster                                                                                                              |
| generators                 | 21.2 ms                                                                                                                | 20.7 ms: 1.03x faster                                                                                                              |
| deepcopy_reduce            | 2.00 us                                                                                                                | 1.96 us: 1.02x faster                                                                                                              |
| regex_effbot               | 1.59 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                              |
| regex_dna                  | 121 ms                                                                                                                 | 119 ms: 1.01x faster                                                                                                               |
| pickle_pure_python         | 181 us                                                                                                                 | 179 us: 1.01x faster                                                                                                               |
| chameleon                  | 4.79 ms                                                                                                                | 4.74 ms: 1.01x faster                                                                                                              |
| coverage                   | 47.0 ms                                                                                                                | 46.6 ms: 1.01x faster                                                                                                              |
| json_loads                 | 13.7 us                                                                                                                | 13.6 us: 1.01x faster                                                                                                              |
| pidigits                   | 147 ms                                                                                                                 | 148 ms: 1.01x slower                                                                                                               |
| pathlib                    | 75.2 ms                                                                                                                | 75.9 ms: 1.01x slower                                                                                                              |
| pickle_dict                | 18.4 us                                                                                                                | 18.6 us: 1.01x slower                                                                                                              |
| json_dumps                 | 5.58 ms                                                                                                                | 5.66 ms: 1.01x slower                                                                                                              |
| pickle                     | 7.14 us                                                                                                                | 7.24 us: 1.01x slower                                                                                                              |
| create_gc_cycles           | 735 us                                                                                                                 | 747 us: 1.02x slower                                                                                                               |
| async_tree_cpu_io_mixed_tg | 469 ms                                                                                                                 | 479 ms: 1.02x slower                                                                                                               |
| bench_mp_pool              | 64.1 ms                                                                                                                | 65.5 ms: 1.02x slower                                                                                                              |
| async_tree_io_tg           | 760 ms                                                                                                                 | 777 ms: 1.02x slower                                                                                                               |
| async_tree_io              | 733 ms                                                                                                                 | 751 ms: 1.02x slower                                                                                                               |
| unpickle                   | 8.28 us                                                                                                                | 8.49 us: 1.03x slower                                                                                                              |
| deepcopy_memo              | 22.4 us                                                                                                                | 23.1 us: 1.03x slower                                                                                                              |
| tornado_http               | 83.4 ms                                                                                                                | 86.1 ms: 1.03x slower                                                                                                              |
| async_tree_memoization     | 342 ms                                                                                                                 | 353 ms: 1.03x slower                                                                                                               |
| async_tree_cpu_io_mixed    | 451 ms                                                                                                                 | 467 ms: 1.04x slower                                                                                                               |
| async_tree_memoization_tg  | 348 ms                                                                                                                 | 361 ms: 1.04x slower                                                                                                               |
| async_tree_none            | 268 ms                                                                                                                 | 280 ms: 1.04x slower                                                                                                               |
| async_tree_none_tg         | 273 ms                                                                                                                 | 285 ms: 1.04x slower                                                                                                               |
| unpack_sequence            | 39.3 ns                                                                                                                | 41.1 ns: 1.04x slower                                                                                                              |
| logging_format             | 6.40 us                                                                                                                | 6.69 us: 1.04x slower                                                                                                              |
| xml_etree_process          | 36.0 ms                                                                                                                | 37.7 ms: 1.05x slower                                                                                                              |
| logging_simple             | 5.95 us                                                                                                                | 6.23 us: 1.05x slower                                                                                                              |
| 2to3                       | 213 ms                                                                                                                 | 224 ms: 1.05x slower                                                                                                               |
| typing_runtime_protocols   | 72.7 us                                                                                                                | 76.3 us: 1.05x slower                                                                                                              |
| async_generators           | 228 ms                                                                                                                 | 240 ms: 1.05x slower                                                                                                               |
| xml_etree_iterparse        | 63.6 ms                                                                                                                | 66.9 ms: 1.05x slower                                                                                                              |
| pickle_list                | 2.97 us                                                                                                                | 3.14 us: 1.06x slower                                                                                                              |
| docutils                   | 1.55 sec                                                                                                               | 1.63 sec: 1.06x slower                                                                                                             |
| tomli_loads                | 1.44 sec                                                                                                               | 1.53 sec: 1.07x slower                                                                                                             |
| sqlglot_optimize           | 33.7 ms                                                                                                                | 36.0 ms: 1.07x slower                                                                                                              |
| mypy2                      | 413 ms                                                                                                                 | 442 ms: 1.07x slower                                                                                                               |
| xml_etree_generate         | 52.2 ms                                                                                                                | 55.8 ms: 1.07x slower                                                                                                              |
| sqlglot_transpile          | 967 us                                                                                                                 | 1.04 ms: 1.07x slower                                                                                                              |
| meteor_contest             | 73.1 ms                                                                                                                | 78.9 ms: 1.08x slower                                                                                                              |
| sqlglot_parse              | 749 us                                                                                                                 | 819 us: 1.09x slower                                                                                                               |
| sqlite_synth               | 1.56 us                                                                                                                | 1.71 us: 1.10x slower                                                                                                              |
| dulwich_log                | 39.9 ms                                                                                                                | 43.7 ms: 1.10x slower                                                                                                              |
| richards                   | 27.0 ms                                                                                                                | 29.6 ms: 1.10x slower                                                                                                              |
| sympy_integrate            | 12.1 ms                                                                                                                | 13.3 ms: 1.10x slower                                                                                                              |
| mdp                        | 1.39 sec                                                                                                               | 1.54 sec: 1.10x slower                                                                                                             |
| sympy_expand               | 262 ms                                                                                                                 | 291 ms: 1.11x slower                                                                                                               |
| richards_super             | 30.3 ms                                                                                                                | 33.8 ms: 1.11x slower                                                                                                              |
| pprint_safe_repr           | 499 ms                                                                                                                 | 557 ms: 1.12x slower                                                                                                               |
| sympy_str                  | 155 ms                                                                                                                 | 173 ms: 1.12x slower                                                                                                               |
| pprint_pformat             | 1.02 sec                                                                                                               | 1.15 sec: 1.12x slower                                                                                                             |
| sympy_sum                  | 81.1 ms                                                                                                                | 91.2 ms: 1.12x slower                                                                                                              |
| fannkuch                   | 241 ms                                                                                                                 | 271 ms: 1.13x slower                                                                                                               |
| scimark_sor                | 76.6 ms                                                                                                                | 86.7 ms: 1.13x slower                                                                                                              |
| float                      | 52.9 ms                                                                                                                | 59.9 ms: 1.13x slower                                                                                                              |
| deltablue                  | 2.02 ms                                                                                                                | 2.30 ms: 1.14x slower                                                                                                              |
| chaos                      | 39.1 ms                                                                                                                | 44.8 ms: 1.15x slower                                                                                                              |
| nbody                      | 69.7 ms                                                                                                                | 80.1 ms: 1.15x slower                                                                                                              |
| crypto_pyaes               | 41.8 ms                                                                                                                | 48.6 ms: 1.16x slower                                                                                                              |
| scimark_fft                | 177 ms                                                                                                                 | 209 ms: 1.18x slower                                                                                                               |
| raytrace                   | 164 ms                                                                                                                 | 194 ms: 1.19x slower                                                                                                               |
| mako                       | 6.48 ms                                                                                                                | 7.70 ms: 1.19x slower                                                                                                              |
| nqueens                    | 57.1 ms                                                                                                                | 68.9 ms: 1.21x slower                                                                                                              |
| go                         | 84.7 ms                                                                                                                | 105 ms: 1.24x slower                                                                                                               |
| comprehensions             | 10.7 us                                                                                                                | 13.3 us: 1.24x slower                                                                                                              |
| pyflate                    | 290 ms                                                                                                                 | 363 ms: 1.25x slower                                                                                                               |
| regex_compile              | 77.5 ms                                                                                                                | 99.9 ms: 1.29x slower                                                                                                              |
| unpickle_pure_python       | 127 us                                                                                                                 | 164 us: 1.29x slower                                                                                                               |
| scimark_sparse_mat_mult    | 2.41 ms                                                                                                                | 3.21 ms: 1.33x slower                                                                                                              |
| spectral_norm              | 60.8 ms                                                                                                                | 82.9 ms: 1.36x slower                                                                                                              |
| scimark_monte_carlo        | 39.6 ms                                                                                                                | 54.4 ms: 1.37x slower                                                                                                              |
| hexiom                     | 3.76 ms                                                                                                                | 5.44 ms: 1.45x slower                                                                                                              |
| scimark_lu                 | 52.5 ms                                                                                                                | 79.7 ms: 1.52x slower                                                                                                              |
| Geometric mean             | (ref)                                                                                                                  | 1.08x slower                                                                                                                       |

Benchmark hidden because not significant (15): asyncio_tcp_ssl, python_startup_no_site, telco, logging_silent, unpickle_list, python_startup, deepcopy, sqlglot_normalize, gc_traversal, coroutines, xml_etree_parse, dask, bench_thread_pool, asyncio_tcp, pycparser


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: unknown