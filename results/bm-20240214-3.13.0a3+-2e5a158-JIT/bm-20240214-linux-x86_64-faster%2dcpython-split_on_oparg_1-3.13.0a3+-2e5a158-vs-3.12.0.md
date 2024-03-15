
# Results vs. 3.12.0

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: 2e5a158
- commit date: 2024-02-14
- overall geometric mean: 1.01x faster \*
- HPT reliability: 55.56%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 277 ms: 1.01x slower                                                         |
| chameleon      | 7.41 ms                                                | 6.88 ms: 1.08x faster                                                        |
| docutils       | 2.77 sec                                               | 2.65 sec: 1.05x faster                                                       |
| tornado_http   | 103 ms                                                 | 96.6 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                  | 1.04x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 445 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                         |
| async_tree_memoization    | 578 ms                                                 | 571 ms: 1.01x faster                                                         |
| async_tree_none_tg        | 450 ms                                                 | 456 ms: 1.01x slower                                                         |
| async_tree_memoization_tg | 575 ms                                                 | 584 ms: 1.02x slower                                                         |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                       |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                       |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                         |
| nbody          | 97.0 ms                                                | 104 ms: 1.07x slower                                                         |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 140 ms: 1.06x faster                                                         |
| regex_effbot   | 3.61 ms                                                | 3.70 ms: 1.03x slower                                                        |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                         |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                        |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                         |
| pickle_dict          | 35.5 us                                                | 33.6 us: 1.06x faster                                                        |
| tomli_loads          | 2.33 sec                                               | 2.21 sec: 1.05x faster                                                       |
| xml_etree_process    | 61.7 ms                                                | 58.5 ms: 1.05x faster                                                        |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                                        |
| unpickle_list        | 5.29 us                                                | 5.05 us: 1.05x faster                                                        |
| xml_etree_generate   | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                        |
| xml_etree_parse      | 159 ms                                                 | 155 ms: 1.03x faster                                                         |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                                        |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                                        |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.00x faster                                                         |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                                 |

