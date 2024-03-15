
# Results vs. 3.12.0

- fork: mdboom
- ref: faster_negate
- machine: linux-x86_64
- commit hash: 34fc24a
- commit date: 2024-01-04
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 265 ms: 1.04x faster                                            |
| chameleon      | 7.41 ms                                                | 6.87 ms: 1.08x faster                                           |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                          |
| tornado_http   | 103 ms                                                 | 94.2 ms: 1.09x faster                                           |
| Geometric mean | (ref)                                                  | 1.07x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 434 ms: 1.09x faster                                            |
| async_tree_memoization  | 578 ms                                                 | 558 ms: 1.03x faster                                            |
| async_tree_cpu_io_mixed | 726 ms                                                 | 703 ms: 1.03x faster                                            |
| async_tree_none_tg      | 450 ms                                                 | 441 ms: 1.02x faster                                            |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.01x slower                                          |
| async_tree_io           | 1.16 sec                                               | 1.17 sec: 1.02x slower                                          |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                    |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 90.1 ms: 1.08x faster                                           |
| float          | 84.7 ms                                                | 80.3 ms: 1.05x faster                                           |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                            |
| Geometric mean | (ref)                                                  | 1.04x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 130 ms: 1.14x faster                                            |
| regex_effbot   | 3.61 ms                                                | 3.64 ms: 1.01x slower                                           |
| regex_dna      | 212 ms                                                 | 225 ms: 1.06x slower                                            |
| regex_v8       | 23.1 ms                                                | 25.0 ms: 1.08x slower                                           |
| Geometric mean | (ref)                                                  | 1.00x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.18 sec: 1.07x faster                                          |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                            |
| unpickle_pure_python | 230 us                                                 | 219 us: 1.05x faster                                            |
| xml_etree_process    | 61.7 ms                                                | 58.9 ms: 1.05x faster                                           |
| xml_etree_generate   | 89.2 ms                                                | 85.8 ms: 1.04x faster                                           |
| pickle_dict          | 35.5 us                                                | 34.2 us: 1.04x faster                                           |
| pickle_list          | 5.08 us                                                | 4.90 us: 1.04x faster                                           |
| unpickle_list        | 5.29 us                                                | 5.10 us: 1.04x faster                                           |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                           |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                            |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                           |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.02x slower                                           |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                    |

