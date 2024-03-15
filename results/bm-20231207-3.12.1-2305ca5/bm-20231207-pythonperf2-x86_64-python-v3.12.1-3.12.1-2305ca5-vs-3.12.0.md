
# Results vs. 3.12.0

- fork: python
- ref: v3.12.1
- machine: linux-x86_64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 281 ms: 1.02x faster                                         |
| chameleon      | 7.23 ms                                                      | 7.31 ms: 1.01x slower                                        |
| docutils       | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                       |
| tornado_http   | 121 ms                                                       | 118 ms: 1.02x faster                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_memoization_tg, async_tree_io, async_tree_memoization, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 85.5 ms: 1.03x faster                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (2): pidigits, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 138 ms: 1.04x faster                                         |
| regex_effbot   | 3.57 ms                                                      | 3.54 ms: 1.01x faster                                        |
| regex_v8       | 23.6 ms                                                      | 23.5 ms: 1.01x faster                                        |
| regex_dna      | 239 ms                                                       | 244 ms: 1.02x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.2 us: 1.04x faster                                        |
| pickle               | 10.5 us                                                      | 10.1 us: 1.04x faster                                        |
| unpickle_pure_python | 210 us                                                       | 205 us: 1.02x faster                                         |
| xml_etree_generate   | 86.1 ms                                                      | 84.6 ms: 1.02x faster                                        |
| xml_etree_iterparse  | 103 ms                                                       | 102 ms: 1.01x faster                                         |
| tomli_loads          | 2.16 sec                                                     | 2.14 sec: 1.01x faster                                       |
| xml_etree_process    | 58.4 ms                                                      | 58.0 ms: 1.01x faster                                        |
| pickle_pure_python   | 318 us                                                       | 320 us: 1.01x slower                                         |
| pickle_list          | 4.43 us                                                      | 4.46 us: 1.01x slower                                        |
| xml_etree_parse      | 144 ms                                                       | 145 ms: 1.01x slower                                         |
| json_loads           | 24.4 us                                                      | 24.6 us: 1.01x slower                                        |
| unpickle             | 14.8 us                                                      | 15.2 us: 1.03x slower                                        |
| unpickle_list        | 4.66 us                                                      | 4.82 us: 1.03x slower                                        |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.53 ms: 1.01x faster                                        |
| python_startup         | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                        |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 37.5 ms: 1.02x faster                                        |
| Geometric mean  | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf2-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols | 152 us                                                       | 122 us: 1.24x faster                                         |
| mypy2                    | 830 ms                                                       | 720 ms: 1.15x faster                                         |
| unpack_sequence          | 53.2 ns                                                      | 49.1 ns: 1.08x faster                                        |
| comprehensions           | 21.9 us                                                      | 20.8 us: 1.05x faster                                        |
| logging_format           | 7.48 us                                                      | 7.11 us: 1.05x faster                                        |
| pickle_dict              | 32.5 us                                                      | 31.2 us: 1.04x faster                                        |
| pickle                   | 10.5 us                                                      | 10.1 us: 1.04x faster                                        |
| regex_compile            | 144 ms                                                       | 138 ms: 1.04x faster                                         |
| logging_simple           | 6.71 us                                                      | 6.49 us: 1.03x faster                                        |
| sqlite_synth             | 2.77 us                                                      | 2.69 us: 1.03x faster                                        |
| chaos                    | 64.0 ms                                                      | 62.1 ms: 1.03x faster                                        |
| async_generators         | 390 ms                                                       | 379 ms: 1.03x faster                                         |
| richards                 | 45.7 ms                                                      | 44.5 ms: 1.03x faster                                        |
| nbody                    | 88.0 ms                                                      | 85.5 ms: 1.03x faster                                        |
| sympy_sum                | 162 ms                                                       | 158 ms: 1.03x faster                                         |
| sympy_integrate          | 23.9 ms                                                      | 23.3 ms: 1.03x faster                                        |
| tornado_http             | 121 ms                                                       | 118 ms: 1.02x faster                                         |
| unpickle_pure_python     | 210 us                                                       | 205 us: 1.02x faster                                         |
| crypto_pyaes             | 80.3 ms                                                      | 78.7 ms: 1.02x faster                                        |
| pprint_safe_repr         | 807 ms                                                       | 791 ms: 1.02x faster                                         |
| scimark_monte_carlo      | 69.0 ms                                                      | 67.7 ms: 1.02x faster                                        |
| pprint_pformat           | 1.65 sec                                                     | 1.62 sec: 1.02x faster                                       |
| django_template          | 38.2 ms                                                      | 37.5 ms: 1.02x faster                                        |
| mdp                      | 2.57 sec                                                     | 2.52 sec: 1.02x faster                                       |
| sympy_str                | 302 ms                                                       | 297 ms: 1.02x faster                                         |
| xml_etree_generate       | 86.1 ms                                                      | 84.6 ms: 1.02x faster                                        |
| dulwich_log              | 65.4 ms                                                      | 64.2 ms: 1.02x faster                                        |
| docutils                 | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                       |
| 2to3                     | 285 ms                                                       | 281 ms: 1.02x faster                                         |
| scimark_fft              | 301 ms                                                       | 297 ms: 1.01x faster                                         |
| pycparser                | 1.23 sec                                                     | 1.22 sec: 1.01x faster                                       |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                       |
| coroutines               | 23.0 ms                                                      | 22.7 ms: 1.01x faster                                        |
| scimark_lu               | 98.8 ms                                                      | 97.5 ms: 1.01x faster                                        |
| python_startup_no_site   | 8.64 ms                                                      | 8.53 ms: 1.01x faster                                        |
| richards_super           | 51.3 ms                                                      | 50.7 ms: 1.01x faster                                        |
| xml_etree_iterparse      | 103 ms                                                       | 102 ms: 1.01x faster                                         |
| asyncio_tcp              | 378 ms                                                       | 374 ms: 1.01x faster                                         |
| regex_effbot             | 3.57 ms                                                      | 3.54 ms: 1.01x faster                                        |
| sympy_expand             | 484 ms                                                       | 479 ms: 1.01x faster                                         |
| generators               | 37.4 ms                                                      | 37.1 ms: 1.01x faster                                        |
| gunicorn                 | 1.00 ms                                                      | 992 us: 1.01x faster                                         |
| hexiom                   | 5.96 ms                                                      | 5.91 ms: 1.01x faster                                        |
| tomli_loads              | 2.16 sec                                                     | 2.14 sec: 1.01x faster                                       |
| go                       | 150 ms                                                       | 149 ms: 1.01x faster                                         |
| python_startup           | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                        |
| xml_etree_process        | 58.4 ms                                                      | 58.0 ms: 1.01x faster                                        |
| fannkuch                 | 350 ms                                                       | 348 ms: 1.01x faster                                         |
| regex_v8                 | 23.6 ms                                                      | 23.5 ms: 1.01x faster                                        |
| scimark_sor              | 109 ms                                                       | 108 ms: 1.00x faster                                         |
| pickle_pure_python       | 318 us                                                       | 320 us: 1.01x slower                                         |
| pyflate                  | 439 ms                                                       | 441 ms: 1.01x slower                                         |
| pickle_list              | 4.43 us                                                      | 4.46 us: 1.01x slower                                        |
| spectral_norm            | 91.6 ms                                                      | 92.6 ms: 1.01x slower                                        |
| xml_etree_parse          | 144 ms                                                       | 145 ms: 1.01x slower                                         |
| chameleon                | 7.23 ms                                                      | 7.31 ms: 1.01x slower                                        |
| json_loads               | 24.4 us                                                      | 24.6 us: 1.01x slower                                        |
| coverage                 | 66.7 ms                                                      | 67.6 ms: 1.01x slower                                        |
| json                     | 5.12 ms                                                      | 5.19 ms: 1.01x slower                                        |
| logging_silent           | 94.4 ns                                                      | 95.8 ns: 1.01x slower                                        |
| deepcopy_memo            | 36.8 us                                                      | 37.4 us: 1.02x slower                                        |
| meteor_contest           | 128 ms                                                       | 131 ms: 1.02x slower                                         |
| regex_dna                | 239 ms                                                       | 244 ms: 1.02x slower                                         |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.31 ms: 1.03x slower                                        |
| unpickle                 | 14.8 us                                                      | 15.2 us: 1.03x slower                                        |
| unpickle_list            | 4.66 us                                                      | 4.82 us: 1.03x slower                                        |
| telco                    | 6.96 ms                                                      | 7.47 ms: 1.07x slower                                        |
| gc_traversal             | 3.48 ms                                                      | 4.10 ms: 1.18x slower                                        |
| Geometric mean           | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (30): sqlalchemy_imperative, bench_thread_pool, dask, async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg, aiohttp, bench_mp_pool, deepcopy, async_tree_none_tg, async_tree_memoization_tg, pathlib, pidigits, json_dumps, async_tree_io, async_tree_memoization, sqlglot_parse, async_tree_io_tg, nqueens, sqlglot_transpile, sqlglot_optimize, sqlalchemy_declarative, deltablue, deepcopy_reduce, sqlglot_normalize, raytrace, float, create_gc_cycles, mako, asyncio_websockets


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.91x