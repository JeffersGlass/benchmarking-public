
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0rc1
- machine: linux-x86_64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 267 ms: 1.03x faster                                         |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.02x faster                                       |
| tornado_http   | 103 ms                                                 | 99.1 ms: 1.04x faster                                        |
| Geometric mean | (ref)                                                  | 1.03x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.02x faster                                         |
| async_tree_io           | 1.16 sec                                               | 1.16 sec: 1.01x slower                                       |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                 |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 89.6 ms: 1.08x faster                                        |
| float          | 84.7 ms                                                | 79.3 ms: 1.07x faster                                        |
| pidigits       | 187 ms                                                 | 201 ms: 1.07x slower                                         |
| Geometric mean | (ref)                                                  | 1.03x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 23.1 ms                                                | 22.5 ms: 1.03x faster                                        |
| regex_effbot   | 3.61 ms                                                | 3.52 ms: 1.03x faster                                        |
| regex_compile  | 148 ms                                                 | 145 ms: 1.02x faster                                         |
| regex_dna      | 212 ms                                                 | 210 ms: 1.01x faster                                         |
| Geometric mean | (ref)                                                  | 1.02x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 31.4 us: 1.13x faster                                        |
| json_loads           | 28.5 us                                                | 25.4 us: 1.12x faster                                        |
| pickle_list          | 5.08 us                                                | 4.55 us: 1.12x faster                                        |
| pickle               | 11.6 us                                                | 10.8 us: 1.08x faster                                        |
| json_dumps           | 10.4 ms                                                | 9.75 ms: 1.07x faster                                        |
| unpickle_list        | 5.29 us                                                | 4.98 us: 1.06x faster                                        |
| unpickle             | 15.9 us                                                | 14.9 us: 1.06x faster                                        |
| tomli_loads          | 2.33 sec                                               | 2.21 sec: 1.05x faster                                       |
| unpickle_pure_python | 230 us                                                 | 219 us: 1.05x faster                                         |
| xml_etree_generate   | 89.2 ms                                                | 85.4 ms: 1.04x faster                                        |
| pickle_pure_python   | 324 us                                                 | 311 us: 1.04x faster                                         |
| xml_etree_process    | 61.7 ms                                                | 59.2 ms: 1.04x faster                                        |
| xml_etree_parse      | 159 ms                                                 | 155 ms: 1.03x faster                                         |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                         |
| Geometric mean       | (ref)                                                  | 1.07x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 9.30 ms: 1.03x faster                                        |
| python_startup_no_site | 6.94 ms                                                | 6.76 ms: 1.03x faster                                        |
| Geometric mean         | (ref)                                                  | 1.03x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.7 ms: 1.11x faster                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict              | 35.5 us                                                | 31.4 us: 1.13x faster                                        |
| json_loads               | 28.5 us                                                | 25.4 us: 1.12x faster                                        |
| pickle_list              | 5.08 us                                                | 4.55 us: 1.12x faster                                        |
| mako                     | 11.9 ms                                                | 10.7 ms: 1.11x faster                                        |
| json                     | 5.26 ms                                                | 4.77 ms: 1.10x faster                                        |
| deepcopy_memo            | 40.7 us                                                | 37.1 us: 1.10x faster                                        |
| pyflate                  | 482 ms                                                 | 444 ms: 1.09x faster                                         |
| nbody                    | 97.0 ms                                                | 89.6 ms: 1.08x faster                                        |
| pickle                   | 11.6 us                                                | 10.8 us: 1.08x faster                                        |
| spectral_norm            | 115 ms                                                 | 107 ms: 1.08x faster                                         |
| meteor_contest           | 112 ms                                                 | 105 ms: 1.07x faster                                         |
| scimark_fft              | 382 ms                                                 | 356 ms: 1.07x faster                                         |
| float                    | 84.7 ms                                                | 79.3 ms: 1.07x faster                                        |
| deepcopy_reduce          | 3.35 us                                                | 3.14 us: 1.07x faster                                        |
| json_dumps               | 10.4 ms                                                | 9.75 ms: 1.07x faster                                        |
| unpickle_list            | 5.29 us                                                | 4.98 us: 1.06x faster                                        |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.06x faster                                        |
| pathlib                  | 19.3 ms                                                | 18.3 ms: 1.06x faster                                        |
| fannkuch                 | 417 ms                                                 | 394 ms: 1.06x faster                                         |
| typing_runtime_protocols | 158 us                                                 | 149 us: 1.06x faster                                         |
| comprehensions           | 21.8 us                                                | 20.7 us: 1.05x faster                                        |
| pprint_safe_repr         | 776 ms                                                 | 737 ms: 1.05x faster                                         |
| tomli_loads              | 2.33 sec                                               | 2.21 sec: 1.05x faster                                       |
| raytrace                 | 312 ms                                                 | 297 ms: 1.05x faster                                         |
| pprint_pformat           | 1.57 sec                                               | 1.50 sec: 1.05x faster                                       |
| unpickle_pure_python     | 230 us                                                 | 219 us: 1.05x faster                                         |
| scimark_monte_carlo      | 75.1 ms                                                | 71.7 ms: 1.05x faster                                        |
| deltablue                | 3.72 ms                                                | 3.55 ms: 1.05x faster                                        |
| chaos                    | 67.0 ms                                                | 64.0 ms: 1.05x faster                                        |
| deepcopy                 | 371 us                                                 | 355 us: 1.05x faster                                         |
| crypto_pyaes             | 81.9 ms                                                | 78.4 ms: 1.04x faster                                        |
| xml_etree_generate       | 89.2 ms                                                | 85.4 ms: 1.04x faster                                        |
| pickle_pure_python       | 324 us                                                 | 311 us: 1.04x faster                                         |
| logging_simple           | 6.46 us                                                | 6.20 us: 1.04x faster                                        |
| xml_etree_process        | 61.7 ms                                                | 59.2 ms: 1.04x faster                                        |
| mdp                      | 2.63 sec                                               | 2.54 sec: 1.04x faster                                       |
| tornado_http             | 103 ms                                                 | 99.1 ms: 1.04x faster                                        |
| telco                    | 7.10 ms                                                | 6.86 ms: 1.04x faster                                        |
| scimark_sor              | 129 ms                                                 | 125 ms: 1.03x faster                                         |
| richards                 | 45.8 ms                                                | 44.3 ms: 1.03x faster                                        |
| generators               | 31.2 ms                                                | 30.2 ms: 1.03x faster                                        |
| logging_format           | 7.23 us                                                | 6.99 us: 1.03x faster                                        |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.89 ms: 1.03x faster                                        |
| hexiom                   | 6.41 ms                                                | 6.21 ms: 1.03x faster                                        |
| scimark_lu               | 118 ms                                                 | 114 ms: 1.03x faster                                         |
| go                       | 139 ms                                                 | 135 ms: 1.03x faster                                         |
| pycparser                | 1.18 sec                                               | 1.14 sec: 1.03x faster                                       |
| xml_etree_parse          | 159 ms                                                 | 155 ms: 1.03x faster                                         |
| sqlite_synth             | 2.83 us                                                | 2.75 us: 1.03x faster                                        |
| async_generators         | 463 ms                                                 | 450 ms: 1.03x faster                                         |
| regex_v8                 | 23.1 ms                                                | 22.5 ms: 1.03x faster                                        |
| python_startup           | 9.55 ms                                                | 9.30 ms: 1.03x faster                                        |
| unpack_sequence          | 54.0 ns                                                | 52.6 ns: 1.03x faster                                        |
| python_startup_no_site   | 6.94 ms                                                | 6.76 ms: 1.03x faster                                        |
| 2to3                     | 274 ms                                                 | 267 ms: 1.03x faster                                         |
| xml_etree_iterparse      | 107 ms                                                 | 104 ms: 1.03x faster                                         |
| regex_effbot             | 3.61 ms                                                | 3.52 ms: 1.03x faster                                        |
| docutils                 | 2.77 sec                                               | 2.70 sec: 1.02x faster                                       |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.02x faster                                         |
| richards_super           | 51.5 ms                                                | 50.3 ms: 1.02x faster                                        |
| regex_compile            | 148 ms                                                 | 145 ms: 1.02x faster                                         |
| nqueens                  | 83.3 ms                                                | 81.5 ms: 1.02x faster                                        |
| coroutines               | 23.2 ms                                                | 22.7 ms: 1.02x faster                                        |
| logging_silent           | 104 ns                                                 | 102 ns: 1.02x faster                                         |
| sqlalchemy_imperative    | 18.7 ms                                                | 18.4 ms: 1.02x faster                                        |
| sqlalchemy_declarative   | 147 ms                                                 | 145 ms: 1.01x faster                                         |
| bench_thread_pool        | 842 us                                                 | 832 us: 1.01x faster                                         |
| regex_dna                | 212 ms                                                 | 210 ms: 1.01x faster                                         |
| sqlglot_transpile        | 1.68 ms                                                | 1.67 ms: 1.01x faster                                        |
| sqlglot_optimize         | 54.8 ms                                                | 54.3 ms: 1.01x faster                                        |
| sqlglot_parse            | 1.36 ms                                                | 1.35 ms: 1.01x faster                                        |
| sqlglot_normalize        | 110 ms                                                 | 111 ms: 1.00x slower                                         |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                       |
| async_tree_io            | 1.16 sec                                               | 1.16 sec: 1.01x slower                                       |
| create_gc_cycles         | 1.48 ms                                                | 1.51 ms: 1.02x slower                                        |
| gc_traversal             | 3.79 ms                                                | 3.91 ms: 1.03x slower                                        |
| asyncio_tcp              | 491 ms                                                 | 515 ms: 1.05x slower                                         |
| pidigits                 | 187 ms                                                 | 201 ms: 1.07x slower                                         |
| coverage                 | 72.7 ms                                                | 94.3 ms: 1.30x slower                                        |
| dask                     | 372 ms                                                 | 537 ms: 1.44x slower                                         |
| Geometric mean           | (ref)                                                  | 1.03x faster                                                 |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_none, dulwich_log, bench_mp_pool
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x