# Results vs. base

- fork: faster-cpython
- ref: optimize_inline_valu
- machine: linux-x86_64
- commit hash: b93e9d3
- commit date: 2024-03-07
- overall geometric mean: 1.00x slower
- HPT reliability: 68.17%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 289 ms                                                                 | 290 ms: 1.00x slower                                                             |
| docutils       | 2.78 sec                                                               | 2.83 sec: 1.02x slower                                                           |
| tornado_http   | 98.2 ms                                                                | 97.5 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): chameleon, html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_memoization_tg | 588 ms                                                                 | 581 ms: 1.01x faster                                                             |
| async_tree_none_tg        | 457 ms                                                                 | 451 ms: 1.01x faster                                                             |
| async_tree_memoization    | 578 ms                                                                 | 572 ms: 1.01x faster                                                             |
| Geometric mean            | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_io_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x slower                                                             |
| float          | 91.4 ms                                                                | 93.3 ms: 1.02x slower                                                            |
| nbody          | 120 ms                                                                 | 122 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.56 ms                                                                | 3.49 ms: 1.02x faster                                                            |
| regex_compile  | 157 ms                                                                 | 160 ms: 1.02x slower                                                             |
| regex_v8       | 24.2 ms                                                                | 24.7 ms: 1.02x slower                                                            |
| regex_dna      | 212 ms                                                                 | 221 ms: 1.04x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.09 us                                                                | 4.86 us: 1.05x faster                                                            |
| xml_etree_parse      | 158 ms                                                                 | 156 ms: 1.01x faster                                                             |
| json_dumps           | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                                            |
| xml_etree_generate   | 88.7 ms                                                                | 88.3 ms: 1.00x faster                                                            |
| pickle_pure_python   | 304 us                                                                 | 306 us: 1.01x slower                                                             |
| json_loads           | 27.7 us                                                                | 27.8 us: 1.01x slower                                                            |
| unpickle_pure_python | 259 us                                                                 | 262 us: 1.01x slower                                                             |
| tomli_loads          | 2.44 sec                                                               | 2.48 sec: 1.01x slower                                                           |
| pickle_list          | 4.97 us                                                                | 5.07 us: 1.02x slower                                                            |
| pickle               | 11.4 us                                                                | 11.7 us: 1.02x slower                                                            |
| pickle_dict          | 33.5 us                                                                | 34.3 us: 1.02x slower                                                            |
| unpickle             | 14.6 us                                                                | 15.1 us: 1.03x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): xml_etree_process, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 8.84 ms                                                                | 8.79 ms: 1.00x faster                                                            |
| python_startup         | 10.2 ms                                                                | 10.2 ms: 1.00x faster                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|-----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| genshi_text     | 25.5 ms                                                                | 25.1 ms: 1.02x faster                                                            |
| django_template | 34.3 ms                                                                | 34.0 ms: 1.01x faster                                                            |
| genshi_xml      | 56.5 ms                                                                | 57.4 ms: 1.02x slower                                                            |
| mako            | 11.7 ms                                                                | 11.9 ms: 1.02x slower                                                            |
| Geometric mean  | (ref)                                                                  | 1.00x slower                                                                     |

All benchmarks:
===============

