
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0rc2
- machine: linux-x86_64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.01x slower \*
- HPT reliability: 93.44%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 287 ms: 1.01x slower                                               |
| docutils       | 2.87 sec                                                     | 2.90 sec: 1.01x slower                                             |
| tornado_http   | 121 ms                                                       | 120 ms: 1.01x faster                                               |
| Geometric mean | (ref)                                                        | 1.00x slower                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none        | 452 ms                                                       | 458 ms: 1.01x slower                                               |
| async_tree_memoization | 544 ms                                                       | 552 ms: 1.02x slower                                               |
| async_tree_io          | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                             |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                       |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                               |
| float          | 76.6 ms                                                      | 79.6 ms: 1.04x slower                                              |
| Geometric mean | (ref)                                                        | 1.01x slower                                                       |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.52 ms: 1.02x faster                                              |
| regex_compile  | 144 ms                                                       | 146 ms: 1.01x slower                                               |
| Geometric mean | (ref)                                                        | 1.00x slower                                                       |

Benchmark hidden because not significant (2): regex_dna, regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 10.4 us: 1.01x faster                                              |
| pickle_dict          | 32.5 us                                                      | 32.4 us: 1.00x faster                                              |
| xml_etree_generate   | 86.1 ms                                                      | 85.8 ms: 1.00x faster                                              |
| tomli_loads          | 2.16 sec                                                     | 2.17 sec: 1.00x slower                                             |
| pickle_list          | 4.43 us                                                      | 4.46 us: 1.01x slower                                              |
| xml_etree_process    | 58.4 ms                                                      | 58.9 ms: 1.01x slower                                              |
| unpickle_pure_python | 210 us                                                       | 212 us: 1.01x slower                                               |
| xml_etree_parse      | 144 ms                                                       | 146 ms: 1.01x slower                                               |
| unpickle_list        | 4.66 us                                                      | 4.75 us: 1.02x slower                                              |
| pickle_pure_python   | 318 us                                                       | 326 us: 1.02x slower                                               |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                       |

