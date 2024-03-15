# Results vs. 3.12.0

- fork: faster-cpython
- ref: optimize_inline_valu
- machine: linux-x86_64
- commit hash: b93e9d3
- commit date: 2024-03-07
- overall geometric mean: 1.03x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 290 ms: 1.06x slower                                                             |
| chameleon      | 7.41 ms                                                | 6.93 ms: 1.07x faster                                                            |
| docutils       | 2.77 sec                                               | 2.83 sec: 1.02x slower                                                           |
| tornado_http   | 103 ms                                                 | 97.5 ms: 1.05x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 444 ms: 1.06x faster                                                             |
| async_tree_memoization    | 578 ms                                                 | 572 ms: 1.01x faster                                                             |
| async_tree_none_tg        | 450 ms                                                 | 451 ms: 1.00x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 581 ms: 1.01x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| Geometric mean            | (ref)                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 93.3 ms: 1.10x slower                                                            |
| nbody          | 97.0 ms                                                | 122 ms: 1.26x slower                                                             |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.49 ms: 1.03x faster                                                            |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                            |
| regex_compile  | 148 ms                                                 | 160 ms: 1.08x slower                                                             |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.86 us: 1.09x faster                                                            |
| pickle_pure_python   | 324 us                                                 | 306 us: 1.06x faster                                                             |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.3 us: 1.04x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 60.2 ms: 1.03x faster                                                            |
| json_loads           | 28.5 us                                                | 27.8 us: 1.02x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                             |
| xml_etree_generate   | 89.2 ms                                                | 88.3 ms: 1.01x faster                                                            |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.48 sec: 1.06x slower                                                           |
| unpickle_pure_python | 230 us                                                 | 262 us: 1.14x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (2): pickle_list, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.79 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 34.6 ms                                                | 34.0 ms: 1.02x faster                                                            |
| mako            | 11.9 ms                                                | 11.9 ms: 1.00x slower                                                            |
| Geometric mean  | (ref)                                                  | 1.01x faster                                                                     |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 114 us: 1.39x faster                                                             |
| logging_format            | 7.23 us                                                | 6.26 us: 1.15x faster                                                            |
| logging_simple            | 6.46 us                                                | 5.73 us: 1.13x faster                                                            |
| unpickle_list             | 5.29 us                                                | 4.86 us: 1.09x faster                                                            |
| deepcopy_reduce           | 3.35 us                                                | 3.10 us: 1.08x faster                                                            |
| chameleon                 | 7.41 ms                                                | 6.93 ms: 1.07x faster                                                            |
| coroutines                | 23.2 ms                                                | 21.8 ms: 1.06x faster                                                            |
| generators                | 31.2 ms                                                | 29.3 ms: 1.06x faster                                                            |
| async_tree_none           | 472 ms                                                 | 444 ms: 1.06x faster                                                             |
| sympy_sum                 | 169 ms                                                 | 159 ms: 1.06x faster                                                             |
| pickle_pure_python        | 324 us                                                 | 306 us: 1.06x faster                                                             |
| tornado_http              | 103 ms                                                 | 97.5 ms: 1.05x faster                                                            |
| unpickle                  | 15.9 us                                                | 15.1 us: 1.05x faster                                                            |
| pickle_dict               | 35.5 us                                                | 34.3 us: 1.04x faster                                                            |
| regex_effbot              | 3.61 ms                                                | 3.49 ms: 1.03x faster                                                            |
| sympy_integrate           | 21.4 ms                                                | 20.8 ms: 1.03x faster                                                            |
| sympy_str                 | 300 ms                                                 | 292 ms: 1.03x faster                                                             |
| comprehensions            | 21.8 us                                                | 21.2 us: 1.03x faster                                                            |
| deepcopy                  | 371 us                                                 | 362 us: 1.03x faster                                                             |
| xml_etree_process         | 61.7 ms                                                | 60.2 ms: 1.03x faster                                                            |
| json_loads                | 28.5 us                                                | 27.8 us: 1.02x faster                                                            |
| gc_traversal              | 3.79 ms                                                | 3.71 ms: 1.02x faster                                                            |
| xml_etree_parse           | 159 ms                                                 | 156 ms: 1.02x faster                                                             |
| django_template           | 34.6 ms                                                | 34.0 ms: 1.02x faster                                                            |
| sqlglot_normalize         | 110 ms                                                 | 108 ms: 1.02x faster                                                             |
| logging_silent            | 104 ns                                                 | 103 ns: 1.01x faster                                                             |
| sqlglot_parse             | 1.36 ms                                                | 1.35 ms: 1.01x faster                                                            |
| async_tree_memoization    | 578 ms                                                 | 572 ms: 1.01x faster                                                             |
| xml_etree_generate        | 89.2 ms                                                | 88.3 ms: 1.01x faster                                                            |
| mako                      | 11.9 ms                                                | 11.9 ms: 1.00x slower                                                            |
| mdp                       | 2.63 sec                                               | 2.64 sec: 1.00x slower                                                           |
| async_tree_none_tg        | 450 ms                                                 | 451 ms: 1.00x slower                                                             |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| pickle                    | 11.6 us                                                | 11.7 us: 1.01x slower                                                            |
| dulwich_log               | 68.5 ms                                                | 69.1 ms: 1.01x slower                                                            |
| async_tree_memoization_tg | 575 ms                                                 | 581 ms: 1.01x slower                                                             |
| crypto_pyaes              | 81.9 ms                                                | 83.1 ms: 1.02x slower                                                            |
| deltablue                 | 3.72 ms                                                | 3.78 ms: 1.02x slower                                                            |
| bench_thread_pool         | 842 us                                                 | 857 us: 1.02x slower                                                             |
| create_gc_cycles          | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                            |
| sqlglot_optimize          | 54.8 ms                                                | 55.9 ms: 1.02x slower                                                            |
| docutils                  | 2.77 sec                                               | 2.83 sec: 1.02x slower                                                           |
| sympy_expand              | 478 ms                                                 | 490 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| deepcopy_memo             | 40.7 us                                                | 41.8 us: 1.03x slower                                                            |
| aiohttp                   | 1.15 ms                                                | 1.18 ms: 1.03x slower                                                            |
| gunicorn                  | 1.24 ms                                                | 1.28 ms: 1.03x slower                                                            |
| xml_etree_iterparse       | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| richards                  | 45.8 ms                                                | 47.3 ms: 1.03x slower                                                            |
| pprint_safe_repr          | 776 ms                                                 | 801 ms: 1.03x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| sqlite_synth              | 2.83 us                                                | 2.93 us: 1.03x slower                                                            |
| meteor_contest            | 112 ms                                                 | 116 ms: 1.03x slower                                                             |
| regex_dna                 | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| richards_super            | 51.5 ms                                                | 53.8 ms: 1.04x slower                                                            |
| 2to3                      | 274 ms                                                 | 290 ms: 1.06x slower                                                             |
| pprint_pformat            | 1.57 sec                                               | 1.66 sec: 1.06x slower                                                           |
| raytrace                  | 312 ms                                                 | 330 ms: 1.06x slower                                                             |
| tomli_loads               | 2.33 sec                                               | 2.48 sec: 1.06x slower                                                           |
| python_startup            | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| unpack_sequence           | 54.0 ns                                                | 57.7 ns: 1.07x slower                                                            |
| regex_v8                  | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                            |
| regex_compile             | 148 ms                                                 | 160 ms: 1.08x slower                                                             |
| chaos                     | 67.0 ms                                                | 72.3 ms: 1.08x slower                                                            |
| float                     | 84.7 ms                                                | 93.3 ms: 1.10x slower                                                            |
| scimark_fft               | 382 ms                                                 | 426 ms: 1.12x slower                                                             |
| pycparser                 | 1.18 sec                                               | 1.32 sec: 1.12x slower                                                           |
| unpickle_pure_python      | 230 us                                                 | 262 us: 1.14x slower                                                             |
| scimark_monte_carlo       | 75.1 ms                                                | 85.7 ms: 1.14x slower                                                            |
| fannkuch                  | 417 ms                                                 | 481 ms: 1.15x slower                                                             |
| scimark_sor               | 129 ms                                                 | 151 ms: 1.17x slower                                                             |
| nqueens                   | 83.3 ms                                                | 98.1 ms: 1.18x slower                                                            |
| pyflate                   | 482 ms                                                 | 571 ms: 1.18x slower                                                             |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 6.02 ms: 1.19x slower                                                            |
| telco                     | 7.10 ms                                                | 8.51 ms: 1.20x slower                                                            |
| go                        | 139 ms                                                 | 175 ms: 1.25x slower                                                             |
| nbody                     | 97.0 ms                                                | 122 ms: 1.26x slower                                                             |
| python_startup_no_site    | 6.94 ms                                                | 8.79 ms: 1.27x slower                                                            |
| coverage                  | 72.7 ms                                                | 96.5 ms: 1.33x slower                                                            |
| scimark_lu                | 118 ms                                                 | 160 ms: 1.35x slower                                                             |
| hexiom                    | 6.41 ms                                                | 8.78 ms: 1.37x slower                                                            |
| dask                      | 372 ms                                                 | 536 ms: 1.44x slower                                                             |
| Geometric mean            | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (14): async_tree_cpu_io_mixed, json, spectral_norm, sqlglot_transpile, pickle_list, bench_mp_pool, async_generators, pathlib, async_tree_cpu_io_mixed_tg, pidigits, asyncio_tcp, asyncio_websockets, json_dumps, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240307-3.13.0a4+-b93e9d3-PYTHON_UOPS/bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.94x