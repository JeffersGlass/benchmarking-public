
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0rc1
- machine: linux-x86_64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.49%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 267 ms: 1.01x slower                                         |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                       |
| tornado_http   | 98.1 ms                                                | 99.1 ms: 1.01x slower                                        |
| Geometric mean | (ref)                                                  | 1.01x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_none         | 528 ms                                                 | 471 ms: 1.12x faster                                         |
| async_tree_memoization  | 639 ms                                                 | 573 ms: 1.11x faster                                         |
| async_tree_io           | 1.29 sec                                               | 1.16 sec: 1.11x faster                                       |
| async_tree_cpu_io_mixed | 749 ms                                                 | 708 ms: 1.06x faster                                         |
| Geometric mean          | (ref)                                                  | 1.10x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 89.6 ms: 1.07x faster                                        |
| float          | 78.9 ms                                                | 79.3 ms: 1.00x slower                                        |
| pidigits       | 194 ms                                                 | 201 ms: 1.03x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 22.5 ms: 1.02x faster                                        |
| regex_effbot   | 3.51 ms                                                | 3.52 ms: 1.00x slower                                        |
| regex_dna      | 205 ms                                                 | 210 ms: 1.03x slower                                         |
| regex_compile  | 141 ms                                                 | 145 ms: 1.03x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.75 ms: 1.37x faster                                        |
| json_loads           | 29.2 us                                                | 25.4 us: 1.15x faster                                        |
| pickle_dict          | 34.6 us                                                | 31.4 us: 1.10x faster                                        |
| unpickle_pure_python | 242 us                                                 | 219 us: 1.10x faster                                         |
| xml_etree_parse      | 164 ms                                                 | 155 ms: 1.06x faster                                         |
| unpickle_list        | 5.21 us                                                | 4.98 us: 1.05x faster                                        |
| tomli_loads          | 2.30 sec                                               | 2.21 sec: 1.04x faster                                       |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                         |
| pickle_pure_python   | 320 us                                                 | 311 us: 1.03x faster                                         |
| pickle               | 11.0 us                                                | 10.8 us: 1.02x faster                                        |
| pickle_list          | 4.59 us                                                | 4.55 us: 1.01x faster                                        |
| xml_etree_process    | 56.9 ms                                                | 59.2 ms: 1.04x slower                                        |
| xml_etree_generate   | 81.1 ms                                                | 85.4 ms: 1.05x slower                                        |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                        |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.30 ms: 1.09x slower                                        |
| python_startup_no_site | 6.01 ms                                                | 6.76 ms: 1.12x slower                                        |
| Geometric mean         | (ref)                                                  | 1.11x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.7 ms: 1.00x slower                                        |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-linux-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols | 520 us                                                 | 149 us: 3.48x faster                                         |
| generators               | 74.9 ms                                                | 30.2 ms: 2.48x faster                                        |
| asyncio_tcp_ssl          | 3.11 sec                                               | 1.80 sec: 1.73x faster                                       |
| asyncio_tcp              | 875 ms                                                 | 515 ms: 1.70x faster                                         |
| json_dumps               | 13.3 ms                                                | 9.75 ms: 1.37x faster                                        |
| richards_super           | 61.9 ms                                                | 50.3 ms: 1.23x faster                                        |
| coroutines               | 27.0 ms                                                | 22.7 ms: 1.19x faster                                        |
| json_loads               | 29.2 us                                                | 25.4 us: 1.15x faster                                        |
| comprehensions           | 23.6 us                                                | 20.7 us: 1.14x faster                                        |
| richards                 | 49.8 ms                                                | 44.3 ms: 1.12x faster                                        |
| chaos                    | 71.9 ms                                                | 64.0 ms: 1.12x faster                                        |
| async_tree_none          | 528 ms                                                 | 471 ms: 1.12x faster                                         |
| async_tree_memoization   | 639 ms                                                 | 573 ms: 1.11x faster                                         |
| hexiom                   | 6.89 ms                                                | 6.21 ms: 1.11x faster                                        |
| async_tree_io            | 1.29 sec                                               | 1.16 sec: 1.11x faster                                       |
| deltablue                | 3.92 ms                                                | 3.55 ms: 1.10x faster                                        |
| pickle_dict              | 34.6 us                                                | 31.4 us: 1.10x faster                                        |
| unpickle_pure_python     | 242 us                                                 | 219 us: 1.10x faster                                         |
| json                     | 5.24 ms                                                | 4.77 ms: 1.10x faster                                        |
| go                       | 149 ms                                                 | 135 ms: 1.10x faster                                         |
| mdp                      | 2.77 sec                                               | 2.54 sec: 1.09x faster                                       |
| logging_silent           | 111 ns                                                 | 102 ns: 1.08x faster                                         |
| deepcopy_memo            | 40.2 us                                                | 37.1 us: 1.08x faster                                        |
| nqueens                  | 87.9 ms                                                | 81.5 ms: 1.08x faster                                        |
| nbody                    | 96.0 ms                                                | 89.6 ms: 1.07x faster                                        |
| sqlglot_parse            | 1.43 ms                                                | 1.35 ms: 1.06x faster                                        |
| xml_etree_parse          | 164 ms                                                 | 155 ms: 1.06x faster                                         |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 708 ms: 1.06x faster                                         |
| sqlglot_transpile        | 1.75 ms                                                | 1.67 ms: 1.05x faster                                        |
| unpickle_list            | 5.21 us                                                | 4.98 us: 1.05x faster                                        |
| meteor_contest           | 109 ms                                                 | 105 ms: 1.04x faster                                         |
| tomli_loads              | 2.30 sec                                               | 2.21 sec: 1.04x faster                                       |
| pprint_pformat           | 1.55 sec                                               | 1.50 sec: 1.04x faster                                       |
| xml_etree_iterparse      | 108 ms                                                 | 104 ms: 1.04x faster                                         |
| raytrace                 | 309 ms                                                 | 297 ms: 1.04x faster                                         |
| pycparser                | 1.19 sec                                               | 1.14 sec: 1.04x faster                                       |
| pickle_pure_python       | 320 us                                                 | 311 us: 1.03x faster                                         |
| deepcopy                 | 365 us                                                 | 355 us: 1.03x faster                                         |
| fannkuch                 | 405 ms                                                 | 394 ms: 1.03x faster                                         |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.89 ms: 1.03x faster                                        |
| gc_traversal             | 4.01 ms                                                | 3.91 ms: 1.03x faster                                        |
| deepcopy_reduce          | 3.22 us                                                | 3.14 us: 1.02x faster                                        |
| pickle                   | 11.0 us                                                | 10.8 us: 1.02x faster                                        |
| sqlglot_optimize         | 55.3 ms                                                | 54.3 ms: 1.02x faster                                        |
| scimark_lu               | 116 ms                                                 | 114 ms: 1.02x faster                                         |
| sqlglot_normalize        | 113 ms                                                 | 111 ms: 1.02x faster                                         |
| regex_v8                 | 22.9 ms                                                | 22.5 ms: 1.02x faster                                        |
| pathlib                  | 18.5 ms                                                | 18.3 ms: 1.01x faster                                        |
| pprint_safe_repr         | 747 ms                                                 | 737 ms: 1.01x faster                                         |
| spectral_norm            | 108 ms                                                 | 107 ms: 1.01x faster                                         |
| pickle_list              | 4.59 us                                                | 4.55 us: 1.01x faster                                        |
| bench_thread_pool        | 834 us                                                 | 832 us: 1.00x faster                                         |
| mako                     | 10.7 ms                                                | 10.7 ms: 1.00x slower                                        |
| regex_effbot             | 3.51 ms                                                | 3.52 ms: 1.00x slower                                        |
| float                    | 78.9 ms                                                | 79.3 ms: 1.00x slower                                        |
| tornado_http             | 98.1 ms                                                | 99.1 ms: 1.01x slower                                        |
| 2to3                     | 264 ms                                                 | 267 ms: 1.01x slower                                         |
| scimark_monte_carlo      | 70.7 ms                                                | 71.7 ms: 1.01x slower                                        |
| docutils                 | 2.66 sec                                               | 2.70 sec: 1.01x slower                                       |
| crypto_pyaes             | 76.7 ms                                                | 78.4 ms: 1.02x slower                                        |
| pyflate                  | 434 ms                                                 | 444 ms: 1.02x slower                                         |
| regex_dna                | 205 ms                                                 | 210 ms: 1.03x slower                                         |
| regex_compile            | 141 ms                                                 | 145 ms: 1.03x slower                                         |
| logging_format           | 6.81 us                                                | 6.99 us: 1.03x slower                                        |
| scimark_sor              | 121 ms                                                 | 125 ms: 1.03x slower                                         |
| sqlalchemy_declarative   | 140 ms                                                 | 145 ms: 1.03x slower                                         |
| scimark_fft              | 345 ms                                                 | 356 ms: 1.03x slower                                         |
| pidigits                 | 194 ms                                                 | 201 ms: 1.03x slower                                         |
| xml_etree_process        | 56.9 ms                                                | 59.2 ms: 1.04x slower                                        |
| xml_etree_generate       | 81.1 ms                                                | 85.4 ms: 1.05x slower                                        |
| create_gc_cycles         | 1.43 ms                                                | 1.51 ms: 1.05x slower                                        |
| dulwich_log              | 64.6 ms                                                | 68.5 ms: 1.06x slower                                        |
| sqlite_synth             | 2.57 us                                                | 2.75 us: 1.07x slower                                        |
| unpickle                 | 13.8 us                                                | 14.9 us: 1.08x slower                                        |
| python_startup           | 8.56 ms                                                | 9.30 ms: 1.09x slower                                        |
| python_startup_no_site   | 6.01 ms                                                | 6.76 ms: 1.12x slower                                        |
| coverage                 | 78.8 ms                                                | 94.3 ms: 1.20x slower                                        |
| async_generators         | 374 ms                                                 | 450 ms: 1.20x slower                                         |
| unpack_sequence          | 43.5 ns                                                | 52.6 ns: 1.21x slower                                        |
| dask                     | 365 ms                                                 | 537 ms: 1.47x slower                                         |
| Geometric mean           | (ref)                                                  | 1.06x faster                                                 |

Benchmark hidden because not significant (4): logging_simple, telco, bench_mp_pool, sqlalchemy_imperative
Ignored benchmarks (21) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.49% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.10x