Benchmark hidden because not significant (2): unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                           |
| python_startup_no_site | 6.94 ms                                                | 8.73 ms: 1.26x slower                                           |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.2 ms: 1.06x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 109 us: 1.45x faster                                            |
| comprehensions           | 21.8 us                                                | 16.4 us: 1.33x faster                                           |
| unpack_sequence          | 54.0 ns                                                | 44.1 ns: 1.22x faster                                           |
| raytrace                 | 312 ms                                                 | 261 ms: 1.20x faster                                            |
| logging_format           | 7.23 us                                                | 6.19 us: 1.17x faster                                           |
| logging_simple           | 6.46 us                                                | 5.58 us: 1.16x faster                                           |
| sympy_sum                | 169 ms                                                 | 148 ms: 1.15x faster                                            |
| deltablue                | 3.72 ms                                                | 3.25 ms: 1.14x faster                                           |
| crypto_pyaes             | 81.9 ms                                                | 71.8 ms: 1.14x faster                                           |
| regex_compile            | 148 ms                                                 | 130 ms: 1.14x faster                                            |
| sympy_str                | 300 ms                                                 | 268 ms: 1.12x faster                                            |
| chaos                    | 67.0 ms                                                | 60.1 ms: 1.11x faster                                           |
| scimark_monte_carlo      | 75.1 ms                                                | 68.4 ms: 1.10x faster                                           |
| sympy_integrate          | 21.4 ms                                                | 19.5 ms: 1.10x faster                                           |
| sqlglot_parse            | 1.36 ms                                                | 1.24 ms: 1.09x faster                                           |
| tornado_http             | 103 ms                                                 | 94.2 ms: 1.09x faster                                           |
| async_tree_none          | 472 ms                                                 | 434 ms: 1.09x faster                                            |
| deepcopy_reduce          | 3.35 us                                                | 3.08 us: 1.09x faster                                           |
| sqlglot_transpile        | 1.68 ms                                                | 1.56 ms: 1.08x faster                                           |
| chameleon                | 7.41 ms                                                | 6.87 ms: 1.08x faster                                           |
| nbody                    | 97.0 ms                                                | 90.1 ms: 1.08x faster                                           |
| deepcopy                 | 371 us                                                 | 346 us: 1.07x faster                                            |
| tomli_loads              | 2.33 sec                                               | 2.18 sec: 1.07x faster                                          |
| docutils                 | 2.77 sec                                               | 2.59 sec: 1.07x faster                                          |
| pickle_pure_python       | 324 us                                                 | 305 us: 1.06x faster                                            |
| pathlib                  | 19.3 ms                                                | 18.2 ms: 1.06x faster                                           |
| mako                     | 11.9 ms                                                | 11.2 ms: 1.06x faster                                           |
| generators               | 31.2 ms                                                | 29.5 ms: 1.06x faster                                           |
| pyflate                  | 482 ms                                                 | 456 ms: 1.06x faster                                            |
| deepcopy_memo            | 40.7 us                                                | 38.6 us: 1.06x faster                                           |
| float                    | 84.7 ms                                                | 80.3 ms: 1.05x faster                                           |
| pprint_safe_repr         | 776 ms                                                 | 737 ms: 1.05x faster                                            |
| dulwich_log              | 68.5 ms                                                | 65.1 ms: 1.05x faster                                           |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                            |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                            |
| coroutines               | 23.2 ms                                                | 22.1 ms: 1.05x faster                                           |
| scimark_fft              | 382 ms                                                 | 364 ms: 1.05x faster                                            |
| unpickle_pure_python     | 230 us                                                 | 219 us: 1.05x faster                                            |
| xml_etree_process        | 61.7 ms                                                | 58.9 ms: 1.05x faster                                           |
| sympy_expand             | 478 ms                                                 | 457 ms: 1.05x faster                                            |
| pprint_pformat           | 1.57 sec                                               | 1.50 sec: 1.05x faster                                          |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                            |
| async_generators         | 463 ms                                                 | 445 ms: 1.04x faster                                            |
| xml_etree_generate       | 89.2 ms                                                | 85.8 ms: 1.04x faster                                           |
| pickle_dict              | 35.5 us                                                | 34.2 us: 1.04x faster                                           |
| 2to3                     | 274 ms                                                 | 265 ms: 1.04x faster                                            |
| pickle_list              | 5.08 us                                                | 4.90 us: 1.04x faster                                           |
| unpickle_list            | 5.29 us                                                | 5.10 us: 1.04x faster                                           |
| async_tree_memoization   | 578 ms                                                 | 558 ms: 1.03x faster                                            |
| fannkuch                 | 417 ms                                                 | 403 ms: 1.03x faster                                            |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 703 ms: 1.03x faster                                            |
| dask                     | 372 ms                                                 | 360 ms: 1.03x faster                                            |
| gc_traversal             | 3.79 ms                                                | 3.70 ms: 1.03x faster                                           |
| sqlglot_optimize         | 54.8 ms                                                | 53.5 ms: 1.02x faster                                           |
| mdp                      | 2.63 sec                                               | 2.57 sec: 1.02x faster                                          |
| hexiom                   | 6.41 ms                                                | 6.29 ms: 1.02x faster                                           |
| async_tree_none_tg       | 450 ms                                                 | 441 ms: 1.02x faster                                            |
| pickle                   | 11.6 us                                                | 11.4 us: 1.02x faster                                           |
| xml_etree_iterparse      | 107 ms                                                 | 105 ms: 1.02x faster                                            |
| bench_thread_pool        | 842 us                                                 | 830 us: 1.01x faster                                            |
| asyncio_tcp              | 491 ms                                                 | 484 ms: 1.01x faster                                            |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.00 ms: 1.01x faster                                           |
| logging_silent           | 104 ns                                                 | 103 ns: 1.01x faster                                            |
| pycparser                | 1.18 sec                                               | 1.17 sec: 1.01x faster                                          |
| json_loads               | 28.5 us                                                | 28.3 us: 1.01x faster                                           |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.78 sec: 1.00x faster                                          |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                            |
| create_gc_cycles         | 1.48 ms                                                | 1.48 ms: 1.00x slower                                           |
| nqueens                  | 83.3 ms                                                | 83.9 ms: 1.01x slower                                           |
| regex_effbot             | 3.61 ms                                                | 3.64 ms: 1.01x slower                                           |
| sqlite_synth             | 2.83 us                                                | 2.86 us: 1.01x slower                                           |
| go                       | 139 ms                                                 | 141 ms: 1.01x slower                                            |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                          |
| scimark_sor              | 129 ms                                                 | 130 ms: 1.01x slower                                            |
| json_dumps               | 10.4 ms                                                | 10.5 ms: 1.02x slower                                           |
| async_tree_io            | 1.16 sec                                               | 1.17 sec: 1.02x slower                                          |
| richards                 | 45.8 ms                                                | 47.2 ms: 1.03x slower                                           |
| richards_super           | 51.5 ms                                                | 53.7 ms: 1.04x slower                                           |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                           |
| regex_dna                | 212 ms                                                 | 225 ms: 1.06x slower                                            |
| regex_v8                 | 23.1 ms                                                | 25.0 ms: 1.08x slower                                           |
| telco                    | 7.10 ms                                                | 8.42 ms: 1.19x slower                                           |
| python_startup_no_site   | 6.94 ms                                                | 8.73 ms: 1.26x slower                                           |
| coverage                 | 72.7 ms                                                | 97.0 ms: 1.33x slower                                           |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                    |

Benchmark hidden because not significant (9): unpickle, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, bench_mp_pool, asyncio_websockets, json, spectral_norm, xml_etree_parse, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.93x