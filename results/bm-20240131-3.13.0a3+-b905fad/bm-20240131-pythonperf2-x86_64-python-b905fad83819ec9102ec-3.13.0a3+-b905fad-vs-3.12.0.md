
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.00x slower
- HPT reliability: 75.30%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 291 ms: 1.02x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.28 ms: 1.01x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.85 sec: 1.01x faster                                                       |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none    | 452 ms                                                       | 428 ms: 1.05x faster                                                         |
| async_tree_none_tg | 431 ms                                                       | 429 ms: 1.00x faster                                                         |
| async_tree_io_tg   | 1.05 sec                                                     | 1.06 sec: 1.00x slower                                                       |
| async_tree_io      | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                                       |
| Geometric mean     | (ref)                                                        | 1.01x faster                                                                 |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 85.6 ms: 1.03x faster                                                        |
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 79.6 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 139 ms: 1.03x faster                                                         |
| regex_dna      | 239 ms                                                       | 238 ms: 1.00x faster                                                         |
| regex_effbot   | 3.57 ms                                                      | 3.67 ms: 1.03x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 25.8 ms: 1.09x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|---------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict         | 32.5 us                                                      | 30.8 us: 1.06x faster                                                        |
| pickle_pure_python  | 318 us                                                       | 303 us: 1.05x faster                                                         |
| pickle              | 10.5 us                                                      | 10.1 us: 1.04x faster                                                        |
| xml_etree_generate  | 86.1 ms                                                      | 84.4 ms: 1.02x faster                                                        |
| xml_etree_process   | 58.4 ms                                                      | 58.8 ms: 1.01x slower                                                        |
| json_loads          | 24.4 us                                                      | 24.9 us: 1.02x slower                                                        |
| json_dumps          | 10.2 ms                                                      | 10.5 ms: 1.03x slower                                                        |
| xml_etree_parse     | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| tomli_loads         | 2.16 sec                                                     | 2.23 sec: 1.04x slower                                                       |
| unpickle            | 14.8 us                                                      | 15.4 us: 1.04x slower                                                        |
| unpickle_list       | 4.66 us                                                      | 4.89 us: 1.05x slower                                                        |
| xml_etree_iterparse | 103 ms                                                       | 109 ms: 1.06x slower                                                         |
| Geometric mean      | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): unpickle_pure_python, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| comprehensions           | 21.9 us                                                      | 16.4 us: 1.33x faster                                                        |
| typing_runtime_protocols | 152 us                                                       | 117 us: 1.30x faster                                                         |
| raytrace                 | 298 ms                                                       | 258 ms: 1.15x faster                                                         |
| crypto_pyaes             | 80.3 ms                                                      | 69.8 ms: 1.15x faster                                                        |
| generators               | 37.4 ms                                                      | 33.8 ms: 1.11x faster                                                        |
| unpack_sequence          | 53.2 ns                                                      | 48.8 ns: 1.09x faster                                                        |
| async_generators         | 390 ms                                                       | 360 ms: 1.09x faster                                                         |
| chaos                    | 64.0 ms                                                      | 59.0 ms: 1.08x faster                                                        |
| sympy_sum                | 162 ms                                                       | 151 ms: 1.07x faster                                                         |
| pickle_dict              | 32.5 us                                                      | 30.8 us: 1.06x faster                                                        |
| coroutines               | 23.0 ms                                                      | 21.8 ms: 1.05x faster                                                        |
| async_tree_none          | 452 ms                                                       | 428 ms: 1.05x faster                                                         |
| scimark_monte_carlo      | 69.0 ms                                                      | 65.6 ms: 1.05x faster                                                        |
| pickle_pure_python       | 318 us                                                       | 303 us: 1.05x faster                                                         |
| sympy_str                | 302 ms                                                       | 289 ms: 1.05x faster                                                         |
| bench_mp_pool            | 4.76 ms                                                      | 4.56 ms: 1.05x faster                                                        |
| pickle                   | 10.5 us                                                      | 10.1 us: 1.04x faster                                                        |
| logging_format           | 7.48 us                                                      | 7.23 us: 1.03x faster                                                        |
| sympy_integrate          | 23.9 ms                                                      | 23.2 ms: 1.03x faster                                                        |
| regex_compile            | 144 ms                                                       | 139 ms: 1.03x faster                                                         |
| asyncio_tcp              | 378 ms                                                       | 366 ms: 1.03x faster                                                         |
| mdp                      | 2.57 sec                                                     | 2.49 sec: 1.03x faster                                                       |
| nbody                    | 88.0 ms                                                      | 85.6 ms: 1.03x faster                                                        |
| nqueens                  | 89.9 ms                                                      | 87.5 ms: 1.03x faster                                                        |
| xml_etree_generate       | 86.1 ms                                                      | 84.4 ms: 1.02x faster                                                        |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.12 ms: 1.02x faster                                                        |
| sqlite_synth             | 2.77 us                                                      | 2.72 us: 1.02x faster                                                        |
| logging_simple           | 6.71 us                                                      | 6.59 us: 1.02x faster                                                        |
| deepcopy_reduce          | 3.37 us                                                      | 3.32 us: 1.02x faster                                                        |
| scimark_fft              | 301 ms                                                       | 298 ms: 1.01x faster                                                         |
| pathlib                  | 18.9 ms                                                      | 18.7 ms: 1.01x faster                                                        |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| meteor_contest           | 128 ms                                                       | 127 ms: 1.01x faster                                                         |
| pidigits                 | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| docutils                 | 2.87 sec                                                     | 2.85 sec: 1.01x faster                                                       |
| regex_dna                | 239 ms                                                       | 238 ms: 1.00x faster                                                         |
| async_tree_none_tg       | 431 ms                                                       | 429 ms: 1.00x faster                                                         |
| async_tree_io_tg         | 1.05 sec                                                     | 1.06 sec: 1.00x slower                                                       |
| chameleon                | 7.23 ms                                                      | 7.28 ms: 1.01x slower                                                        |
| xml_etree_process        | 58.4 ms                                                      | 58.8 ms: 1.01x slower                                                        |
| sqlglot_transpile        | 1.78 ms                                                      | 1.79 ms: 1.01x slower                                                        |
| json                     | 5.12 ms                                                      | 5.16 ms: 1.01x slower                                                        |
| gc_traversal             | 3.48 ms                                                      | 3.51 ms: 1.01x slower                                                        |
| spectral_norm            | 91.6 ms                                                      | 92.6 ms: 1.01x slower                                                        |
| dask                     | 392 ms                                                       | 397 ms: 1.01x slower                                                         |
| deepcopy_memo            | 36.8 us                                                      | 37.2 us: 1.01x slower                                                        |
| sqlglot_optimize         | 57.5 ms                                                      | 58.4 ms: 1.02x slower                                                        |
| async_tree_io            | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                                       |
| 2to3                     | 285 ms                                                       | 291 ms: 1.02x slower                                                         |
| sympy_expand             | 484 ms                                                       | 494 ms: 1.02x slower                                                         |
| json_loads               | 24.4 us                                                      | 24.9 us: 1.02x slower                                                        |
| pycparser                | 1.23 sec                                                     | 1.26 sec: 1.02x slower                                                       |
| json_dumps               | 10.2 ms                                                      | 10.5 ms: 1.03x slower                                                        |
| bench_thread_pool        | 950 us                                                       | 975 us: 1.03x slower                                                         |
| dulwich_log              | 65.4 ms                                                      | 67.2 ms: 1.03x slower                                                        |
| regex_effbot             | 3.57 ms                                                      | 3.67 ms: 1.03x slower                                                        |
| xml_etree_parse          | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| tomli_loads              | 2.16 sec                                                     | 2.23 sec: 1.04x slower                                                       |
| unpickle                 | 14.8 us                                                      | 15.4 us: 1.04x slower                                                        |
| float                    | 76.6 ms                                                      | 79.6 ms: 1.04x slower                                                        |
| mako                     | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                        |
| unpickle_list            | 4.66 us                                                      | 4.89 us: 1.05x slower                                                        |
| hexiom                   | 5.96 ms                                                      | 6.31 ms: 1.06x slower                                                        |
| xml_etree_iterparse      | 103 ms                                                       | 109 ms: 1.06x slower                                                         |
| python_startup           | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| regex_v8                 | 23.6 ms                                                      | 25.8 ms: 1.09x slower                                                        |
| fannkuch                 | 350 ms                                                       | 385 ms: 1.10x slower                                                         |
| deltablue                | 3.24 ms                                                      | 3.58 ms: 1.11x slower                                                        |
| go                       | 150 ms                                                       | 166 ms: 1.11x slower                                                         |
| richards_super           | 51.3 ms                                                      | 57.6 ms: 1.12x slower                                                        |
| richards                 | 45.7 ms                                                      | 51.6 ms: 1.13x slower                                                        |
| pyflate                  | 439 ms                                                       | 502 ms: 1.14x slower                                                         |
| telco                    | 6.96 ms                                                      | 8.02 ms: 1.15x slower                                                        |
| coverage                 | 66.7 ms                                                      | 78.7 ms: 1.18x slower                                                        |
| python_startup_no_site   | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| scimark_sor              | 109 ms                                                       | 141 ms: 1.29x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (17): async_tree_memoization, async_tree_cpu_io_mixed, deepcopy, logging_silent, pprint_safe_repr, scimark_lu, unpickle_pure_python, tornado_http, async_tree_cpu_io_mixed_tg, sqlglot_normalize, pprint_pformat, sqlglot_parse, asyncio_websockets, async_tree_memoization_tg, pickle_list, create_gc_cycles, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 75.30% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.88x