| Benchmark                 | bm-20240307-linux-x86_64-python-72d3cc94cd8cae1925e7-3.13.0a4+-72d3cc9 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mdp                       | 2.82 sec                                                               | 2.64 sec: 1.07x faster                                                           |
| unpickle_list             | 5.09 us                                                                | 4.86 us: 1.05x faster                                                            |
| logging_format            | 6.39 us                                                                | 6.26 us: 1.02x faster                                                            |
| regex_effbot              | 3.56 ms                                                                | 3.49 ms: 1.02x faster                                                            |
| coroutines                | 22.2 ms                                                                | 21.8 ms: 1.02x faster                                                            |
| telco                     | 8.65 ms                                                                | 8.51 ms: 1.02x faster                                                            |
| logging_simple            | 5.82 us                                                                | 5.73 us: 1.02x faster                                                            |
| genshi_text               | 25.5 ms                                                                | 25.1 ms: 1.02x faster                                                            |
| raytrace                  | 335 ms                                                                 | 330 ms: 1.02x faster                                                             |
| sqlglot_normalize         | 110 ms                                                                 | 108 ms: 1.01x faster                                                             |
| go                        | 177 ms                                                                 | 175 ms: 1.01x faster                                                             |
| sympy_expand              | 496 ms                                                                 | 490 ms: 1.01x faster                                                             |
| async_tree_memoization_tg | 588 ms                                                                 | 581 ms: 1.01x faster                                                             |
| async_tree_none_tg        | 457 ms                                                                 | 451 ms: 1.01x faster                                                             |
| sympy_integrate           | 21.0 ms                                                                | 20.8 ms: 1.01x faster                                                            |
| deepcopy_reduce           | 3.14 us                                                                | 3.10 us: 1.01x faster                                                            |
| async_tree_memoization    | 578 ms                                                                 | 572 ms: 1.01x faster                                                             |
| async_generators          | 468 ms                                                                 | 463 ms: 1.01x faster                                                             |
| deepcopy_memo             | 42.2 us                                                                | 41.8 us: 1.01x faster                                                            |
| xml_etree_parse           | 158 ms                                                                 | 156 ms: 1.01x faster                                                             |
| pathlib                   | 19.5 ms                                                                | 19.3 ms: 1.01x faster                                                            |
| django_template           | 34.3 ms                                                                | 34.0 ms: 1.01x faster                                                            |
| sympy_sum                 | 161 ms                                                                 | 159 ms: 1.01x faster                                                             |
| richards                  | 47.8 ms                                                                | 47.3 ms: 1.01x faster                                                            |
| generators                | 29.6 ms                                                                | 29.3 ms: 1.01x faster                                                            |
| richards_super            | 54.2 ms                                                                | 53.8 ms: 1.01x faster                                                            |
| json_dumps                | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                                            |
| dulwich_log               | 69.7 ms                                                                | 69.1 ms: 1.01x faster                                                            |
| tornado_http              | 98.2 ms                                                                | 97.5 ms: 1.01x faster                                                            |
| sqlglot_optimize          | 56.2 ms                                                                | 55.9 ms: 1.01x faster                                                            |
| asyncio_tcp_ssl           | 1.81 sec                                                               | 1.80 sec: 1.01x faster                                                           |
| python_startup_no_site    | 8.84 ms                                                                | 8.79 ms: 1.00x faster                                                            |
| xml_etree_generate        | 88.7 ms                                                                | 88.3 ms: 1.00x faster                                                            |
| python_startup            | 10.2 ms                                                                | 10.2 ms: 1.00x faster                                                            |
| fannkuch                  | 483 ms                                                                 | 481 ms: 1.00x faster                                                             |
| asyncio_tcp               | 493 ms                                                                 | 491 ms: 1.00x faster                                                             |
| bench_thread_pool         | 859 us                                                                 | 857 us: 1.00x faster                                                             |
| pidigits                  | 187 ms                                                                 | 187 ms: 1.00x slower                                                             |
| 2to3                      | 289 ms                                                                 | 290 ms: 1.00x slower                                                             |
| pickle_pure_python        | 304 us                                                                 | 306 us: 1.01x slower                                                             |
| json_loads                | 27.7 us                                                                | 27.8 us: 1.01x slower                                                            |
| crypto_pyaes              | 82.6 ms                                                                | 83.1 ms: 1.01x slower                                                            |
| coverage                  | 95.9 ms                                                                | 96.5 ms: 1.01x slower                                                            |
| meteor_contest            | 115 ms                                                                 | 116 ms: 1.01x slower                                                             |
| pprint_pformat            | 1.64 sec                                                               | 1.66 sec: 1.01x slower                                                           |
| deepcopy                  | 358 us                                                                 | 362 us: 1.01x slower                                                             |
| sqlite_synth              | 2.90 us                                                                | 2.93 us: 1.01x slower                                                            |
| deltablue                 | 3.74 ms                                                                | 3.78 ms: 1.01x slower                                                            |
| unpickle_pure_python      | 259 us                                                                 | 262 us: 1.01x slower                                                             |
| pyflate                   | 563 ms                                                                 | 571 ms: 1.01x slower                                                             |
| tomli_loads               | 2.44 sec                                                               | 2.48 sec: 1.01x slower                                                           |
| genshi_xml                | 56.5 ms                                                                | 57.4 ms: 1.02x slower                                                            |
| docutils                  | 2.78 sec                                                               | 2.83 sec: 1.02x slower                                                           |
| mako                      | 11.7 ms                                                                | 11.9 ms: 1.02x slower                                                            |
| regex_compile             | 157 ms                                                                 | 160 ms: 1.02x slower                                                             |
| pickle_list               | 4.97 us                                                                | 5.07 us: 1.02x slower                                                            |
| float                     | 91.4 ms                                                                | 93.3 ms: 1.02x slower                                                            |
| regex_v8                  | 24.2 ms                                                                | 24.7 ms: 1.02x slower                                                            |
| gc_traversal              | 3.63 ms                                                                | 3.71 ms: 1.02x slower                                                            |
| scimark_sor               | 147 ms                                                                 | 151 ms: 1.02x slower                                                             |
| nbody                     | 120 ms                                                                 | 122 ms: 1.02x slower                                                             |
| pickle                    | 11.4 us                                                                | 11.7 us: 1.02x slower                                                            |
| scimark_fft               | 416 ms                                                                 | 426 ms: 1.02x slower                                                             |
| pickle_dict               | 33.5 us                                                                | 34.3 us: 1.02x slower                                                            |
| hexiom                    | 8.55 ms                                                                | 8.78 ms: 1.03x slower                                                            |
| comprehensions            | 20.7 us                                                                | 21.2 us: 1.03x slower                                                            |
| unpack_sequence           | 56.0 ns                                                                | 57.7 ns: 1.03x slower                                                            |
| unpickle                  | 14.6 us                                                                | 15.1 us: 1.03x slower                                                            |
| scimark_lu                | 154 ms                                                                 | 160 ms: 1.04x slower                                                             |
| scimark_monte_carlo       | 82.8 ms                                                                | 85.7 ms: 1.04x slower                                                            |
| pycparser                 | 1.27 sec                                                               | 1.32 sec: 1.04x slower                                                           |
| regex_dna                 | 212 ms                                                                 | 221 ms: 1.04x slower                                                             |
| scimark_sparse_mat_mult   | 5.73 ms                                                                | 6.02 ms: 1.05x slower                                                            |
| Geometric mean            | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (29): sympy_str, json, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, thrift, async_tree_none, chaos, logging_silent, nqueens, async_tree_io_tg, xml_etree_process, bench_mp_pool, xml_etree_iterparse, mypy2, chameleon, asyncio_websockets, gunicorn, dask, async_tree_io, create_gc_cycles, sqlglot_transpile, pylint, spectral_norm, pprint_safe_repr, djangocms, sqlglot_parse, html5lib, typing_runtime_protocols, aiohttp


# HPT report

- Reliability score: 68.17% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x