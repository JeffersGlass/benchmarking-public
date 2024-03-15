
# Results vs. 3.12.0

- fork: faster-cpython
- ref: load_attr_module_con
- machine: linux-x86_64
- commit hash: 76389dd
- commit date: 2024-02-15
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 292 ms: 1.06x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.10 ms: 1.04x faster                                                            |
| docutils       | 2.77 sec                                               | 2.80 sec: 1.01x slower                                                           |
| tornado_http   | 103 ms                                                 | 99.0 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                             |
| async_tree_none_tg        | 450 ms                                                 | 455 ms: 1.01x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                           |
| async_tree_io             | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| async_tree_memoization_tg | 575 ms                                                 | 603 ms: 1.05x slower                                                             |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 89.8 ms: 1.06x slower                                                            |
| nbody          | 97.0 ms                                                | 115 ms: 1.18x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.58 ms: 1.01x faster                                                            |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| regex_v8       | 23.1 ms                                                | 25.1 ms: 1.08x slower                                                            |
| regex_compile  | 148 ms                                                 | 176 ms: 1.19x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                             |
| pickle_dict          | 35.5 us                                                | 33.6 us: 1.06x faster                                                            |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                                            |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 61.0 ms: 1.01x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.23 us: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| xml_etree_generate   | 89.2 ms                                                | 89.5 ms: 1.00x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.64 sec: 1.14x slower                                                           |
| unpickle_pure_python | 230 us                                                 | 271 us: 1.18x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): pickle_list, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 114 us: 1.38x faster                                                             |
| pickle_pure_python        | 324 us                                                 | 301 us: 1.08x faster                                                             |
| deepcopy_reduce           | 3.35 us                                                | 3.11 us: 1.07x faster                                                            |
| generators                | 31.2 ms                                                | 29.4 ms: 1.06x faster                                                            |
| pickle_dict               | 35.5 us                                                | 33.6 us: 1.06x faster                                                            |
| async_tree_none           | 472 ms                                                 | 450 ms: 1.05x faster                                                             |
| unpickle                  | 15.9 us                                                | 15.1 us: 1.05x faster                                                            |
| logging_simple            | 6.46 us                                                | 6.17 us: 1.05x faster                                                            |
| chameleon                 | 7.41 ms                                                | 7.10 ms: 1.04x faster                                                            |
| json                      | 5.26 ms                                                | 5.04 ms: 1.04x faster                                                            |
| logging_silent            | 104 ns                                                 | 100 ns: 1.04x faster                                                             |
| tornado_http              | 103 ms                                                 | 99.0 ms: 1.04x faster                                                            |
| sympy_sum                 | 169 ms                                                 | 163 ms: 1.04x faster                                                             |
| comprehensions            | 21.8 us                                                | 21.0 us: 1.04x faster                                                            |
| deepcopy                  | 371 us                                                 | 360 us: 1.03x faster                                                             |
| json_loads                | 28.5 us                                                | 27.7 us: 1.03x faster                                                            |
| logging_format            | 7.23 us                                                | 7.05 us: 1.03x faster                                                            |
| pathlib                   | 19.3 ms                                                | 19.1 ms: 1.01x faster                                                            |
| xml_etree_process         | 61.7 ms                                                | 61.0 ms: 1.01x faster                                                            |
| dask                      | 372 ms                                                 | 367 ms: 1.01x faster                                                             |
| sympy_integrate           | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                            |
| unpickle_list             | 5.29 us                                                | 5.23 us: 1.01x faster                                                            |
| gc_traversal              | 3.79 ms                                                | 3.75 ms: 1.01x faster                                                            |
| xml_etree_parse           | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| coroutines                | 23.2 ms                                                | 23.0 ms: 1.01x faster                                                            |
| regex_effbot              | 3.61 ms                                                | 3.58 ms: 1.01x faster                                                            |
| sympy_str                 | 300 ms                                                 | 298 ms: 1.01x faster                                                             |
| xml_etree_generate        | 89.2 ms                                                | 89.5 ms: 1.00x slower                                                            |
| async_generators          | 463 ms                                                 | 466 ms: 1.01x slower                                                             |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| mdp                       | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                           |
| pidigits                  | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| async_tree_none_tg        | 450 ms                                                 | 455 ms: 1.01x slower                                                             |
| create_gc_cycles          | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                            |
| docutils                  | 2.77 sec                                               | 2.80 sec: 1.01x slower                                                           |
| json_dumps                | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| sqlite_synth              | 2.83 us                                                | 2.89 us: 1.02x slower                                                            |
| bench_thread_pool         | 842 us                                                 | 862 us: 1.02x slower                                                             |
| deepcopy_memo             | 40.7 us                                                | 41.7 us: 1.02x slower                                                            |
| crypto_pyaes              | 81.9 ms                                                | 83.9 ms: 1.02x slower                                                            |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                           |
| sqlglot_normalize         | 110 ms                                                 | 113 ms: 1.03x slower                                                             |
| meteor_contest            | 112 ms                                                 | 116 ms: 1.03x slower                                                             |
| xml_etree_iterparse       | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| regex_dna                 | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| sqlglot_transpile         | 1.68 ms                                                | 1.76 ms: 1.05x slower                                                            |
| async_tree_memoization_tg | 575 ms                                                 | 603 ms: 1.05x slower                                                             |
| sqlglot_parse             | 1.36 ms                                                | 1.43 ms: 1.05x slower                                                            |
| sympy_expand              | 478 ms                                                 | 505 ms: 1.06x slower                                                             |
| unpack_sequence           | 54.0 ns                                                | 57.0 ns: 1.06x slower                                                            |
| float                     | 84.7 ms                                                | 89.8 ms: 1.06x slower                                                            |
| dulwich_log               | 68.5 ms                                                | 72.7 ms: 1.06x slower                                                            |
| 2to3                      | 274 ms                                                 | 292 ms: 1.06x slower                                                             |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| pycparser                 | 1.18 sec                                               | 1.27 sec: 1.08x slower                                                           |
| regex_v8                  | 23.1 ms                                                | 25.1 ms: 1.08x slower                                                            |
| scimark_sor               | 129 ms                                                 | 141 ms: 1.09x slower                                                             |
| pprint_safe_repr          | 776 ms                                                 | 851 ms: 1.10x slower                                                             |
| scimark_fft               | 382 ms                                                 | 419 ms: 1.10x slower                                                             |
| sqlglot_optimize          | 54.8 ms                                                | 60.2 ms: 1.10x slower                                                            |
| chaos                     | 67.0 ms                                                | 73.9 ms: 1.10x slower                                                            |
| fannkuch                  | 417 ms                                                 | 473 ms: 1.13x slower                                                             |
| tomli_loads               | 2.33 sec                                               | 2.64 sec: 1.14x slower                                                           |
| raytrace                  | 312 ms                                                 | 355 ms: 1.14x slower                                                             |
| scimark_monte_carlo       | 75.1 ms                                                | 85.6 ms: 1.14x slower                                                            |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.82 ms: 1.15x slower                                                            |
| pprint_pformat            | 1.57 sec                                               | 1.82 sec: 1.16x slower                                                           |
| unpickle_pure_python      | 230 us                                                 | 271 us: 1.18x slower                                                             |
| mako                      | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                            |
| nbody                     | 97.0 ms                                                | 115 ms: 1.18x slower                                                             |
| spectral_norm             | 115 ms                                                 | 136 ms: 1.19x slower                                                             |
| regex_compile             | 148 ms                                                 | 176 ms: 1.19x slower                                                             |
| nqueens                   | 83.3 ms                                                | 100 ms: 1.20x slower                                                             |
| pyflate                   | 482 ms                                                 | 588 ms: 1.22x slower                                                             |
| telco                     | 7.10 ms                                                | 8.81 ms: 1.24x slower                                                            |
| go                        | 139 ms                                                 | 176 ms: 1.26x slower                                                             |
| python_startup_no_site    | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                            |
| richards_super            | 51.5 ms                                                | 66.0 ms: 1.28x slower                                                            |
| richards                  | 45.8 ms                                                | 59.9 ms: 1.31x slower                                                            |
| coverage                  | 72.7 ms                                                | 97.9 ms: 1.35x slower                                                            |
| scimark_lu                | 118 ms                                                 | 167 ms: 1.41x slower                                                             |
| hexiom                    | 6.41 ms                                                | 9.15 ms: 1.43x slower                                                            |
| Geometric mean            | (ref)                                                  | 1.05x slower                                                                     |

Benchmark hidden because not significant (10): async_tree_memoization, async_tree_cpu_io_mixed, bench_mp_pool, asyncio_tcp, pickle_list, asyncio_websockets, pickle, deltablue, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.94x