Benchmark hidden because not significant (4): unpickle, json_dumps, json_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.67 ms: 1.00x slower                                              |
| python_startup         | 11.6 ms                                                      | 11.7 ms: 1.01x slower                                              |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 9.92 ms: 1.01x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-pythonperf2-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| scimark_fft              | 301 ms                                                       | 288 ms: 1.05x faster                                               |
| fannkuch                 | 350 ms                                                       | 335 ms: 1.05x faster                                               |
| chaos                    | 64.0 ms                                                      | 62.3 ms: 1.03x faster                                              |
| richards                 | 45.7 ms                                                      | 44.6 ms: 1.03x faster                                              |
| async_generators         | 390 ms                                                       | 381 ms: 1.02x faster                                               |
| mdp                      | 2.57 sec                                                     | 2.52 sec: 1.02x faster                                             |
| generators               | 37.4 ms                                                      | 36.7 ms: 1.02x faster                                              |
| sqlite_synth             | 2.77 us                                                      | 2.72 us: 1.02x faster                                              |
| meteor_contest           | 128 ms                                                       | 126 ms: 1.02x faster                                               |
| richards_super           | 51.3 ms                                                      | 50.5 ms: 1.02x faster                                              |
| typing_runtime_protocols | 152 us                                                       | 149 us: 1.02x faster                                               |
| regex_effbot             | 3.57 ms                                                      | 3.52 ms: 1.02x faster                                              |
| tornado_http             | 121 ms                                                       | 120 ms: 1.01x faster                                               |
| scimark_lu               | 98.8 ms                                                      | 97.6 ms: 1.01x faster                                              |
| go                       | 150 ms                                                       | 148 ms: 1.01x faster                                               |
| logging_format           | 7.48 us                                                      | 7.40 us: 1.01x faster                                              |
| pickle                   | 10.5 us                                                      | 10.4 us: 1.01x faster                                              |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                             |
| mako                     | 10.0 ms                                                      | 9.92 ms: 1.01x faster                                              |
| dulwich_log              | 65.4 ms                                                      | 64.9 ms: 1.01x faster                                              |
| pickle_dict              | 32.5 us                                                      | 32.4 us: 1.00x faster                                              |
| pidigits                 | 265 ms                                                       | 264 ms: 1.00x faster                                               |
| spectral_norm            | 91.6 ms                                                      | 91.3 ms: 1.00x faster                                              |
| xml_etree_generate       | 86.1 ms                                                      | 85.8 ms: 1.00x faster                                              |
| telco                    | 6.96 ms                                                      | 6.99 ms: 1.00x slower                                              |
| python_startup_no_site   | 8.64 ms                                                      | 8.67 ms: 1.00x slower                                              |
| tomli_loads              | 2.16 sec                                                     | 2.17 sec: 1.00x slower                                             |
| 2to3                     | 285 ms                                                       | 287 ms: 1.01x slower                                               |
| pprint_pformat           | 1.65 sec                                                     | 1.67 sec: 1.01x slower                                             |
| scimark_monte_carlo      | 69.0 ms                                                      | 69.4 ms: 1.01x slower                                              |
| python_startup           | 11.6 ms                                                      | 11.7 ms: 1.01x slower                                              |
| pickle_list              | 4.43 us                                                      | 4.46 us: 1.01x slower                                              |
| xml_etree_process        | 58.4 ms                                                      | 58.9 ms: 1.01x slower                                              |
| pyflate                  | 439 ms                                                       | 443 ms: 1.01x slower                                               |
| unpickle_pure_python     | 210 us                                                       | 212 us: 1.01x slower                                               |
| unpack_sequence          | 53.2 ns                                                      | 53.7 ns: 1.01x slower                                              |
| docutils                 | 2.87 sec                                                     | 2.90 sec: 1.01x slower                                             |
| pathlib                  | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                              |
| coroutines               | 23.0 ms                                                      | 23.3 ms: 1.01x slower                                              |
| crypto_pyaes             | 80.3 ms                                                      | 81.5 ms: 1.01x slower                                              |
| xml_etree_parse          | 144 ms                                                       | 146 ms: 1.01x slower                                               |
| regex_compile            | 144 ms                                                       | 146 ms: 1.01x slower                                               |
| async_tree_none          | 452 ms                                                       | 458 ms: 1.01x slower                                               |
| async_tree_memoization   | 544 ms                                                       | 552 ms: 1.02x slower                                               |
| pprint_safe_repr         | 807 ms                                                       | 820 ms: 1.02x slower                                               |
| deltablue                | 3.24 ms                                                      | 3.29 ms: 1.02x slower                                              |
| scimark_sor              | 109 ms                                                       | 111 ms: 1.02x slower                                               |
| async_tree_io            | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                             |
| logging_silent           | 94.4 ns                                                      | 95.9 ns: 1.02x slower                                              |
| nqueens                  | 89.9 ms                                                      | 91.3 ms: 1.02x slower                                              |
| logging_simple           | 6.71 us                                                      | 6.84 us: 1.02x slower                                              |
| gc_traversal             | 3.48 ms                                                      | 3.54 ms: 1.02x slower                                              |
| unpickle_list            | 4.66 us                                                      | 4.75 us: 1.02x slower                                              |
| sqlglot_transpile        | 1.78 ms                                                      | 1.81 ms: 1.02x slower                                              |
| sqlglot_optimize         | 57.5 ms                                                      | 58.6 ms: 1.02x slower                                              |
| asyncio_tcp              | 378 ms                                                       | 386 ms: 1.02x slower                                               |
| pickle_pure_python       | 318 us                                                       | 326 us: 1.02x slower                                               |
| deepcopy_reduce          | 3.37 us                                                      | 3.45 us: 1.03x slower                                              |
| deepcopy_memo            | 36.8 us                                                      | 37.7 us: 1.03x slower                                              |
| bench_thread_pool        | 950 us                                                       | 975 us: 1.03x slower                                               |
| sqlglot_parse            | 1.38 ms                                                      | 1.41 ms: 1.03x slower                                              |
| raytrace                 | 298 ms                                                       | 308 ms: 1.03x slower                                               |
| deepcopy                 | 368 us                                                       | 382 us: 1.04x slower                                               |
| sqlglot_normalize        | 116 ms                                                       | 120 ms: 1.04x slower                                               |
| float                    | 76.6 ms                                                      | 79.6 ms: 1.04x slower                                              |
| create_gc_cycles         | 1.59 ms                                                      | 1.66 ms: 1.05x slower                                              |
| coverage                 | 66.7 ms                                                      | 88.0 ms: 1.32x slower                                              |
| dask                     | 392 ms                                                       | 566 ms: 1.44x slower                                               |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                       |

Benchmark hidden because not significant (14): pycparser, nbody, unpickle, comprehensions, regex_dna, scimark_sparse_mat_mult, json_dumps, json, json_loads, hexiom, xml_etree_iterparse, regex_v8, bench_mp_pool, async_tree_cpu_io_mixed
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 93.44% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x