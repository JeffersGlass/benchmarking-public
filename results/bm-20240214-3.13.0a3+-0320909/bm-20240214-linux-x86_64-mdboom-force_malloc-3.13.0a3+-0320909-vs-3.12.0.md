
# Results vs. 3.12.0

- fork: mdboom
- ref: force_malloc
- machine: linux-x86_64
- commit hash: 0320909
- commit date: 2024-02-14
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 262 ms: 1.05x faster                                           |
| chameleon      | 7.41 ms                                                | 6.82 ms: 1.09x faster                                          |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                         |
| tornado_http   | 103 ms                                                 | 94.8 ms: 1.08x faster                                          |
| Geometric mean | (ref)                                                  | 1.07x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 424 ms: 1.11x faster                                           |
| async_tree_none_tg         | 450 ms                                                 | 427 ms: 1.05x faster                                           |
| async_tree_memoization     | 578 ms                                                 | 553 ms: 1.04x faster                                           |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 697 ms: 1.04x faster                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 703 ms: 1.03x faster                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 557 ms: 1.03x faster                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.17 sec: 1.01x faster                                         |
| async_tree_io              | 1.16 sec                                               | 1.15 sec: 1.01x faster                                         |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 84.7 ms                                                | 76.2 ms: 1.11x faster                                          |
| nbody          | 97.0 ms                                                | 91.9 ms: 1.06x faster                                          |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                           |
| Geometric mean | (ref)                                                  | 1.06x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 127 ms: 1.17x faster                                           |
| regex_effbot   | 3.61 ms                                                | 3.67 ms: 1.02x slower                                          |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                           |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                          |
| Geometric mean | (ref)                                                  | 1.00x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 291 us: 1.11x faster                                           |
| tomli_loads          | 2.33 sec                                               | 2.13 sec: 1.10x faster                                         |
| unpickle_pure_python | 230 us                                                 | 212 us: 1.08x faster                                           |
| unpickle_list        | 5.29 us                                                | 4.89 us: 1.08x faster                                          |
| xml_etree_process    | 61.7 ms                                                | 57.9 ms: 1.07x faster                                          |
| xml_etree_generate   | 89.2 ms                                                | 84.5 ms: 1.05x faster                                          |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                          |
| unpickle             | 15.9 us                                                | 15.4 us: 1.03x faster                                          |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                           |
| pickle_dict          | 35.5 us                                                | 34.7 us: 1.02x faster                                          |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.02x faster                                           |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                          |
| pickle_list          | 5.08 us                                                | 5.13 us: 1.01x slower                                          |
| pickle               | 11.6 us                                                | 11.8 us: 1.01x slower                                          |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                          |
| python_startup_no_site | 6.94 ms                                                | 8.70 ms: 1.25x slower                                          |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.07x faster                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 108 us: 1.47x faster                                           |
| comprehensions             | 21.8 us                                                | 15.9 us: 1.37x faster                                          |
| raytrace                   | 312 ms                                                 | 258 ms: 1.21x faster                                           |
| logging_format             | 7.23 us                                                | 6.09 us: 1.19x faster                                          |
| deltablue                  | 3.72 ms                                                | 3.16 ms: 1.18x faster                                          |
| regex_compile              | 148 ms                                                 | 127 ms: 1.17x faster                                           |
| logging_simple             | 6.46 us                                                | 5.56 us: 1.16x faster                                          |
| crypto_pyaes               | 81.9 ms                                                | 70.6 ms: 1.16x faster                                          |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                           |
| deepcopy_reduce            | 3.35 us                                                | 2.95 us: 1.14x faster                                          |
| scimark_monte_carlo        | 75.1 ms                                                | 66.3 ms: 1.13x faster                                          |
| sympy_str                  | 300 ms                                                 | 266 ms: 1.13x faster                                           |
| chaos                      | 67.0 ms                                                | 59.5 ms: 1.12x faster                                          |
| async_tree_none            | 472 ms                                                 | 424 ms: 1.11x faster                                           |
| pickle_pure_python         | 324 us                                                 | 291 us: 1.11x faster                                           |
| float                      | 84.7 ms                                                | 76.2 ms: 1.11x faster                                          |
| sympy_integrate            | 21.4 ms                                                | 19.4 ms: 1.11x faster                                          |
| scimark_sor                | 129 ms                                                 | 117 ms: 1.10x faster                                           |
| deepcopy                   | 371 us                                                 | 338 us: 1.10x faster                                           |
| logging_silent             | 104 ns                                                 | 95.2 ns: 1.10x faster                                          |
| deepcopy_memo              | 40.7 us                                                | 37.1 us: 1.10x faster                                          |
| tomli_loads                | 2.33 sec                                               | 2.13 sec: 1.10x faster                                         |
| fannkuch                   | 417 ms                                                 | 381 ms: 1.10x faster                                           |
| sqlglot_parse              | 1.36 ms                                                | 1.25 ms: 1.09x faster                                          |
| chameleon                  | 7.41 ms                                                | 6.82 ms: 1.09x faster                                          |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.66 ms: 1.09x faster                                          |
| unpack_sequence            | 54.0 ns                                                | 49.8 ns: 1.08x faster                                          |
| tornado_http               | 103 ms                                                 | 94.8 ms: 1.08x faster                                          |
| unpickle_pure_python       | 230 us                                                 | 212 us: 1.08x faster                                           |
| sqlglot_transpile          | 1.68 ms                                                | 1.56 ms: 1.08x faster                                          |
| unpickle_list              | 5.29 us                                                | 4.89 us: 1.08x faster                                          |
| scimark_fft                | 382 ms                                                 | 354 ms: 1.08x faster                                           |
| pyflate                    | 482 ms                                                 | 447 ms: 1.08x faster                                           |
| coroutines                 | 23.2 ms                                                | 21.5 ms: 1.08x faster                                          |
| pathlib                    | 19.3 ms                                                | 18.0 ms: 1.07x faster                                          |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.07x faster                                          |
| docutils                   | 2.77 sec                                               | 2.59 sec: 1.07x faster                                         |
| scimark_lu                 | 118 ms                                                 | 111 ms: 1.07x faster                                           |
| xml_etree_process          | 61.7 ms                                                | 57.9 ms: 1.07x faster                                          |
| hexiom                     | 6.41 ms                                                | 6.04 ms: 1.06x faster                                          |
| sympy_expand               | 478 ms                                                 | 451 ms: 1.06x faster                                           |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.06x faster                                           |
| pprint_safe_repr           | 776 ms                                                 | 732 ms: 1.06x faster                                           |
| generators                 | 31.2 ms                                                | 29.5 ms: 1.06x faster                                          |
| nbody                      | 97.0 ms                                                | 91.9 ms: 1.06x faster                                          |
| bench_thread_pool          | 842 us                                                 | 798 us: 1.05x faster                                           |
| xml_etree_generate         | 89.2 ms                                                | 84.5 ms: 1.05x faster                                          |
| async_tree_none_tg         | 450 ms                                                 | 427 ms: 1.05x faster                                           |
| pprint_pformat             | 1.57 sec                                               | 1.49 sec: 1.05x faster                                         |
| meteor_contest             | 112 ms                                                 | 107 ms: 1.05x faster                                           |
| dulwich_log                | 68.5 ms                                                | 65.2 ms: 1.05x faster                                          |
| mdp                        | 2.63 sec                                               | 2.51 sec: 1.05x faster                                         |
| 2to3                       | 274 ms                                                 | 262 ms: 1.05x faster                                           |
| sqlglot_normalize          | 110 ms                                                 | 105 ms: 1.05x faster                                           |
| async_generators           | 463 ms                                                 | 442 ms: 1.05x faster                                           |
| async_tree_memoization     | 578 ms                                                 | 553 ms: 1.04x faster                                           |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 697 ms: 1.04x faster                                           |
| json                       | 5.26 ms                                                | 5.08 ms: 1.04x faster                                          |
| dask                       | 372 ms                                                 | 360 ms: 1.03x faster                                           |
| nqueens                    | 83.3 ms                                                | 80.6 ms: 1.03x faster                                          |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 703 ms: 1.03x faster                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 557 ms: 1.03x faster                                           |
| go                         | 139 ms                                                 | 135 ms: 1.03x faster                                           |
| sqlglot_optimize           | 54.8 ms                                                | 53.2 ms: 1.03x faster                                          |
| json_loads                 | 28.5 us                                                | 27.7 us: 1.03x faster                                          |
| gc_traversal               | 3.79 ms                                                | 3.69 ms: 1.03x faster                                          |
| unpickle                   | 15.9 us                                                | 15.4 us: 1.03x faster                                          |
| xml_etree_parse            | 159 ms                                                 | 156 ms: 1.02x faster                                           |
| pickle_dict                | 35.5 us                                                | 34.7 us: 1.02x faster                                          |
| xml_etree_iterparse        | 107 ms                                                 | 104 ms: 1.02x faster                                           |
| pycparser                  | 1.18 sec                                               | 1.16 sec: 1.02x faster                                         |
| asyncio_tcp                | 491 ms                                                 | 484 ms: 1.01x faster                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.17 sec: 1.01x faster                                         |
| sqlite_synth               | 2.83 us                                                | 2.80 us: 1.01x faster                                          |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                          |
| async_tree_io              | 1.16 sec                                               | 1.15 sec: 1.01x faster                                         |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                           |
| json_dumps                 | 10.4 ms                                                | 10.4 ms: 1.00x slower                                          |
| pickle_list                | 5.08 us                                                | 5.13 us: 1.01x slower                                          |
| pickle                     | 11.6 us                                                | 11.8 us: 1.01x slower                                          |
| regex_effbot               | 3.61 ms                                                | 3.67 ms: 1.02x slower                                          |
| richards_super             | 51.5 ms                                                | 52.7 ms: 1.02x slower                                          |
| richards                   | 45.8 ms                                                | 47.0 ms: 1.02x slower                                          |
| regex_dna                  | 212 ms                                                 | 220 ms: 1.04x slower                                           |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                          |
| regex_v8                   | 23.1 ms                                                | 25.2 ms: 1.09x slower                                          |
| telco                      | 7.10 ms                                                | 8.35 ms: 1.18x slower                                          |
| python_startup_no_site     | 6.94 ms                                                | 8.70 ms: 1.25x slower                                          |
| coverage                   | 72.7 ms                                                | 95.9 ms: 1.32x slower                                          |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                   |

Benchmark hidden because not significant (4): asyncio_websockets, bench_mp_pool, asyncio_tcp_ssl, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.94x