
# Results vs. 3.12.0

- fork: faster-cpython
- ref: globals_to_constants
- machine: linux-x86_64
- commit hash: 9d9bc24
- commit date: 2024-01-18
- overall geometric mean: 1.02x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 283 ms: 1.03x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.20 ms: 1.03x faster                                                            |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 101 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 449 ms: 1.05x faster                                                             |
| async_tree_none_tg        | 450 ms                                                 | 455 ms: 1.01x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 584 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| async_tree_io             | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 91.1 ms: 1.08x slower                                                            |
| nbody          | 97.0 ms                                                | 118 ms: 1.22x slower                                                             |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.53 ms: 1.02x faster                                                            |
| regex_compile  | 148 ms                                                 | 151 ms: 1.02x slower                                                             |
| regex_dna      | 212 ms                                                 | 225 ms: 1.06x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                             |
| pickle_dict          | 35.5 us                                                | 33.0 us: 1.08x faster                                                            |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                            |
| pickle_list          | 5.08 us                                                | 4.95 us: 1.03x faster                                                            |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                             |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 61.4 ms: 1.01x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.33 us: 1.01x slower                                                            |
| xml_etree_generate   | 89.2 ms                                                | 90.1 ms: 1.01x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| tomli_loads          | 2.33 sec                                               | 2.39 sec: 1.02x slower                                                           |
| unpickle_pure_python | 230 us                                                 | 237 us: 1.03x slower                                                             |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 115 us: 1.37x faster                                                             |
| unpack_sequence           | 54.0 ns                                                | 40.3 ns: 1.34x faster                                                            |
| pickle_pure_python        | 324 us                                                 | 299 us: 1.08x faster                                                             |
| pickle_dict               | 35.5 us                                                | 33.0 us: 1.08x faster                                                            |
| deepcopy_reduce           | 3.35 us                                                | 3.14 us: 1.07x faster                                                            |
| logging_simple            | 6.46 us                                                | 6.08 us: 1.06x faster                                                            |
| unpickle                  | 15.9 us                                                | 15.0 us: 1.06x faster                                                            |
| sympy_sum                 | 169 ms                                                 | 160 ms: 1.05x faster                                                             |
| async_tree_none           | 472 ms                                                 | 449 ms: 1.05x faster                                                             |
| pathlib                   | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                            |
| logging_format            | 7.23 us                                                | 6.90 us: 1.05x faster                                                            |
| raytrace                  | 312 ms                                                 | 300 ms: 1.04x faster                                                             |
| generators                | 31.2 ms                                                | 30.1 ms: 1.04x faster                                                            |
| deepcopy                  | 371 us                                                 | 359 us: 1.03x faster                                                             |
| sympy_str                 | 300 ms                                                 | 291 ms: 1.03x faster                                                             |
| chameleon                 | 7.41 ms                                                | 7.20 ms: 1.03x faster                                                            |
| sqlglot_parse             | 1.36 ms                                                | 1.32 ms: 1.03x faster                                                            |
| docutils                  | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| pickle_list               | 5.08 us                                                | 4.95 us: 1.03x faster                                                            |
| gc_traversal              | 3.79 ms                                                | 3.70 ms: 1.02x faster                                                            |
| pickle                    | 11.6 us                                                | 11.3 us: 1.02x faster                                                            |
| comprehensions            | 21.8 us                                                | 21.3 us: 1.02x faster                                                            |
| regex_effbot              | 3.61 ms                                                | 3.53 ms: 1.02x faster                                                            |
| sqlglot_transpile         | 1.68 ms                                                | 1.65 ms: 1.02x faster                                                            |
| coroutines                | 23.2 ms                                                | 22.8 ms: 1.02x faster                                                            |
| asyncio_tcp               | 491 ms                                                 | 483 ms: 1.02x faster                                                             |
| xml_etree_parse           | 159 ms                                                 | 157 ms: 1.01x faster                                                             |
| tornado_http              | 103 ms                                                 | 101 ms: 1.01x faster                                                             |
| dask                      | 372 ms                                                 | 367 ms: 1.01x faster                                                             |
| async_generators          | 463 ms                                                 | 457 ms: 1.01x faster                                                             |
| sympy_integrate           | 21.4 ms                                                | 21.1 ms: 1.01x faster                                                            |
| json_loads                | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| json                      | 5.26 ms                                                | 5.22 ms: 1.01x faster                                                            |
| xml_etree_process         | 61.7 ms                                                | 61.4 ms: 1.01x faster                                                            |
| create_gc_cycles          | 1.48 ms                                                | 1.47 ms: 1.00x faster                                                            |
| deepcopy_memo             | 40.7 us                                                | 40.9 us: 1.01x slower                                                            |
| pidigits                  | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| bench_thread_pool         | 842 us                                                 | 848 us: 1.01x slower                                                             |
| unpickle_list             | 5.29 us                                                | 5.33 us: 1.01x slower                                                            |
| xml_etree_generate        | 89.2 ms                                                | 90.1 ms: 1.01x slower                                                            |
| async_tree_none_tg        | 450 ms                                                 | 455 ms: 1.01x slower                                                             |
| dulwich_log               | 68.5 ms                                                | 69.4 ms: 1.01x slower                                                            |
| crypto_pyaes              | 81.9 ms                                                | 83.0 ms: 1.01x slower                                                            |
| sympy_expand              | 478 ms                                                 | 485 ms: 1.02x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 584 ms: 1.02x slower                                                             |
| scimark_sor               | 129 ms                                                 | 131 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| regex_compile             | 148 ms                                                 | 151 ms: 1.02x slower                                                             |
| logging_silent            | 104 ns                                                 | 107 ns: 1.02x slower                                                             |
| json_dumps                | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| pycparser                 | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| scimark_lu                | 118 ms                                                 | 121 ms: 1.02x slower                                                             |
| tomli_loads               | 2.33 sec                                               | 2.39 sec: 1.02x slower                                                           |
| meteor_contest            | 112 ms                                                 | 115 ms: 1.03x slower                                                             |
| unpickle_pure_python      | 230 us                                                 | 237 us: 1.03x slower                                                             |
| sqlite_synth              | 2.83 us                                                | 2.92 us: 1.03x slower                                                            |
| 2to3                      | 274 ms                                                 | 283 ms: 1.03x slower                                                             |
| xml_etree_iterparse       | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| sqlglot_normalize         | 110 ms                                                 | 115 ms: 1.04x slower                                                             |
| pprint_safe_repr          | 776 ms                                                 | 818 ms: 1.05x slower                                                             |
| sqlglot_optimize          | 54.8 ms                                                | 57.9 ms: 1.06x slower                                                            |
| python_startup            | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| regex_dna                 | 212 ms                                                 | 225 ms: 1.06x slower                                                             |
| richards                  | 45.8 ms                                                | 48.8 ms: 1.06x slower                                                            |
| richards_super            | 51.5 ms                                                | 54.8 ms: 1.06x slower                                                            |
| scimark_monte_carlo       | 75.1 ms                                                | 80.2 ms: 1.07x slower                                                            |
| regex_v8                  | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                            |
| float                     | 84.7 ms                                                | 91.1 ms: 1.08x slower                                                            |
| pprint_pformat            | 1.57 sec                                               | 1.70 sec: 1.08x slower                                                           |
| fannkuch                  | 417 ms                                                 | 455 ms: 1.09x slower                                                             |
| chaos                     | 67.0 ms                                                | 73.7 ms: 1.10x slower                                                            |
| pyflate                   | 482 ms                                                 | 532 ms: 1.10x slower                                                             |
| go                        | 139 ms                                                 | 155 ms: 1.11x slower                                                             |
| nqueens                   | 83.3 ms                                                | 94.6 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.91 ms: 1.17x slower                                                            |
| mako                      | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                            |
| scimark_fft               | 382 ms                                                 | 456 ms: 1.19x slower                                                             |
| telco                     | 7.10 ms                                                | 8.56 ms: 1.21x slower                                                            |
| nbody                     | 97.0 ms                                                | 118 ms: 1.22x slower                                                             |
| python_startup_no_site    | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                            |
| spectral_norm             | 115 ms                                                 | 147 ms: 1.28x slower                                                             |
| deltablue                 | 3.72 ms                                                | 4.74 ms: 1.28x slower                                                            |
| hexiom                    | 6.41 ms                                                | 8.42 ms: 1.31x slower                                                            |
| coverage                  | 72.7 ms                                                | 95.5 ms: 1.31x slower                                                            |
| Geometric mean            | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed, async_tree_memoization, mdp, bench_mp_pool, asyncio_websockets, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x