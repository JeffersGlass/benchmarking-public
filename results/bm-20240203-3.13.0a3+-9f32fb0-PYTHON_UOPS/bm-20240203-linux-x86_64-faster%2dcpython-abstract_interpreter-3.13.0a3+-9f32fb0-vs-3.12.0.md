
# Results vs. 3.12.0

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: 9f32fb0
- commit date: 2024-02-03
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.87%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 284 ms: 1.03x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.28 ms: 1.02x faster                                                            |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 99.0 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 448 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| async_tree_none_tg        | 450 ms                                                 | 458 ms: 1.02x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 586 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 90.0 ms: 1.06x slower                                                            |
| nbody          | 97.0 ms                                                | 109 ms: 1.12x slower                                                             |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 149 ms: 1.01x slower                                                             |
| regex_effbot   | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                            |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                                             |
| regex_v8       | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                             |
| unpickle_list        | 5.29 us                                                | 5.02 us: 1.05x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.6 us: 1.03x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 60.1 ms: 1.03x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                             |
| xml_etree_generate   | 89.2 ms                                                | 88.3 ms: 1.01x faster                                                            |
| json_loads           | 28.5 us                                                | 28.6 us: 1.00x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 108 ms: 1.01x slower                                                             |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 234 us: 1.02x slower                                                             |
| json_dumps           | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.03x slower                                                            |
| tomli_loads          | 2.33 sec                                               | 2.55 sec: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.80 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.1 ms: 1.10x slower                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-9f32fb0 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 112 us: 1.41x faster                                                             |
| logging_simple            | 6.46 us                                                | 5.85 us: 1.10x faster                                                            |
| logging_format            | 7.23 us                                                | 6.63 us: 1.09x faster                                                            |
| pickle_pure_python        | 324 us                                                 | 301 us: 1.08x faster                                                             |
| deepcopy_reduce           | 3.35 us                                                | 3.14 us: 1.07x faster                                                            |
| unpack_sequence           | 54.0 ns                                                | 50.7 ns: 1.06x faster                                                            |
| scimark_sor               | 129 ms                                                 | 122 ms: 1.06x faster                                                             |
| sympy_sum                 | 169 ms                                                 | 160 ms: 1.05x faster                                                             |
| unpickle_list             | 5.29 us                                                | 5.02 us: 1.05x faster                                                            |
| async_tree_none           | 472 ms                                                 | 448 ms: 1.05x faster                                                             |
| coroutines                | 23.2 ms                                                | 22.0 ms: 1.05x faster                                                            |
| deltablue                 | 3.72 ms                                                | 3.54 ms: 1.05x faster                                                            |
| comprehensions            | 21.8 us                                                | 20.8 us: 1.05x faster                                                            |
| pathlib                   | 19.3 ms                                                | 18.5 ms: 1.05x faster                                                            |
| raytrace                  | 312 ms                                                 | 301 ms: 1.04x faster                                                             |
| deepcopy                  | 371 us                                                 | 358 us: 1.04x faster                                                             |
| tornado_http              | 103 ms                                                 | 99.0 ms: 1.04x faster                                                            |
| generators                | 31.2 ms                                                | 30.3 ms: 1.03x faster                                                            |
| deepcopy_memo             | 40.7 us                                                | 39.6 us: 1.03x faster                                                            |
| pickle_dict               | 35.5 us                                                | 34.6 us: 1.03x faster                                                            |
| xml_etree_process         | 61.7 ms                                                | 60.1 ms: 1.03x faster                                                            |
| sqlglot_parse             | 1.36 ms                                                | 1.33 ms: 1.03x faster                                                            |
| docutils                  | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| sympy_integrate           | 21.4 ms                                                | 20.9 ms: 1.02x faster                                                            |
| sympy_str                 | 300 ms                                                 | 293 ms: 1.02x faster                                                             |
| chameleon                 | 7.41 ms                                                | 7.28 ms: 1.02x faster                                                            |
| sqlglot_transpile         | 1.68 ms                                                | 1.66 ms: 1.01x faster                                                            |
| xml_etree_parse           | 159 ms                                                 | 157 ms: 1.01x faster                                                             |
| scimark_lu                | 118 ms                                                 | 117 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| async_generators          | 463 ms                                                 | 457 ms: 1.01x faster                                                             |
| xml_etree_generate        | 89.2 ms                                                | 88.3 ms: 1.01x faster                                                            |
| create_gc_cycles          | 1.48 ms                                                | 1.47 ms: 1.00x faster                                                            |
| gc_traversal              | 3.79 ms                                                | 3.79 ms: 1.00x faster                                                            |
| json_loads                | 28.5 us                                                | 28.6 us: 1.00x slower                                                            |
| pidigits                  | 187 ms                                                 | 188 ms: 1.01x slower                                                             |
| regex_compile             | 148 ms                                                 | 149 ms: 1.01x slower                                                             |
| bench_thread_pool         | 842 us                                                 | 848 us: 1.01x slower                                                             |
| mdp                       | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                           |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| xml_etree_iterparse       | 107 ms                                                 | 108 ms: 1.01x slower                                                             |
| pickle                    | 11.6 us                                                | 11.7 us: 1.01x slower                                                            |
| unpickle_pure_python      | 230 us                                                 | 234 us: 1.02x slower                                                             |
| regex_effbot              | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                            |
| async_tree_none_tg        | 450 ms                                                 | 458 ms: 1.02x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 586 ms: 1.02x slower                                                             |
| dulwich_log               | 68.5 ms                                                | 69.9 ms: 1.02x slower                                                            |
| sqlglot_normalize         | 110 ms                                                 | 113 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| json_dumps                | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                            |
| pprint_safe_repr          | 776 ms                                                 | 795 ms: 1.03x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| 2to3                      | 274 ms                                                 | 284 ms: 1.03x slower                                                             |
| pickle_list               | 5.08 us                                                | 5.26 us: 1.03x slower                                                            |
| sympy_expand              | 478 ms                                                 | 496 ms: 1.04x slower                                                             |
| regex_dna                 | 212 ms                                                 | 220 ms: 1.04x slower                                                             |
| sqlglot_optimize          | 54.8 ms                                                | 57.1 ms: 1.04x slower                                                            |
| pprint_pformat            | 1.57 sec                                               | 1.65 sec: 1.05x slower                                                           |
| pyflate                   | 482 ms                                                 | 509 ms: 1.06x slower                                                             |
| richards_super            | 51.5 ms                                                | 54.5 ms: 1.06x slower                                                            |
| fannkuch                  | 417 ms                                                 | 441 ms: 1.06x slower                                                             |
| float                     | 84.7 ms                                                | 90.0 ms: 1.06x slower                                                            |
| scimark_monte_carlo       | 75.1 ms                                                | 79.9 ms: 1.06x slower                                                            |
| richards                  | 45.8 ms                                                | 48.8 ms: 1.06x slower                                                            |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.06x slower                                                            |
| pycparser                 | 1.18 sec                                               | 1.27 sec: 1.08x slower                                                           |
| chaos                     | 67.0 ms                                                | 72.2 ms: 1.08x slower                                                            |
| regex_v8                  | 23.1 ms                                                | 25.0 ms: 1.08x slower                                                            |
| tomli_loads               | 2.33 sec                                               | 2.55 sec: 1.10x slower                                                           |
| mako                      | 11.9 ms                                                | 13.1 ms: 1.10x slower                                                            |
| nqueens                   | 83.3 ms                                                | 92.3 ms: 1.11x slower                                                            |
| nbody                     | 97.0 ms                                                | 109 ms: 1.12x slower                                                             |
| scimark_fft               | 382 ms                                                 | 431 ms: 1.13x slower                                                             |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.75 ms: 1.14x slower                                                            |
| spectral_norm             | 115 ms                                                 | 134 ms: 1.17x slower                                                             |
| telco                     | 7.10 ms                                                | 8.79 ms: 1.24x slower                                                            |
| go                        | 139 ms                                                 | 175 ms: 1.25x slower                                                             |
| hexiom                    | 6.41 ms                                                | 8.11 ms: 1.26x slower                                                            |
| python_startup_no_site    | 6.94 ms                                                | 8.80 ms: 1.27x slower                                                            |
| coverage                  | 72.7 ms                                                | 95.8 ms: 1.32x slower                                                            |
| Geometric mean            | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (12): dask, async_tree_memoization, crypto_pyaes, meteor_contest, bench_mp_pool, asyncio_websockets, json, asyncio_tcp, async_tree_cpu_io_mixed_tg, logging_silent, sqlite_synth, unpickle
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.87% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x