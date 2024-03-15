
# Results vs. 3.12.0

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 262 ms: 1.05x faster                                      |
| chameleon      | 7.41 ms                                                | 6.68 ms: 1.11x faster                                     |
| docutils       | 2.77 sec                                               | 2.56 sec: 1.08x faster                                    |
| tornado_http   | 103 ms                                                 | 94.3 ms: 1.09x faster                                     |
| Geometric mean | (ref)                                                  | 1.08x faster                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                      |
| async_tree_memoization     | 578 ms                                                 | 555 ms: 1.04x faster                                      |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 701 ms: 1.04x faster                                      |
| async_tree_none_tg         | 450 ms                                                 | 442 ms: 1.02x faster                                      |
| async_tree_memoization_tg  | 575 ms                                                 | 565 ms: 1.02x faster                                      |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 714 ms: 1.02x faster                                      |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                    |
| Geometric mean             | (ref)                                                  | 1.03x faster                                              |

Benchmark hidden because not significant (1): async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.7 ms: 1.09x faster                                     |
| float          | 84.7 ms                                                | 79.2 ms: 1.07x faster                                     |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                      |
| Geometric mean | (ref)                                                  | 1.05x faster                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 127 ms: 1.17x faster                                      |
| regex_v8       | 23.1 ms                                                | 23.8 ms: 1.03x slower                                     |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                      |
| Geometric mean | (ref)                                                  | 1.02x faster                                              |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.09 sec: 1.12x faster                                    |
| pickle_pure_python   | 324 us                                                 | 293 us: 1.11x faster                                      |
| unpickle_pure_python | 230 us                                                 | 210 us: 1.10x faster                                      |
| xml_etree_process    | 61.7 ms                                                | 57.8 ms: 1.07x faster                                     |
| unpickle_list        | 5.29 us                                                | 4.98 us: 1.06x faster                                     |
| xml_etree_generate   | 89.2 ms                                                | 84.5 ms: 1.05x faster                                     |
| pickle_dict          | 35.5 us                                                | 34.0 us: 1.04x faster                                     |
| pickle_list          | 5.08 us                                                | 4.92 us: 1.03x faster                                     |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                      |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                      |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                     |
| pickle               | 11.6 us                                                | 11.6 us: 1.00x slower                                     |
| Geometric mean       | (ref)                                                  | 1.04x faster                                              |