Benchmark hidden because not significant (2): pickle_list, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.3 ms: 1.08x slower                                                        |
| python_startup_no_site | 6.94 ms                                                | 8.91 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.2 ms: 1.03x slower                                                        |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 111 us: 1.43x faster                                                         |
| comprehensions            | 21.8 us                                                | 18.2 us: 1.20x faster                                                        |
| logging_format            | 7.23 us                                                | 6.34 us: 1.14x faster                                                        |
| logging_simple            | 6.46 us                                                | 5.77 us: 1.12x faster                                                        |
| raytrace                  | 312 ms                                                 | 283 ms: 1.10x faster                                                         |
| deltablue                 | 3.72 ms                                                | 3.39 ms: 1.10x faster                                                        |
| pickle_pure_python        | 324 us                                                 | 299 us: 1.08x faster                                                         |
| deepcopy_reduce           | 3.35 us                                                | 3.10 us: 1.08x faster                                                        |
| chameleon                 | 7.41 ms                                                | 6.88 ms: 1.08x faster                                                        |
| sympy_sum                 | 169 ms                                                 | 157 ms: 1.07x faster                                                         |
| generators                | 31.2 ms                                                | 29.2 ms: 1.07x faster                                                        |
| scimark_sor               | 129 ms                                                 | 121 ms: 1.07x faster                                                         |
| tornado_http              | 103 ms                                                 | 96.6 ms: 1.06x faster                                                        |
| sympy_str                 | 300 ms                                                 | 282 ms: 1.06x faster                                                         |
| async_tree_none           | 472 ms                                                 | 445 ms: 1.06x faster                                                         |
| deepcopy                  | 371 us                                                 | 351 us: 1.06x faster                                                         |
| regex_compile             | 148 ms                                                 | 140 ms: 1.06x faster                                                         |
| pickle_dict               | 35.5 us                                                | 33.6 us: 1.06x faster                                                        |
| tomli_loads               | 2.33 sec                                               | 2.21 sec: 1.05x faster                                                       |
| xml_etree_process         | 61.7 ms                                                | 58.5 ms: 1.05x faster                                                        |
| sqlglot_parse             | 1.36 ms                                                | 1.29 ms: 1.05x faster                                                        |
| unpickle                  | 15.9 us                                                | 15.1 us: 1.05x faster                                                        |
| unpickle_list             | 5.29 us                                                | 5.05 us: 1.05x faster                                                        |
| docutils                  | 2.77 sec                                               | 2.65 sec: 1.05x faster                                                       |
| pathlib                   | 19.3 ms                                                | 18.6 ms: 1.04x faster                                                        |
| scimark_lu                | 118 ms                                                 | 113 ms: 1.04x faster                                                         |
| xml_etree_generate        | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                        |
| deepcopy_memo             | 40.7 us                                                | 39.2 us: 1.04x faster                                                        |
| sympy_integrate           | 21.4 ms                                                | 20.6 ms: 1.04x faster                                                        |
| crypto_pyaes              | 81.9 ms                                                | 78.7 ms: 1.04x faster                                                        |
| sqlglot_transpile         | 1.68 ms                                                | 1.63 ms: 1.04x faster                                                        |
| xml_etree_parse           | 159 ms                                                 | 155 ms: 1.03x faster                                                         |
| json_loads                | 28.5 us                                                | 27.7 us: 1.03x faster                                                        |
| meteor_contest            | 112 ms                                                 | 110 ms: 1.02x faster                                                         |
| pickle                    | 11.6 us                                                | 11.3 us: 1.02x faster                                                        |
| mdp                       | 2.63 sec                                               | 2.57 sec: 1.02x faster                                                       |
| scimark_fft               | 382 ms                                                 | 374 ms: 1.02x faster                                                         |
| json                      | 5.26 ms                                                | 5.15 ms: 1.02x faster                                                        |
| sqlglot_normalize         | 110 ms                                                 | 108 ms: 1.02x faster                                                         |
| dask                      | 372 ms                                                 | 366 ms: 1.02x faster                                                         |
| richards                  | 45.8 ms                                                | 45.1 ms: 1.02x faster                                                        |
| logging_silent            | 104 ns                                                 | 103 ns: 1.02x faster                                                         |
| coroutines                | 23.2 ms                                                | 22.8 ms: 1.01x faster                                                        |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                         |
| async_tree_memoization    | 578 ms                                                 | 571 ms: 1.01x faster                                                         |
| dulwich_log               | 68.5 ms                                                | 67.9 ms: 1.01x faster                                                        |
| async_generators          | 463 ms                                                 | 461 ms: 1.00x faster                                                         |
| unpickle_pure_python      | 230 us                                                 | 229 us: 1.00x faster                                                         |
| asyncio_tcp               | 491 ms                                                 | 489 ms: 1.00x faster                                                         |
| pidigits                  | 187 ms                                                 | 188 ms: 1.00x slower                                                         |
| json_dumps                | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                        |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                       |
| 2to3                      | 274 ms                                                 | 277 ms: 1.01x slower                                                         |
| sqlglot_optimize          | 54.8 ms                                                | 55.4 ms: 1.01x slower                                                        |
| create_gc_cycles          | 1.48 ms                                                | 1.50 ms: 1.01x slower                                                        |
| async_tree_none_tg        | 450 ms                                                 | 456 ms: 1.01x slower                                                         |
| gc_traversal              | 3.79 ms                                                | 3.85 ms: 1.01x slower                                                        |
| async_tree_memoization_tg | 575 ms                                                 | 584 ms: 1.02x slower                                                         |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                       |
| regex_effbot              | 3.61 ms                                                | 3.70 ms: 1.03x slower                                                        |
| mako                      | 11.9 ms                                                | 12.2 ms: 1.03x slower                                                        |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                       |
| pprint_pformat            | 1.57 sec                                               | 1.63 sec: 1.04x slower                                                       |
| pyflate                   | 482 ms                                                 | 504 ms: 1.04x slower                                                         |
| regex_dna                 | 212 ms                                                 | 222 ms: 1.05x slower                                                         |
| chaos                     | 67.0 ms                                                | 70.5 ms: 1.05x slower                                                        |
| go                        | 139 ms                                                 | 149 ms: 1.07x slower                                                         |
| nbody                     | 97.0 ms                                                | 104 ms: 1.07x slower                                                         |
| unpack_sequence           | 54.0 ns                                                | 58.0 ns: 1.07x slower                                                        |
| python_startup            | 9.55 ms                                                | 10.3 ms: 1.08x slower                                                        |
| nqueens                   | 83.3 ms                                                | 90.2 ms: 1.08x slower                                                        |
| regex_v8                  | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                        |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.55 ms: 1.10x slower                                                        |
| spectral_norm             | 115 ms                                                 | 132 ms: 1.15x slower                                                         |
| telco                     | 7.10 ms                                                | 8.65 ms: 1.22x slower                                                        |
| hexiom                    | 6.41 ms                                                | 7.86 ms: 1.23x slower                                                        |
| python_startup_no_site    | 6.94 ms                                                | 8.91 ms: 1.28x slower                                                        |
| coverage                  | 72.7 ms                                                | 94.8 ms: 1.30x slower                                                        |
| Geometric mean            | (ref)                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (15): sqlite_synth, richards_super, pickle_list, bench_mp_pool, bench_thread_pool, asyncio_websockets, fannkuch, sympy_expand, xml_etree_iterparse, float, scimark_monte_carlo, pycparser, pprint_safe_repr, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 55.56% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x