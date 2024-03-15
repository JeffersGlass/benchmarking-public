
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0rc1
- machine: linux-x86_64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.35x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 267 ms: 1.30x faster                                         |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                       |
| tornado_http   | 136 ms                                                 | 99.1 ms: 1.38x faster                                        |
| Geometric mean | (ref)                                                  | 1.30x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 471 ms: 1.55x faster                                         |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                       |
| async_tree_memoization  | 870 ms                                                 | 573 ms: 1.52x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.43x faster                                         |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 89.6 ms: 1.71x faster                                        |
| float          | 117 ms                                                 | 79.3 ms: 1.48x faster                                        |
| pidigits       | 191 ms                                                 | 201 ms: 1.05x slower                                         |
| Geometric mean | (ref)                                                  | 1.34x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 145 ms: 1.30x faster                                         |
| regex_v8       | 27.8 ms                                                | 22.5 ms: 1.23x faster                                        |
| regex_dna      | 227 ms                                                 | 210 ms: 1.08x faster                                         |
| regex_effbot   | 3.63 ms                                                | 3.52 ms: 1.03x faster                                        |
| Geometric mean | (ref)                                                  | 1.16x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 311 us: 1.56x faster                                         |
| unpickle_pure_python | 331 us                                                 | 219 us: 1.51x faster                                         |
| json_dumps           | 14.2 ms                                                | 9.75 ms: 1.45x faster                                        |
| tomli_loads          | 3.14 sec                                               | 2.21 sec: 1.42x faster                                       |
| xml_etree_process    | 79.1 ms                                                | 59.2 ms: 1.34x faster                                        |
| json_loads           | 31.2 us                                                | 25.4 us: 1.23x faster                                        |
| xml_etree_generate   | 99.4 ms                                                | 85.4 ms: 1.16x faster                                        |
| pickle_list          | 5.08 us                                                | 4.55 us: 1.12x faster                                        |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                         |
| xml_etree_parse      | 168 ms                                                 | 155 ms: 1.09x faster                                         |
| unpickle_list        | 5.20 us                                                | 4.98 us: 1.04x faster                                        |
| pickle               | 10.7 us                                                | 10.8 us: 1.01x slower                                        |
| unpickle             | 14.4 us                                                | 14.9 us: 1.04x slower                                        |
| pickle_dict          | 29.6 us                                                | 31.4 us: 1.06x slower                                        |
| Geometric mean       | (ref)                                                  | 1.19x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.30 ms: 1.57x faster                                        |
| python_startup_no_site | 5.93 ms                                                | 6.76 ms: 1.14x slower                                        |
| Geometric mean         | (ref)                                                  | 1.17x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.7 ms: 1.53x faster                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 149 us: 3.64x faster                                         |
| generators               | 80.1 ms                                                | 30.2 ms: 2.65x faster                                        |
| deltablue                | 7.91 ms                                                | 3.55 ms: 2.23x faster                                        |
| richards_super           | 94.7 ms                                                | 50.3 ms: 1.88x faster                                        |
| logging_silent           | 190 ns                                                 | 102 ns: 1.85x faster                                         |
| chaos                    | 115 ms                                                 | 64.0 ms: 1.80x faster                                        |
| asyncio_tcp              | 922 ms                                                 | 515 ms: 1.79x faster                                         |
| richards                 | 79.3 ms                                                | 44.3 ms: 1.79x faster                                        |
| go                       | 240 ms                                                 | 135 ms: 1.77x faster                                         |
| scimark_sor              | 220 ms                                                 | 125 ms: 1.76x faster                                         |
| nbody                    | 154 ms                                                 | 89.6 ms: 1.71x faster                                        |
| raytrace                 | 507 ms                                                 | 297 ms: 1.70x faster                                         |
| hexiom                   | 10.4 ms                                                | 6.21 ms: 1.67x faster                                        |
| scimark_monte_carlo      | 118 ms                                                 | 71.7 ms: 1.65x faster                                        |
| crypto_pyaes             | 128 ms                                                 | 78.4 ms: 1.63x faster                                        |
| pyflate                  | 716 ms                                                 | 444 ms: 1.61x faster                                         |
| sqlglot_parse            | 2.17 ms                                                | 1.35 ms: 1.61x faster                                        |
| spectral_norm            | 170 ms                                                 | 107 ms: 1.59x faster                                         |
| deepcopy_memo            | 58.5 us                                                | 37.1 us: 1.58x faster                                        |
| python_startup           | 14.6 ms                                                | 9.30 ms: 1.57x faster                                        |
| pickle_pure_python       | 484 us                                                 | 311 us: 1.56x faster                                         |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.55x faster                                        |
| async_tree_none          | 728 ms                                                 | 471 ms: 1.55x faster                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                        |
| scimark_lu               | 176 ms                                                 | 114 ms: 1.54x faster                                         |
| mako                     | 16.3 ms                                                | 10.7 ms: 1.53x faster                                        |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                       |
| async_tree_memoization   | 870 ms                                                 | 573 ms: 1.52x faster                                         |
| unpickle_pure_python     | 331 us                                                 | 219 us: 1.51x faster                                         |
| float                    | 117 ms                                                 | 79.3 ms: 1.48x faster                                        |
| json_dumps               | 14.2 ms                                                | 9.75 ms: 1.45x faster                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.43x faster                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                       |
| tomli_loads              | 3.14 sec                                               | 2.21 sec: 1.42x faster                                       |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.41x faster                                       |
| comprehensions           | 28.8 us                                                | 20.7 us: 1.39x faster                                        |
| pprint_safe_repr         | 1.02 sec                                               | 737 ms: 1.38x faster                                         |
| pycparser                | 1.58 sec                                               | 1.14 sec: 1.38x faster                                       |
| tornado_http             | 136 ms                                                 | 99.1 ms: 1.38x faster                                        |
| deepcopy                 | 479 us                                                 | 355 us: 1.35x faster                                         |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                         |
| logging_simple           | 8.30 us                                                | 6.20 us: 1.34x faster                                        |
| xml_etree_process        | 79.1 ms                                                | 59.2 ms: 1.34x faster                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                        |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.89 ms: 1.32x faster                                        |
| scimark_fft              | 466 ms                                                 | 356 ms: 1.31x faster                                         |
| 2to3                     | 348 ms                                                 | 267 ms: 1.30x faster                                         |
| regex_compile            | 188 ms                                                 | 145 ms: 1.30x faster                                         |
| logging_format           | 9.09 us                                                | 6.99 us: 1.30x faster                                        |
| nqueens                  | 106 ms                                                 | 81.5 ms: 1.30x faster                                        |
| sqlglot_normalize        | 143 ms                                                 | 111 ms: 1.29x faster                                         |
| sqlglot_optimize         | 69.2 ms                                                | 54.3 ms: 1.27x faster                                        |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.4 ms: 1.27x faster                                        |
| regex_v8                 | 27.8 ms                                                | 22.5 ms: 1.23x faster                                        |
| dulwich_log              | 84.3 ms                                                | 68.5 ms: 1.23x faster                                        |
| json_loads               | 31.2 us                                                | 25.4 us: 1.23x faster                                        |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                       |
| json                     | 5.69 ms                                                | 4.77 ms: 1.19x faster                                        |
| sqlalchemy_declarative   | 172 ms                                                 | 145 ms: 1.19x faster                                         |
| bench_thread_pool        | 986 us                                                 | 832 us: 1.19x faster                                         |
| xml_etree_generate       | 99.4 ms                                                | 85.4 ms: 1.16x faster                                        |
| meteor_contest           | 120 ms                                                 | 105 ms: 1.14x faster                                         |
| unpack_sequence          | 60.0 ns                                                | 52.6 ns: 1.14x faster                                        |
| mdp                      | 2.85 sec                                               | 2.54 sec: 1.12x faster                                       |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                        |
| pickle_list              | 5.08 us                                                | 4.55 us: 1.12x faster                                        |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                         |
| sqlite_synth             | 3.02 us                                                | 2.75 us: 1.10x faster                                        |
| xml_etree_parse          | 168 ms                                                 | 155 ms: 1.09x faster                                         |
| regex_dna                | 227 ms                                                 | 210 ms: 1.08x faster                                         |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                        |
| telco                    | 7.27 ms                                                | 6.86 ms: 1.06x faster                                        |
| unpickle_list            | 5.20 us                                                | 4.98 us: 1.04x faster                                        |
| regex_effbot             | 3.63 ms                                                | 3.52 ms: 1.03x faster                                        |
| pickle                   | 10.7 us                                                | 10.8 us: 1.01x slower                                        |
| async_generators         | 444 ms                                                 | 450 ms: 1.01x slower                                         |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.04x slower                                        |
| pidigits                 | 191 ms                                                 | 201 ms: 1.05x slower                                         |
| pickle_dict              | 29.6 us                                                | 31.4 us: 1.06x slower                                        |
| gc_traversal             | 3.62 ms                                                | 3.91 ms: 1.08x slower                                        |
| python_startup_no_site   | 5.93 ms                                                | 6.76 ms: 1.14x slower                                        |
| coverage                 | 79.4 ms                                                | 94.3 ms: 1.19x slower                                        |
| dask                     | 441 ms                                                 | 537 ms: 1.22x slower                                         |
| Geometric mean           | (ref)                                                  | 1.35x faster                                                 |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (17) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.17x