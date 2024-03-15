
# Results vs. 3.12.0

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: 939c26f
- commit date: 2024-02-01
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 286 ms: 1.04x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                            |
| docutils       | 2.77 sec                                               | 2.73 sec: 1.02x faster                                                           |
| tornado_http   | 103 ms                                                 | 99.3 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 452 ms: 1.04x faster                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| async_tree_none_tg        | 450 ms                                                 | 459 ms: 1.02x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| async_tree_memoization_tg | 575 ms                                                 | 597 ms: 1.04x slower                                                             |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 100 ms: 1.18x slower                                                             |
| nbody          | 97.0 ms                                                | 119 ms: 1.23x slower                                                             |
| Geometric mean | (ref)                                                  | 1.14x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                            |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                                             |
| regex_compile  | 148 ms                                                 | 154 ms: 1.04x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                            |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 298 us: 1.09x faster                                                             |
| pickle_dict          | 35.5 us                                                | 33.2 us: 1.07x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.01 us: 1.06x faster                                                            |
| pickle_list          | 5.08 us                                                | 4.93 us: 1.03x faster                                                            |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| xml_etree_generate   | 89.2 ms                                                | 90.8 ms: 1.02x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 237 us: 1.03x slower                                                             |
| xml_etree_iterparse  | 107 ms                                                 | 114 ms: 1.07x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.70 sec: 1.16x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (4): xml_etree_parse, xml_etree_process, json_loads, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.7 ms: 1.23x slower                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 115 us: 1.37x faster                                                             |
| unpack_sequence           | 54.0 ns                                                | 39.6 ns: 1.36x faster                                                            |
| pickle_pure_python        | 324 us                                                 | 298 us: 1.09x faster                                                             |
| logging_format            | 7.23 us                                                | 6.71 us: 1.08x faster                                                            |
| pickle_dict               | 35.5 us                                                | 33.2 us: 1.07x faster                                                            |
| generators                | 31.2 ms                                                | 29.3 ms: 1.06x faster                                                            |
| logging_simple            | 6.46 us                                                | 6.10 us: 1.06x faster                                                            |
| deepcopy_reduce           | 3.35 us                                                | 3.17 us: 1.06x faster                                                            |
| unpickle_list             | 5.29 us                                                | 5.01 us: 1.06x faster                                                            |
| deepcopy                  | 371 us                                                 | 354 us: 1.05x faster                                                             |
| sympy_sum                 | 169 ms                                                 | 162 ms: 1.04x faster                                                             |
| async_tree_none           | 472 ms                                                 | 452 ms: 1.04x faster                                                             |
| coroutines                | 23.2 ms                                                | 22.4 ms: 1.04x faster                                                            |
| pathlib                   | 19.3 ms                                                | 18.7 ms: 1.03x faster                                                            |
| tornado_http              | 103 ms                                                 | 99.3 ms: 1.03x faster                                                            |
| pickle_list               | 5.08 us                                                | 4.93 us: 1.03x faster                                                            |
| raytrace                  | 312 ms                                                 | 304 ms: 1.03x faster                                                             |
| scimark_sor               | 129 ms                                                 | 126 ms: 1.02x faster                                                             |
| chameleon                 | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                            |
| docutils                  | 2.77 sec                                               | 2.73 sec: 1.02x faster                                                           |
| sqlglot_parse             | 1.36 ms                                                | 1.34 ms: 1.02x faster                                                            |
| pickle                    | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| dask                      | 372 ms                                                 | 367 ms: 1.01x faster                                                             |
| sqlglot_transpile         | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                            |
| gc_traversal              | 3.79 ms                                                | 3.76 ms: 1.01x faster                                                            |
| json                      | 5.26 ms                                                | 5.21 ms: 1.01x faster                                                            |
| sympy_integrate           | 21.4 ms                                                | 21.4 ms: 1.00x faster                                                            |
| logging_silent            | 104 ns                                                 | 105 ns: 1.00x slower                                                             |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.79 sec: 1.00x slower                                                           |
| async_generators          | 463 ms                                                 | 466 ms: 1.01x slower                                                             |
| deepcopy_memo             | 40.7 us                                                | 41.0 us: 1.01x slower                                                            |
| bench_thread_pool         | 842 us                                                 | 850 us: 1.01x slower                                                             |
| json_dumps                | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| regex_effbot              | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                            |
| pidigits                  | 187 ms                                                 | 190 ms: 1.01x slower                                                             |
| create_gc_cycles          | 1.48 ms                                                | 1.50 ms: 1.01x slower                                                            |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| dulwich_log               | 68.5 ms                                                | 69.6 ms: 1.02x slower                                                            |
| xml_etree_generate        | 89.2 ms                                                | 90.8 ms: 1.02x slower                                                            |
| async_tree_none_tg        | 450 ms                                                 | 459 ms: 1.02x slower                                                             |
| comprehensions            | 21.8 us                                                | 22.3 us: 1.03x slower                                                            |
| sqlite_synth              | 2.83 us                                                | 2.91 us: 1.03x slower                                                            |
| unpickle_pure_python      | 230 us                                                 | 237 us: 1.03x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| sympy_expand              | 478 ms                                                 | 493 ms: 1.03x slower                                                             |
| regex_dna                 | 212 ms                                                 | 220 ms: 1.04x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 597 ms: 1.04x slower                                                             |
| regex_compile             | 148 ms                                                 | 154 ms: 1.04x slower                                                             |
| sqlglot_normalize         | 110 ms                                                 | 115 ms: 1.04x slower                                                             |
| 2to3                      | 274 ms                                                 | 286 ms: 1.04x slower                                                             |
| meteor_contest            | 112 ms                                                 | 118 ms: 1.05x slower                                                             |
| crypto_pyaes              | 81.9 ms                                                | 86.2 ms: 1.05x slower                                                            |
| mdp                       | 2.63 sec                                               | 2.79 sec: 1.06x slower                                                           |
| pycparser                 | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                           |
| regex_v8                  | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                            |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| xml_etree_iterparse       | 107 ms                                                 | 114 ms: 1.07x slower                                                             |
| sqlglot_optimize          | 54.8 ms                                                | 58.9 ms: 1.07x slower                                                            |
| richards_super            | 51.5 ms                                                | 55.6 ms: 1.08x slower                                                            |
| pprint_safe_repr          | 776 ms                                                 | 837 ms: 1.08x slower                                                             |
| richards                  | 45.8 ms                                                | 49.6 ms: 1.08x slower                                                            |
| pprint_pformat            | 1.57 sec                                               | 1.74 sec: 1.11x slower                                                           |
| pyflate                   | 482 ms                                                 | 534 ms: 1.11x slower                                                             |
| chaos                     | 67.0 ms                                                | 74.3 ms: 1.11x slower                                                            |
| fannkuch                  | 417 ms                                                 | 463 ms: 1.11x slower                                                             |
| scimark_monte_carlo       | 75.1 ms                                                | 84.8 ms: 1.13x slower                                                            |
| tomli_loads               | 2.33 sec                                               | 2.70 sec: 1.16x slower                                                           |
| go                        | 139 ms                                                 | 162 ms: 1.16x slower                                                             |
| scimark_fft               | 382 ms                                                 | 447 ms: 1.17x slower                                                             |
| float                     | 84.7 ms                                                | 100 ms: 1.18x slower                                                             |
| nqueens                   | 83.3 ms                                                | 98.6 ms: 1.18x slower                                                            |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 6.18 ms: 1.22x slower                                                            |
| nbody                     | 97.0 ms                                                | 119 ms: 1.23x slower                                                             |
| telco                     | 7.10 ms                                                | 8.73 ms: 1.23x slower                                                            |
| mako                      | 11.9 ms                                                | 14.7 ms: 1.23x slower                                                            |
| python_startup_no_site    | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                            |
| spectral_norm             | 115 ms                                                 | 152 ms: 1.32x slower                                                             |
| coverage                  | 72.7 ms                                                | 96.9 ms: 1.33x slower                                                            |
| deltablue                 | 3.72 ms                                                | 5.18 ms: 1.39x slower                                                            |
| hexiom                    | 6.41 ms                                                | 9.09 ms: 1.42x slower                                                            |
| Geometric mean            | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (13): async_tree_cpu_io_mixed, sympy_str, xml_etree_parse, xml_etree_process, asyncio_tcp, asyncio_websockets, bench_mp_pool, async_tree_memoization, json_loads, scimark_lu, unpickle, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x