Benchmark hidden because not significant (2): unpickle, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.06x slower                                     |
| python_startup_no_site | 6.94 ms                                                | 8.78 ms: 1.27x slower                                     |
| Geometric mean         | (ref)                                                  | 1.16x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.07x faster                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 108 us: 1.46x faster                                      |
| comprehensions             | 21.8 us                                                | 16.0 us: 1.36x faster                                     |
| raytrace                   | 312 ms                                                 | 260 ms: 1.20x faster                                      |
| logging_format             | 7.23 us                                                | 6.14 us: 1.18x faster                                     |
| regex_compile              | 148 ms                                                 | 127 ms: 1.17x faster                                      |
| deltablue                  | 3.72 ms                                                | 3.19 ms: 1.17x faster                                     |
| crypto_pyaes               | 81.9 ms                                                | 70.6 ms: 1.16x faster                                     |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                      |
| logging_simple             | 6.46 us                                                | 5.61 us: 1.15x faster                                     |
| chaos                      | 67.0 ms                                                | 58.8 ms: 1.14x faster                                     |
| scimark_monte_carlo        | 75.1 ms                                                | 65.9 ms: 1.14x faster                                     |
| sympy_str                  | 300 ms                                                 | 264 ms: 1.14x faster                                      |
| deepcopy_reduce            | 3.35 us                                                | 2.99 us: 1.12x faster                                     |
| deepcopy_memo              | 40.7 us                                                | 36.4 us: 1.12x faster                                     |
| tomli_loads                | 2.33 sec                                               | 2.09 sec: 1.12x faster                                    |
| chameleon                  | 7.41 ms                                                | 6.68 ms: 1.11x faster                                     |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.56 ms: 1.11x faster                                     |
| pickle_pure_python         | 324 us                                                 | 293 us: 1.11x faster                                      |
| sympy_integrate            | 21.4 ms                                                | 19.4 ms: 1.11x faster                                     |
| logging_silent             | 104 ns                                                 | 94.7 ns: 1.10x faster                                     |
| deepcopy                   | 371 us                                                 | 338 us: 1.10x faster                                      |
| sqlglot_parse              | 1.36 ms                                                | 1.24 ms: 1.10x faster                                     |
| unpickle_pure_python       | 230 us                                                 | 210 us: 1.10x faster                                      |
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                      |
| nbody                      | 97.0 ms                                                | 88.7 ms: 1.09x faster                                     |
| tornado_http               | 103 ms                                                 | 94.3 ms: 1.09x faster                                     |
| scimark_fft                | 382 ms                                                 | 352 ms: 1.09x faster                                      |
| sqlglot_transpile          | 1.68 ms                                                | 1.55 ms: 1.08x faster                                     |
| hexiom                     | 6.41 ms                                                | 5.91 ms: 1.08x faster                                     |
| docutils                   | 2.77 sec                                               | 2.56 sec: 1.08x faster                                    |
| generators                 | 31.2 ms                                                | 28.9 ms: 1.08x faster                                     |
| unpack_sequence            | 54.0 ns                                                | 50.1 ns: 1.08x faster                                     |
| pprint_safe_repr           | 776 ms                                                 | 721 ms: 1.08x faster                                      |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.07x faster                                     |
| fannkuch                   | 417 ms                                                 | 390 ms: 1.07x faster                                      |
| pprint_pformat             | 1.57 sec                                               | 1.47 sec: 1.07x faster                                    |
| sympy_expand               | 478 ms                                                 | 447 ms: 1.07x faster                                      |
| float                      | 84.7 ms                                                | 79.2 ms: 1.07x faster                                     |
| nqueens                    | 83.3 ms                                                | 77.9 ms: 1.07x faster                                     |
| pathlib                    | 19.3 ms                                                | 18.1 ms: 1.07x faster                                     |
| xml_etree_process          | 61.7 ms                                                | 57.8 ms: 1.07x faster                                     |
| unpickle_list              | 5.29 us                                                | 4.98 us: 1.06x faster                                     |
| scimark_lu                 | 118 ms                                                 | 111 ms: 1.06x faster                                      |
| sqlglot_normalize          | 110 ms                                                 | 104 ms: 1.06x faster                                      |
| xml_etree_generate         | 89.2 ms                                                | 84.5 ms: 1.05x faster                                     |
| dulwich_log                | 68.5 ms                                                | 65.1 ms: 1.05x faster                                     |
| meteor_contest             | 112 ms                                                 | 107 ms: 1.05x faster                                      |
| 2to3                       | 274 ms                                                 | 262 ms: 1.05x faster                                      |
| pickle_dict                | 35.5 us                                                | 34.0 us: 1.04x faster                                     |
| spectral_norm              | 115 ms                                                 | 110 ms: 1.04x faster                                      |
| async_tree_memoization     | 578 ms                                                 | 555 ms: 1.04x faster                                      |
| sqlglot_optimize           | 54.8 ms                                                | 52.9 ms: 1.04x faster                                     |
| dask                       | 372 ms                                                 | 359 ms: 1.04x faster                                      |
| pyflate                    | 482 ms                                                 | 466 ms: 1.04x faster                                      |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 701 ms: 1.04x faster                                      |
| async_generators           | 463 ms                                                 | 448 ms: 1.03x faster                                      |
| pickle_list                | 5.08 us                                                | 4.92 us: 1.03x faster                                     |
| json                       | 5.26 ms                                                | 5.10 ms: 1.03x faster                                     |
| coroutines                 | 23.2 ms                                                | 22.5 ms: 1.03x faster                                     |
| bench_thread_pool          | 842 us                                                 | 816 us: 1.03x faster                                      |
| pycparser                  | 1.18 sec                                               | 1.15 sec: 1.03x faster                                    |
| sqlite_synth               | 2.83 us                                                | 2.77 us: 1.02x faster                                     |
| xml_etree_parse            | 159 ms                                                 | 156 ms: 1.02x faster                                      |
| xml_etree_iterparse        | 107 ms                                                 | 105 ms: 1.02x faster                                      |
| async_tree_none_tg         | 450 ms                                                 | 442 ms: 1.02x faster                                      |
| async_tree_memoization_tg  | 575 ms                                                 | 565 ms: 1.02x faster                                      |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 714 ms: 1.02x faster                                      |
| asyncio_tcp                | 491 ms                                                 | 484 ms: 1.01x faster                                      |
| json_loads                 | 28.5 us                                                | 28.3 us: 1.01x faster                                     |
| go                         | 139 ms                                                 | 139 ms: 1.01x faster                                      |
| gc_traversal               | 3.79 ms                                                | 3.78 ms: 1.00x faster                                     |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                      |
| pickle                     | 11.6 us                                                | 11.6 us: 1.00x slower                                     |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                    |
| create_gc_cycles           | 1.48 ms                                                | 1.50 ms: 1.02x slower                                     |
| richards                   | 45.8 ms                                                | 46.7 ms: 1.02x slower                                     |
| richards_super             | 51.5 ms                                                | 52.8 ms: 1.03x slower                                     |
| regex_v8                   | 23.1 ms                                                | 23.8 ms: 1.03x slower                                     |
| mdp                        | 2.63 sec                                               | 2.72 sec: 1.03x slower                                    |
| regex_dna                  | 212 ms                                                 | 223 ms: 1.05x slower                                      |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.06x slower                                     |
| telco                      | 7.10 ms                                                | 8.23 ms: 1.16x slower                                     |
| python_startup_no_site     | 6.94 ms                                                | 8.78 ms: 1.27x slower                                     |
| coverage                   | 72.7 ms                                                | 95.2 ms: 1.31x slower                                     |
| Geometric mean             | (ref)                                                  | 1.05x faster                                              |

Benchmark hidden because not significant (9): unpickle, scimark_sor, json_dumps, regex_effbot, asyncio_tcp_ssl, bench_mp_pool, async_tree_io_tg, asyncio_websockets, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x