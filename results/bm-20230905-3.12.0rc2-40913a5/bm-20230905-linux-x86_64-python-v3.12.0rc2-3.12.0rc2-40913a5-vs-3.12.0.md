
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0rc2
- machine: linux-x86_64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 268 ms: 1.02x faster                                         |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                       |
| Geometric mean | (ref)                                                  | 1.02x faster                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.03x faster                                         |
| async_tree_io           | 1.16 sec                                               | 1.14 sec: 1.01x faster                                       |
| async_tree_none         | 472 ms                                                 | 465 ms: 1.01x faster                                         |
| async_tree_memoization  | 578 ms                                                 | 571 ms: 1.01x faster                                         |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.1 ms: 1.06x faster                                        |
| nbody          | 97.0 ms                                                | 93.4 ms: 1.04x faster                                        |
| pidigits       | 187 ms                                                 | 212 ms: 1.13x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 23.1 ms                                                | 22.3 ms: 1.04x faster                                        |
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                         |
| regex_effbot   | 3.61 ms                                                | 3.59 ms: 1.01x faster                                        |
| regex_dna      | 212 ms                                                 | 213 ms: 1.01x slower                                         |
| Geometric mean | (ref)                                                  | 1.02x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| json_loads           | 28.5 us                                                | 25.1 us: 1.14x faster                                        |
| pickle_dict          | 35.5 us                                                | 31.8 us: 1.12x faster                                        |
| pickle               | 11.6 us                                                | 10.6 us: 1.10x faster                                        |
| pickle_list          | 5.08 us                                                | 4.67 us: 1.09x faster                                        |
| tomli_loads          | 2.33 sec                                               | 2.20 sec: 1.06x faster                                       |
| xml_etree_generate   | 89.2 ms                                                | 84.3 ms: 1.06x faster                                        |
| xml_etree_process    | 61.7 ms                                                | 58.7 ms: 1.05x faster                                        |
| json_dumps           | 10.4 ms                                                | 9.89 ms: 1.05x faster                                        |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                        |
| unpickle_pure_python | 230 us                                                 | 219 us: 1.05x faster                                         |
| xml_etree_parse      | 159 ms                                                 | 154 ms: 1.04x faster                                         |
| xml_etree_iterparse  | 107 ms                                                 | 103 ms: 1.03x faster                                         |
| pickle_pure_python   | 324 us                                                 | 314 us: 1.03x faster                                         |
| unpickle_list        | 5.29 us                                                | 5.38 us: 1.02x slower                                        |
| Geometric mean       | (ref)                                                  | 1.06x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 9.46 ms: 1.01x faster                                        |
| python_startup_no_site | 6.94 ms                                                | 6.88 ms: 1.01x faster                                        |
| Geometric mean         | (ref)                                                  | 1.01x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.9 ms: 1.09x faster                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| unpack_sequence          | 54.0 ns                                                | 45.6 ns: 1.18x faster                                        |
| json_loads               | 28.5 us                                                | 25.1 us: 1.14x faster                                        |
| pickle_dict              | 35.5 us                                                | 31.8 us: 1.12x faster                                        |
| pickle                   | 11.6 us                                                | 10.6 us: 1.10x faster                                        |
| json                     | 5.26 ms                                                | 4.80 ms: 1.10x faster                                        |
| typing_runtime_protocols | 158 us                                                 | 144 us: 1.09x faster                                         |
| mako                     | 11.9 ms                                                | 10.9 ms: 1.09x faster                                        |
| pickle_list              | 5.08 us                                                | 4.67 us: 1.09x faster                                        |
| deepcopy_memo            | 40.7 us                                                | 37.5 us: 1.09x faster                                        |
| spectral_norm            | 115 ms                                                 | 106 ms: 1.08x faster                                         |
| deepcopy_reduce          | 3.35 us                                                | 3.12 us: 1.07x faster                                        |
| deltablue                | 3.72 ms                                                | 3.49 ms: 1.07x faster                                        |
| raytrace                 | 312 ms                                                 | 293 ms: 1.06x faster                                         |
| logging_silent           | 104 ns                                                 | 98.5 ns: 1.06x faster                                        |
| tomli_loads              | 2.33 sec                                               | 2.20 sec: 1.06x faster                                       |
| meteor_contest           | 112 ms                                                 | 106 ms: 1.06x faster                                         |
| richards                 | 45.8 ms                                                | 43.3 ms: 1.06x faster                                        |
| float                    | 84.7 ms                                                | 80.1 ms: 1.06x faster                                        |
| deepcopy                 | 371 us                                                 | 351 us: 1.06x faster                                         |
| xml_etree_generate       | 89.2 ms                                                | 84.3 ms: 1.06x faster                                        |
| richards_super           | 51.5 ms                                                | 48.9 ms: 1.05x faster                                        |
| pprint_safe_repr         | 776 ms                                                 | 736 ms: 1.05x faster                                         |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                        |
| scimark_monte_carlo      | 75.1 ms                                                | 71.4 ms: 1.05x faster                                        |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.81 ms: 1.05x faster                                        |
| xml_etree_process        | 61.7 ms                                                | 58.7 ms: 1.05x faster                                        |
| comprehensions           | 21.8 us                                                | 20.7 us: 1.05x faster                                        |
| coroutines               | 23.2 ms                                                | 22.1 ms: 1.05x faster                                        |
| json_dumps               | 10.4 ms                                                | 9.89 ms: 1.05x faster                                        |
| unpickle                 | 15.9 us                                                | 15.1 us: 1.05x faster                                        |
| unpickle_pure_python     | 230 us                                                 | 219 us: 1.05x faster                                         |
| scimark_fft              | 382 ms                                                 | 364 ms: 1.05x faster                                         |
| chaos                    | 67.0 ms                                                | 63.8 ms: 1.05x faster                                        |
| fannkuch                 | 417 ms                                                 | 400 ms: 1.04x faster                                         |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.04x faster                                         |
| async_generators         | 463 ms                                                 | 445 ms: 1.04x faster                                         |
| scimark_sor              | 129 ms                                                 | 124 ms: 1.04x faster                                         |
| pprint_pformat           | 1.57 sec                                               | 1.51 sec: 1.04x faster                                       |
| telco                    | 7.10 ms                                                | 6.83 ms: 1.04x faster                                        |
| hexiom                   | 6.41 ms                                                | 6.17 ms: 1.04x faster                                        |
| nbody                    | 97.0 ms                                                | 93.4 ms: 1.04x faster                                        |
| regex_v8                 | 23.1 ms                                                | 22.3 ms: 1.04x faster                                        |
| xml_etree_parse          | 159 ms                                                 | 154 ms: 1.04x faster                                         |
| xml_etree_iterparse      | 107 ms                                                 | 103 ms: 1.03x faster                                         |
| sqlite_synth             | 2.83 us                                                | 2.74 us: 1.03x faster                                        |
| pyflate                  | 482 ms                                                 | 467 ms: 1.03x faster                                         |
| pickle_pure_python       | 324 us                                                 | 314 us: 1.03x faster                                         |
| go                       | 139 ms                                                 | 135 ms: 1.03x faster                                         |
| regex_compile            | 148 ms                                                 | 144 ms: 1.03x faster                                         |
| crypto_pyaes             | 81.9 ms                                                | 79.6 ms: 1.03x faster                                        |
| logging_simple           | 6.46 us                                                | 6.28 us: 1.03x faster                                        |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.03x faster                                         |
| sqlglot_optimize         | 54.8 ms                                                | 53.5 ms: 1.02x faster                                        |
| 2to3                     | 274 ms                                                 | 268 ms: 1.02x faster                                         |
| nqueens                  | 83.3 ms                                                | 81.4 ms: 1.02x faster                                        |
| mdp                      | 2.63 sec                                               | 2.58 sec: 1.02x faster                                       |
| sqlglot_transpile        | 1.68 ms                                                | 1.65 ms: 1.02x faster                                        |
| sqlglot_parse            | 1.36 ms                                                | 1.33 ms: 1.02x faster                                        |
| docutils                 | 2.77 sec                                               | 2.71 sec: 1.02x faster                                       |
| logging_format           | 7.23 us                                                | 7.08 us: 1.02x faster                                        |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                         |
| pycparser                | 1.18 sec                                               | 1.16 sec: 1.02x faster                                       |
| bench_thread_pool        | 842 us                                                 | 829 us: 1.02x faster                                         |
| sqlalchemy_imperative    | 18.7 ms                                                | 18.4 ms: 1.01x faster                                        |
| async_tree_io            | 1.16 sec                                               | 1.14 sec: 1.01x faster                                       |
| async_tree_none          | 472 ms                                                 | 465 ms: 1.01x faster                                         |
| generators               | 31.2 ms                                                | 30.8 ms: 1.01x faster                                        |
| async_tree_memoization   | 578 ms                                                 | 571 ms: 1.01x faster                                         |
| sqlalchemy_declarative   | 147 ms                                                 | 145 ms: 1.01x faster                                         |
| python_startup           | 9.55 ms                                                | 9.46 ms: 1.01x faster                                        |
| python_startup_no_site   | 6.94 ms                                                | 6.88 ms: 1.01x faster                                        |
| regex_effbot             | 3.61 ms                                                | 3.59 ms: 1.01x faster                                        |
| dulwich_log              | 68.5 ms                                                | 68.2 ms: 1.00x faster                                        |
| regex_dna                | 212 ms                                                 | 213 ms: 1.01x slower                                         |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                       |
| gc_traversal             | 3.79 ms                                                | 3.83 ms: 1.01x slower                                        |
| unpickle_list            | 5.29 us                                                | 5.38 us: 1.02x slower                                        |
| create_gc_cycles         | 1.48 ms                                                | 1.51 ms: 1.02x slower                                        |
| asyncio_tcp              | 491 ms                                                 | 505 ms: 1.03x slower                                         |
| pidigits                 | 187 ms                                                 | 212 ms: 1.13x slower                                         |
| coverage                 | 72.7 ms                                                | 94.7 ms: 1.30x slower                                        |
| dask                     | 372 ms                                                 | 537 ms: 1.45x slower                                         |
| Geometric mean           | (ref)                                                  | 1.03x faster                                                 |

Benchmark hidden because not significant (2): tornado_http, bench_mp_pool
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x