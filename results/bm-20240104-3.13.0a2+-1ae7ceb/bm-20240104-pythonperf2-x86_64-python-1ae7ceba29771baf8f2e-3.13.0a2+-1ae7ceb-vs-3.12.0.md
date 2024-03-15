
# Results vs. 3.12.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.01x slower
- HPT reliability: 94.64%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 292 ms: 1.02x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                                       |
| tornado_http   | 121 ms                                                       | 118 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none    | 452 ms                                                       | 431 ms: 1.05x faster                                                         |
| async_tree_none_tg | 431 ms                                                       | 427 ms: 1.01x faster                                                         |
| async_tree_io_tg   | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                                       |
| async_tree_io      | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| Geometric mean     | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 84.6 ms: 1.04x faster                                                        |
| pidigits       | 265 ms                                                       | 263 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 78.5 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 142 ms: 1.02x faster                                                         |
| regex_dna      | 239 ms                                                       | 247 ms: 1.04x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 25.4 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|---------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict         | 32.5 us                                                      | 31.4 us: 1.04x faster                                                        |
| pickle              | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| pickle_pure_python  | 318 us                                                       | 311 us: 1.02x faster                                                         |
| unpickle            | 14.8 us                                                      | 14.9 us: 1.01x slower                                                        |
| xml_etree_generate  | 86.1 ms                                                      | 87.1 ms: 1.01x slower                                                        |
| xml_etree_process   | 58.4 ms                                                      | 59.3 ms: 1.02x slower                                                        |
| json_loads          | 24.4 us                                                      | 24.8 us: 1.02x slower                                                        |
| tomli_loads         | 2.16 sec                                                     | 2.22 sec: 1.03x slower                                                       |
| xml_etree_parse     | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| json_dumps          | 10.2 ms                                                      | 10.6 ms: 1.03x slower                                                        |
| xml_etree_iterparse | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| Geometric mean      | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (3): pickle_list, unpickle_list, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.17x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| comprehensions           | 21.9 us                                                      | 16.6 us: 1.32x faster                                                        |
| typing_runtime_protocols | 152 us                                                       | 116 us: 1.30x faster                                                         |
| crypto_pyaes             | 80.3 ms                                                      | 70.0 ms: 1.15x faster                                                        |
| raytrace                 | 298 ms                                                       | 270 ms: 1.10x faster                                                         |
| generators               | 37.4 ms                                                      | 34.2 ms: 1.09x faster                                                        |
| chaos                    | 64.0 ms                                                      | 58.8 ms: 1.09x faster                                                        |
| async_generators         | 390 ms                                                       | 360 ms: 1.08x faster                                                         |
| sympy_sum                | 162 ms                                                       | 152 ms: 1.07x faster                                                         |
| bench_mp_pool            | 4.76 ms                                                      | 4.46 ms: 1.07x faster                                                        |
| async_tree_none          | 452 ms                                                       | 431 ms: 1.05x faster                                                         |
| sympy_str                | 302 ms                                                       | 290 ms: 1.04x faster                                                         |
| nbody                    | 88.0 ms                                                      | 84.6 ms: 1.04x faster                                                        |
| nqueens                  | 89.9 ms                                                      | 86.6 ms: 1.04x faster                                                        |
| pickle_dict              | 32.5 us                                                      | 31.4 us: 1.04x faster                                                        |
| asyncio_tcp              | 378 ms                                                       | 365 ms: 1.04x faster                                                         |
| sympy_integrate          | 23.9 ms                                                      | 23.1 ms: 1.03x faster                                                        |
| coroutines               | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                                        |
| scimark_lu               | 98.8 ms                                                      | 95.9 ms: 1.03x faster                                                        |
| pickle                   | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| logging_format           | 7.48 us                                                      | 7.28 us: 1.03x faster                                                        |
| sqlite_synth             | 2.77 us                                                      | 2.70 us: 1.03x faster                                                        |
| logging_simple           | 6.71 us                                                      | 6.54 us: 1.03x faster                                                        |
| tornado_http             | 121 ms                                                       | 118 ms: 1.02x faster                                                         |
| mdp                      | 2.57 sec                                                     | 2.51 sec: 1.02x faster                                                       |
| pickle_pure_python       | 318 us                                                       | 311 us: 1.02x faster                                                         |
| scimark_monte_carlo      | 69.0 ms                                                      | 67.8 ms: 1.02x faster                                                        |
| docutils                 | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                                       |
| regex_compile            | 144 ms                                                       | 142 ms: 1.02x faster                                                         |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| async_tree_none_tg       | 431 ms                                                       | 427 ms: 1.01x faster                                                         |
| pidigits                 | 265 ms                                                       | 263 ms: 1.01x faster                                                         |
| scimark_fft              | 301 ms                                                       | 299 ms: 1.01x faster                                                         |
| spectral_norm            | 91.6 ms                                                      | 91.4 ms: 1.00x faster                                                        |
| meteor_contest           | 128 ms                                                       | 128 ms: 1.00x faster                                                         |
| sqlglot_normalize        | 116 ms                                                       | 116 ms: 1.01x slower                                                         |
| unpickle                 | 14.8 us                                                      | 14.9 us: 1.01x slower                                                        |
| sqlglot_transpile        | 1.78 ms                                                      | 1.79 ms: 1.01x slower                                                        |
| sqlglot_parse            | 1.38 ms                                                      | 1.39 ms: 1.01x slower                                                        |
| pprint_pformat           | 1.65 sec                                                     | 1.67 sec: 1.01x slower                                                       |
| async_tree_io_tg         | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                                       |
| xml_etree_generate       | 86.1 ms                                                      | 87.1 ms: 1.01x slower                                                        |
| pathlib                  | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                                        |
| dask                     | 392 ms                                                       | 398 ms: 1.01x slower                                                         |
| xml_etree_process        | 58.4 ms                                                      | 59.3 ms: 1.02x slower                                                        |
| create_gc_cycles         | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                                        |
| pprint_safe_repr         | 807 ms                                                       | 821 ms: 1.02x slower                                                         |
| json_loads               | 24.4 us                                                      | 24.8 us: 1.02x slower                                                        |
| deepcopy                 | 368 us                                                       | 377 us: 1.02x slower                                                         |
| 2to3                     | 285 ms                                                       | 292 ms: 1.02x slower                                                         |
| float                    | 76.6 ms                                                      | 78.5 ms: 1.02x slower                                                        |
| async_tree_io            | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| json                     | 5.12 ms                                                      | 5.25 ms: 1.03x slower                                                        |
| pycparser                | 1.23 sec                                                     | 1.27 sec: 1.03x slower                                                       |
| tomli_loads              | 2.16 sec                                                     | 2.22 sec: 1.03x slower                                                       |
| sqlglot_optimize         | 57.5 ms                                                      | 59.0 ms: 1.03x slower                                                        |
| sympy_expand             | 484 ms                                                       | 498 ms: 1.03x slower                                                         |
| gc_traversal             | 3.48 ms                                                      | 3.58 ms: 1.03x slower                                                        |
| xml_etree_parse          | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| json_dumps               | 10.2 ms                                                      | 10.6 ms: 1.03x slower                                                        |
| mako                     | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                        |
| logging_silent           | 94.4 ns                                                      | 97.6 ns: 1.03x slower                                                        |
| regex_dna                | 239 ms                                                       | 247 ms: 1.04x slower                                                         |
| xml_etree_iterparse      | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| chameleon                | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                                        |
| dulwich_log              | 65.4 ms                                                      | 68.5 ms: 1.05x slower                                                        |
| deepcopy_memo            | 36.8 us                                                      | 39.0 us: 1.06x slower                                                        |
| hexiom                   | 5.96 ms                                                      | 6.31 ms: 1.06x slower                                                        |
| regex_v8                 | 23.6 ms                                                      | 25.4 ms: 1.07x slower                                                        |
| python_startup           | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| deltablue                | 3.24 ms                                                      | 3.54 ms: 1.09x slower                                                        |
| fannkuch                 | 350 ms                                                       | 386 ms: 1.10x slower                                                         |
| go                       | 150 ms                                                       | 167 ms: 1.12x slower                                                         |
| richards_super           | 51.3 ms                                                      | 58.4 ms: 1.14x slower                                                        |
| richards                 | 45.7 ms                                                      | 52.3 ms: 1.14x slower                                                        |
| pyflate                  | 439 ms                                                       | 503 ms: 1.15x slower                                                         |
| telco                    | 6.96 ms                                                      | 8.09 ms: 1.16x slower                                                        |
| coverage                 | 66.7 ms                                                      | 78.4 ms: 1.18x slower                                                        |
| python_startup_no_site   | 8.64 ms                                                      | 11.0 ms: 1.27x slower                                                        |
| scimark_sor              | 109 ms                                                       | 145 ms: 1.33x slower                                                         |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (14): pickle_list, async_tree_cpu_io_mixed, async_tree_memoization, unpickle_list, asyncio_websockets, async_tree_cpu_io_mixed_tg, unpack_sequence, regex_effbot, bench_thread_pool, unpickle_pure_python, deepcopy_reduce, scimark_sparse_mat_mult, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 94.64% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.88x