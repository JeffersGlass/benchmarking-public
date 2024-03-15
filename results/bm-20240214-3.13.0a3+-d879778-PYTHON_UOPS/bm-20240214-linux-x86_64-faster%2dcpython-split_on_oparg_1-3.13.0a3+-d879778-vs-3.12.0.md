
# Results vs. 3.12.0

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: d879778
- commit date: 2024-02-14
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.94%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 284 ms: 1.03x slower                                                         |
| chameleon      | 7.41 ms                                                | 7.01 ms: 1.06x faster                                                        |
| docutils       | 2.77 sec                                               | 2.68 sec: 1.03x faster                                                       |
| tornado_http   | 103 ms                                                 | 98.0 ms: 1.05x faster                                                        |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 448 ms: 1.05x faster                                                         |
| async_tree_memoization     | 578 ms                                                 | 569 ms: 1.02x faster                                                         |
| async_tree_none_tg         | 450 ms                                                 | 453 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 733 ms: 1.01x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 584 ms: 1.02x slower                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                       |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                       |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                         |
| float          | 84.7 ms                                                | 93.5 ms: 1.10x slower                                                        |
| nbody          | 97.0 ms                                                | 121 ms: 1.25x slower                                                         |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 150 ms: 1.01x slower                                                         |
| regex_effbot   | 3.61 ms                                                | 3.75 ms: 1.04x slower                                                        |
| regex_dna      | 212 ms                                                 | 228 ms: 1.08x slower                                                         |
| regex_v8       | 23.1 ms                                                | 26.3 ms: 1.14x slower                                                        |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                         |
| unpickle_list        | 5.29 us                                                | 4.97 us: 1.06x faster                                                        |
| json_loads           | 28.5 us                                                | 27.5 us: 1.04x faster                                                        |
| unpickle             | 15.9 us                                                | 15.4 us: 1.03x faster                                                        |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                                        |
| xml_etree_process    | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                        |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                         |
| xml_etree_generate   | 89.2 ms                                                | 88.8 ms: 1.00x faster                                                        |
| unpickle_pure_python | 230 us                                                 | 232 us: 1.01x slower                                                         |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                         |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                                        |
| pickle               | 11.6 us                                                | 12.0 us: 1.03x slower                                                        |
| tomli_loads          | 2.33 sec                                               | 2.61 sec: 1.12x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.3 ms: 1.07x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 8.88 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.9 ms: 1.17x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 115 us: 1.37x faster                                                         |
| unpack_sequence            | 54.0 ns                                                | 42.9 ns: 1.26x faster                                                        |
| pickle_pure_python         | 324 us                                                 | 299 us: 1.08x faster                                                         |
| generators                 | 31.2 ms                                                | 29.1 ms: 1.07x faster                                                        |
| comprehensions             | 21.8 us                                                | 20.3 us: 1.07x faster                                                        |
| logging_format             | 7.23 us                                                | 6.76 us: 1.07x faster                                                        |
| logging_simple             | 6.46 us                                                | 6.05 us: 1.07x faster                                                        |
| sympy_sum                  | 169 ms                                                 | 159 ms: 1.07x faster                                                         |
| deepcopy_reduce            | 3.35 us                                                | 3.14 us: 1.07x faster                                                        |
| unpickle_list              | 5.29 us                                                | 4.97 us: 1.06x faster                                                        |
| deltablue                  | 3.72 ms                                                | 3.50 ms: 1.06x faster                                                        |
| chameleon                  | 7.41 ms                                                | 7.01 ms: 1.06x faster                                                        |
| async_tree_none            | 472 ms                                                 | 448 ms: 1.05x faster                                                         |
| tornado_http               | 103 ms                                                 | 98.0 ms: 1.05x faster                                                        |
| raytrace                   | 312 ms                                                 | 298 ms: 1.05x faster                                                         |
| pathlib                    | 19.3 ms                                                | 18.5 ms: 1.04x faster                                                        |
| scimark_sor                | 129 ms                                                 | 124 ms: 1.04x faster                                                         |
| deepcopy                   | 371 us                                                 | 357 us: 1.04x faster                                                         |
| json_loads                 | 28.5 us                                                | 27.5 us: 1.04x faster                                                        |
| sympy_integrate            | 21.4 ms                                                | 20.7 ms: 1.04x faster                                                        |
| sympy_str                  | 300 ms                                                 | 290 ms: 1.03x faster                                                         |
| docutils                   | 2.77 sec                                               | 2.68 sec: 1.03x faster                                                       |
| unpickle                   | 15.9 us                                                | 15.4 us: 1.03x faster                                                        |
| json                       | 5.26 ms                                                | 5.11 ms: 1.03x faster                                                        |
| logging_silent             | 104 ns                                                 | 102 ns: 1.02x faster                                                         |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                        |
| pickle_dict                | 35.5 us                                                | 34.8 us: 1.02x faster                                                        |
| xml_etree_process          | 61.7 ms                                                | 60.6 ms: 1.02x faster                                                        |
| async_tree_memoization     | 578 ms                                                 | 569 ms: 1.02x faster                                                         |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.01x faster                                                         |
| coroutines                 | 23.2 ms                                                | 22.9 ms: 1.01x faster                                                        |
| dask                       | 372 ms                                                 | 367 ms: 1.01x faster                                                         |
| sqlglot_transpile          | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                        |
| async_generators           | 463 ms                                                 | 461 ms: 1.01x faster                                                         |
| xml_etree_generate         | 89.2 ms                                                | 88.8 ms: 1.00x faster                                                        |
| mdp                        | 2.63 sec                                               | 2.62 sec: 1.00x faster                                                       |
| bench_thread_pool          | 842 us                                                 | 845 us: 1.00x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 69.0 ms: 1.01x slower                                                        |
| unpickle_pure_python       | 230 us                                                 | 232 us: 1.01x slower                                                         |
| async_tree_none_tg         | 450 ms                                                 | 453 ms: 1.01x slower                                                         |
| regex_compile              | 148 ms                                                 | 150 ms: 1.01x slower                                                         |
| sqlite_synth               | 2.83 us                                                | 2.86 us: 1.01x slower                                                        |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                       |
| meteor_contest             | 112 ms                                                 | 113 ms: 1.01x slower                                                         |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 733 ms: 1.01x slower                                                         |
| create_gc_cycles           | 1.48 ms                                                | 1.50 ms: 1.01x slower                                                        |
| async_tree_memoization_tg  | 575 ms                                                 | 584 ms: 1.02x slower                                                         |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                        |
| crypto_pyaes               | 81.9 ms                                                | 83.4 ms: 1.02x slower                                                        |
| sqlglot_normalize          | 110 ms                                                 | 112 ms: 1.02x slower                                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                       |
| gc_traversal               | 3.79 ms                                                | 3.89 ms: 1.03x slower                                                        |
| xml_etree_iterparse        | 107 ms                                                 | 110 ms: 1.03x slower                                                         |
| pickle_list                | 5.08 us                                                | 5.23 us: 1.03x slower                                                        |
| pprint_safe_repr           | 776 ms                                                 | 799 ms: 1.03x slower                                                         |
| pickle                     | 11.6 us                                                | 12.0 us: 1.03x slower                                                        |
| sympy_expand               | 478 ms                                                 | 493 ms: 1.03x slower                                                         |
| 2to3                       | 274 ms                                                 | 284 ms: 1.03x slower                                                         |
| regex_effbot               | 3.61 ms                                                | 3.75 ms: 1.04x slower                                                        |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                       |
| richards                   | 45.8 ms                                                | 47.8 ms: 1.04x slower                                                        |
| richards_super             | 51.5 ms                                                | 53.9 ms: 1.05x slower                                                        |
| sqlglot_optimize           | 54.8 ms                                                | 57.6 ms: 1.05x slower                                                        |
| pprint_pformat             | 1.57 sec                                               | 1.66 sec: 1.06x slower                                                       |
| fannkuch                   | 417 ms                                                 | 444 ms: 1.06x slower                                                         |
| pyflate                    | 482 ms                                                 | 518 ms: 1.07x slower                                                         |
| python_startup             | 9.55 ms                                                | 10.3 ms: 1.07x slower                                                        |
| regex_dna                  | 212 ms                                                 | 228 ms: 1.08x slower                                                         |
| scimark_monte_carlo        | 75.1 ms                                                | 81.3 ms: 1.08x slower                                                        |
| pycparser                  | 1.18 sec                                               | 1.28 sec: 1.08x slower                                                       |
| chaos                      | 67.0 ms                                                | 72.8 ms: 1.09x slower                                                        |
| float                      | 84.7 ms                                                | 93.5 ms: 1.10x slower                                                        |
| go                         | 139 ms                                                 | 155 ms: 1.11x slower                                                         |
| tomli_loads                | 2.33 sec                                               | 2.61 sec: 1.12x slower                                                       |
| scimark_fft                | 382 ms                                                 | 433 ms: 1.13x slower                                                         |
| regex_v8                   | 23.1 ms                                                | 26.3 ms: 1.14x slower                                                        |
| nqueens                    | 83.3 ms                                                | 94.8 ms: 1.14x slower                                                        |
| mako                       | 11.9 ms                                                | 13.9 ms: 1.17x slower                                                        |
| spectral_norm              | 115 ms                                                 | 139 ms: 1.21x slower                                                         |
| telco                      | 7.10 ms                                                | 8.71 ms: 1.23x slower                                                        |
| nbody                      | 97.0 ms                                                | 121 ms: 1.25x slower                                                         |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.34 ms: 1.25x slower                                                        |
| python_startup_no_site     | 6.94 ms                                                | 8.88 ms: 1.28x slower                                                        |
| hexiom                     | 6.41 ms                                                | 8.40 ms: 1.31x slower                                                        |
| coverage                   | 72.7 ms                                                | 96.9 ms: 1.33x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                 |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed, deepcopy_memo, bench_mp_pool, asyncio_websockets, asyncio_tcp, scimark_lu, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.94% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x