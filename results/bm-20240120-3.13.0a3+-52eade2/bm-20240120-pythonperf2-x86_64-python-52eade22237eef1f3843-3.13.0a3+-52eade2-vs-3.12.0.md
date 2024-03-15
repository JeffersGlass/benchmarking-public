
# Results vs. 3.12.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: linux-x86_64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.01x slower
- HPT reliability: 62.69%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 293 ms: 1.03x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.16 ms: 1.01x faster                                                        |
| docutils       | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                                       |
| tornado_http   | 121 ms                                                       | 117 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none  | 452 ms                                                       | 432 ms: 1.05x faster                                                         |
| async_tree_io_tg | 1.05 sec                                                     | 1.07 sec: 1.01x slower                                                       |
| async_tree_io    | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| Geometric mean   | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (5): async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| float          | 76.6 ms                                                      | 79.9 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 140 ms: 1.03x faster                                                         |
| regex_dna      | 239 ms                                                       | 239 ms: 1.00x slower                                                         |
| regex_effbot   | 3.57 ms                                                      | 3.59 ms: 1.00x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 26.7 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.7 us: 1.06x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 307 us: 1.04x faster                                                         |
| xml_etree_process    | 58.4 ms                                                      | 57.3 ms: 1.02x faster                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 84.7 ms: 1.02x faster                                                        |
| pickle               | 10.5 us                                                      | 10.4 us: 1.01x faster                                                        |
| pickle_list          | 4.43 us                                                      | 4.39 us: 1.01x faster                                                        |
| unpickle_pure_python | 210 us                                                       | 211 us: 1.01x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.0 us: 1.03x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| unpickle_list        | 4.66 us                                                      | 4.88 us: 1.05x slower                                                        |
| tomli_loads          | 2.16 sec                                                     | 2.31 sec: 1.07x slower                                                       |
| xml_etree_parse      | 144 ms                                                       | 156 ms: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 152 us                                                       | 114 us: 1.33x faster                                                         |
| comprehensions           | 21.9 us                                                      | 16.5 us: 1.32x faster                                                        |
| crypto_pyaes             | 80.3 ms                                                      | 70.0 ms: 1.15x faster                                                        |
| raytrace                 | 298 ms                                                       | 263 ms: 1.13x faster                                                         |
| generators               | 37.4 ms                                                      | 33.8 ms: 1.11x faster                                                        |
| chaos                    | 64.0 ms                                                      | 58.9 ms: 1.09x faster                                                        |
| async_generators         | 390 ms                                                       | 363 ms: 1.07x faster                                                         |
| sympy_sum                | 162 ms                                                       | 152 ms: 1.06x faster                                                         |
| logging_format           | 7.48 us                                                      | 7.04 us: 1.06x faster                                                        |
| pickle_dict              | 32.5 us                                                      | 30.7 us: 1.06x faster                                                        |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.01 ms: 1.05x faster                                                        |
| async_tree_none          | 452 ms                                                       | 432 ms: 1.05x faster                                                         |
| sympy_str                | 302 ms                                                       | 290 ms: 1.04x faster                                                         |
| mdp                      | 2.57 sec                                                     | 2.47 sec: 1.04x faster                                                       |
| scimark_monte_carlo      | 69.0 ms                                                      | 66.3 ms: 1.04x faster                                                        |
| coroutines               | 23.0 ms                                                      | 22.1 ms: 1.04x faster                                                        |
| pickle_pure_python       | 318 us                                                       | 307 us: 1.04x faster                                                         |
| sympy_integrate          | 23.9 ms                                                      | 23.1 ms: 1.04x faster                                                        |
| asyncio_tcp              | 378 ms                                                       | 365 ms: 1.04x faster                                                         |
| tornado_http             | 121 ms                                                       | 117 ms: 1.03x faster                                                         |
| logging_simple           | 6.71 us                                                      | 6.50 us: 1.03x faster                                                        |
| scimark_lu               | 98.8 ms                                                      | 96.1 ms: 1.03x faster                                                        |
| regex_compile            | 144 ms                                                       | 140 ms: 1.03x faster                                                         |
| sqlite_synth             | 2.77 us                                                      | 2.70 us: 1.03x faster                                                        |
| nqueens                  | 89.9 ms                                                      | 87.6 ms: 1.03x faster                                                        |
| deepcopy_reduce          | 3.37 us                                                      | 3.30 us: 1.02x faster                                                        |
| unpack_sequence          | 53.2 ns                                                      | 52.1 ns: 1.02x faster                                                        |
| pprint_pformat           | 1.65 sec                                                     | 1.62 sec: 1.02x faster                                                       |
| xml_etree_process        | 58.4 ms                                                      | 57.3 ms: 1.02x faster                                                        |
| create_gc_cycles         | 1.59 ms                                                      | 1.56 ms: 1.02x faster                                                        |
| xml_etree_generate       | 86.1 ms                                                      | 84.7 ms: 1.02x faster                                                        |
| scimark_fft              | 301 ms                                                       | 296 ms: 1.02x faster                                                         |
| docutils                 | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                                       |
| pprint_safe_repr         | 807 ms                                                       | 796 ms: 1.01x faster                                                         |
| pickle                   | 10.5 us                                                      | 10.4 us: 1.01x faster                                                        |
| sqlglot_parse            | 1.38 ms                                                      | 1.36 ms: 1.01x faster                                                        |
| pathlib                  | 18.9 ms                                                      | 18.7 ms: 1.01x faster                                                        |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| pickle_list              | 4.43 us                                                      | 4.39 us: 1.01x faster                                                        |
| sqlglot_normalize        | 116 ms                                                       | 115 ms: 1.01x faster                                                         |
| chameleon                | 7.23 ms                                                      | 7.16 ms: 1.01x faster                                                        |
| meteor_contest           | 128 ms                                                       | 127 ms: 1.01x faster                                                         |
| sqlglot_transpile        | 1.78 ms                                                      | 1.77 ms: 1.01x faster                                                        |
| pidigits                 | 265 ms                                                       | 264 ms: 1.00x faster                                                         |
| deepcopy                 | 368 us                                                       | 367 us: 1.00x faster                                                         |
| spectral_norm            | 91.6 ms                                                      | 91.4 ms: 1.00x faster                                                        |
| regex_dna                | 239 ms                                                       | 239 ms: 1.00x slower                                                         |
| regex_effbot             | 3.57 ms                                                      | 3.59 ms: 1.00x slower                                                        |
| deepcopy_memo            | 36.8 us                                                      | 37.0 us: 1.00x slower                                                        |
| unpickle_pure_python     | 210 us                                                       | 211 us: 1.01x slower                                                         |
| dask                     | 392 ms                                                       | 396 ms: 1.01x slower                                                         |
| async_tree_io_tg         | 1.05 sec                                                     | 1.07 sec: 1.01x slower                                                       |
| sympy_expand             | 484 ms                                                       | 491 ms: 1.01x slower                                                         |
| logging_silent           | 94.4 ns                                                      | 95.8 ns: 1.02x slower                                                        |
| sqlglot_optimize         | 57.5 ms                                                      | 58.6 ms: 1.02x slower                                                        |
| json_loads               | 24.4 us                                                      | 25.0 us: 1.03x slower                                                        |
| async_tree_io            | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| 2to3                     | 285 ms                                                       | 293 ms: 1.03x slower                                                         |
| json                     | 5.12 ms                                                      | 5.30 ms: 1.04x slower                                                        |
| json_dumps               | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                        |
| mako                     | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                        |
| dulwich_log              | 65.4 ms                                                      | 67.9 ms: 1.04x slower                                                        |
| xml_etree_iterparse      | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| float                    | 76.6 ms                                                      | 79.9 ms: 1.04x slower                                                        |
| unpickle_list            | 4.66 us                                                      | 4.88 us: 1.05x slower                                                        |
| pycparser                | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                                       |
| tomli_loads              | 2.16 sec                                                     | 2.31 sec: 1.07x slower                                                       |
| hexiom                   | 5.96 ms                                                      | 6.39 ms: 1.07x slower                                                        |
| python_startup           | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| xml_etree_parse          | 144 ms                                                       | 156 ms: 1.09x slower                                                         |
| fannkuch                 | 350 ms                                                       | 382 ms: 1.09x slower                                                         |
| deltablue                | 3.24 ms                                                      | 3.53 ms: 1.09x slower                                                        |
| go                       | 150 ms                                                       | 169 ms: 1.13x slower                                                         |
| regex_v8                 | 23.6 ms                                                      | 26.7 ms: 1.13x slower                                                        |
| richards                 | 45.7 ms                                                      | 52.2 ms: 1.14x slower                                                        |
| richards_super           | 51.3 ms                                                      | 58.9 ms: 1.15x slower                                                        |
| gc_traversal             | 3.48 ms                                                      | 4.00 ms: 1.15x slower                                                        |
| telco                    | 6.96 ms                                                      | 8.05 ms: 1.16x slower                                                        |
| pyflate                  | 439 ms                                                       | 518 ms: 1.18x slower                                                         |
| coverage                 | 66.7 ms                                                      | 80.5 ms: 1.21x slower                                                        |
| python_startup_no_site   | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| scimark_sor              | 109 ms                                                       | 141 ms: 1.29x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (11): bench_mp_pool, async_tree_none_tg, unpickle, async_tree_cpu_io_mixed, asyncio_websockets, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, nbody, bench_thread_pool, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 62.69% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.88x