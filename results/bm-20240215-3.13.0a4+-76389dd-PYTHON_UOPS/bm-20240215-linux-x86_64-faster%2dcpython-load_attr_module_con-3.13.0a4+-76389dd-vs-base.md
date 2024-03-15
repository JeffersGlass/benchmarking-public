# Results vs. base

- fork: faster-cpython
- ref: load_attr_module_con
- machine: linux-x86_64
- commit hash: 76389dd
- commit date: 2024-02-15
- overall geometric mean: 1.00x slower
- HPT reliability: 80.94%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 292 ms                                                                 | 292 ms: 1.00x faster                                                             |
| chameleon      | 7.23 ms                                                                | 7.10 ms: 1.02x faster                                                            |
| docutils       | 2.81 sec                                                               | 2.80 sec: 1.00x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg | 459 ms                                                                 | 455 ms: 1.01x faster                                                             |
| async_tree_io_tg   | 1.22 sec                                                               | 1.21 sec: 1.01x faster                                                           |
| async_tree_io      | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (5): async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 90.8 ms                                                                | 89.8 ms: 1.01x faster                                                            |
| pidigits       | 189 ms                                                                 | 189 ms: 1.00x slower                                                             |
| nbody          | 114 ms                                                                 | 115 ms: 1.01x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.85 ms                                                                | 3.58 ms: 1.08x faster                                                            |
| regex_dna      | 230 ms                                                                 | 221 ms: 1.04x faster                                                             |
| regex_v8       | 25.9 ms                                                                | 25.1 ms: 1.03x faster                                                            |
| regex_compile  | 172 ms                                                                 | 176 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|---------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle            | 15.6 us                                                                | 15.1 us: 1.03x faster                                                            |
| pickle_dict         | 34.6 us                                                                | 33.6 us: 1.03x faster                                                            |
| pickle_list         | 5.23 us                                                                | 5.08 us: 1.03x faster                                                            |
| pickle              | 11.7 us                                                                | 11.6 us: 1.01x faster                                                            |
| xml_etree_iterparse | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| xml_etree_generate  | 89.1 ms                                                                | 89.5 ms: 1.01x slower                                                            |
| tomli_loads         | 2.63 sec                                                               | 2.64 sec: 1.01x slower                                                           |
| json_loads          | 27.5 us                                                                | 27.7 us: 1.01x slower                                                            |
| unpickle_list       | 4.96 us                                                                | 5.23 us: 1.05x slower                                                            |
| Geometric mean      | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (5): json_dumps, pickle_pure_python, unpickle_pure_python, xml_etree_parse, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 8.85 ms                                                                | 8.82 ms: 1.00x faster                                                            |
| python_startup         | 10.2 ms                                                                | 10.2 ms: 1.00x faster                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 13.0 ms                                                                | 14.0 ms: 1.08x slower                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot             | 3.85 ms                                                                | 3.58 ms: 1.08x faster                                                            |
| mdp                      | 2.84 sec                                                               | 2.66 sec: 1.07x faster                                                           |
| logging_silent           | 105 ns                                                                 | 100 ns: 1.04x faster                                                             |
| pycparser                | 1.32 sec                                                               | 1.27 sec: 1.04x faster                                                           |
| regex_dna                | 230 ms                                                                 | 221 ms: 1.04x faster                                                             |
| unpickle                 | 15.6 us                                                                | 15.1 us: 1.03x faster                                                            |
| gc_traversal             | 3.87 ms                                                                | 3.75 ms: 1.03x faster                                                            |
| regex_v8                 | 25.9 ms                                                                | 25.1 ms: 1.03x faster                                                            |
| pickle_dict              | 34.6 us                                                                | 33.6 us: 1.03x faster                                                            |
| pickle_list              | 5.23 us                                                                | 5.08 us: 1.03x faster                                                            |
| create_gc_cycles         | 1.52 ms                                                                | 1.49 ms: 1.02x faster                                                            |
| json                     | 5.14 ms                                                                | 5.04 ms: 1.02x faster                                                            |
| chameleon                | 7.23 ms                                                                | 7.10 ms: 1.02x faster                                                            |
| float                    | 90.8 ms                                                                | 89.8 ms: 1.01x faster                                                            |
| scimark_fft              | 424 ms                                                                 | 419 ms: 1.01x faster                                                             |
| deepcopy_reduce          | 3.14 us                                                                | 3.11 us: 1.01x faster                                                            |
| generators               | 29.7 ms                                                                | 29.4 ms: 1.01x faster                                                            |
| async_tree_none_tg       | 459 ms                                                                 | 455 ms: 1.01x faster                                                             |
| coroutines               | 23.1 ms                                                                | 23.0 ms: 1.01x faster                                                            |
| async_tree_io_tg         | 1.22 sec                                                               | 1.21 sec: 1.01x faster                                                           |
| pickle                   | 11.7 us                                                                | 11.6 us: 1.01x faster                                                            |
| xml_etree_iterparse      | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| async_tree_io            | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| chaos                    | 74.4 ms                                                                | 73.9 ms: 1.01x faster                                                            |
| asyncio_tcp              | 493 ms                                                                 | 491 ms: 1.00x faster                                                             |
| docutils                 | 2.81 sec                                                               | 2.80 sec: 1.00x faster                                                           |
| python_startup_no_site   | 8.85 ms                                                                | 8.82 ms: 1.00x faster                                                            |
| 2to3                     | 292 ms                                                                 | 292 ms: 1.00x faster                                                             |
| asyncio_tcp_ssl          | 1.81 sec                                                               | 1.80 sec: 1.00x faster                                                           |
| python_startup           | 10.2 ms                                                                | 10.2 ms: 1.00x faster                                                            |
| bench_mp_pool            | 24.0 ms                                                                | 24.0 ms: 1.00x slower                                                            |
| sympy_integrate          | 21.1 ms                                                                | 21.2 ms: 1.00x slower                                                            |
| pidigits                 | 189 ms                                                                 | 189 ms: 1.00x slower                                                             |
| xml_etree_generate       | 89.1 ms                                                                | 89.5 ms: 1.01x slower                                                            |
| tomli_loads              | 2.63 sec                                                               | 2.64 sec: 1.01x slower                                                           |
| nbody                    | 114 ms                                                                 | 115 ms: 1.01x slower                                                             |
| deltablue                | 3.70 ms                                                                | 3.72 ms: 1.01x slower                                                            |
| typing_runtime_protocols | 113 us                                                                 | 114 us: 1.01x slower                                                             |
| bench_thread_pool        | 856 us                                                                 | 862 us: 1.01x slower                                                             |
| logging_format           | 7.00 us                                                                | 7.05 us: 1.01x slower                                                            |
| meteor_contest           | 115 ms                                                                 | 116 ms: 1.01x slower                                                             |
| json_loads               | 27.5 us                                                                | 27.7 us: 1.01x slower                                                            |
| pprint_safe_repr         | 844 ms                                                                 | 851 ms: 1.01x slower                                                             |
| telco                    | 8.72 ms                                                                | 8.81 ms: 1.01x slower                                                            |
| sqlglot_transpile        | 1.75 ms                                                                | 1.76 ms: 1.01x slower                                                            |
| dulwich_log              | 72.0 ms                                                                | 72.7 ms: 1.01x slower                                                            |
| pathlib                  | 18.9 ms                                                                | 19.1 ms: 1.01x slower                                                            |
| fannkuch                 | 468 ms                                                                 | 473 ms: 1.01x slower                                                             |
| deepcopy                 | 356 us                                                                 | 360 us: 1.01x slower                                                             |
| comprehensions           | 20.7 us                                                                | 21.0 us: 1.01x slower                                                            |
| sqlglot_parse            | 1.41 ms                                                                | 1.43 ms: 1.01x slower                                                            |
| scimark_monte_carlo      | 84.3 ms                                                                | 85.6 ms: 1.02x slower                                                            |
| go                       | 173 ms                                                                 | 176 ms: 1.02x slower                                                             |
| deepcopy_memo            | 41.0 us                                                                | 41.7 us: 1.02x slower                                                            |
| unpack_sequence          | 55.8 ns                                                                | 57.0 ns: 1.02x slower                                                            |
| nqueens                  | 97.8 ms                                                                | 100 ms: 1.02x slower                                                             |
| scimark_sparse_mat_mult  | 5.68 ms                                                                | 5.82 ms: 1.02x slower                                                            |
| hexiom                   | 8.93 ms                                                                | 9.15 ms: 1.02x slower                                                            |
| regex_compile            | 172 ms                                                                 | 176 ms: 1.03x slower                                                             |
| richards_super           | 64.2 ms                                                                | 66.0 ms: 1.03x slower                                                            |
| pprint_pformat           | 1.76 sec                                                               | 1.82 sec: 1.03x slower                                                           |
| spectral_norm            | 132 ms                                                                 | 136 ms: 1.03x slower                                                             |
| pyflate                  | 565 ms                                                                 | 588 ms: 1.04x slower                                                             |
| richards                 | 57.6 ms                                                                | 59.9 ms: 1.04x slower                                                            |
| raytrace                 | 339 ms                                                                 | 355 ms: 1.05x slower                                                             |
| unpickle_list            | 4.96 us                                                                | 5.23 us: 1.05x slower                                                            |
| scimark_lu               | 154 ms                                                                 | 167 ms: 1.08x slower                                                             |
| mako                     | 13.0 ms                                                                | 14.0 ms: 1.08x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (25): async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_none, json_dumps, scimark_sor, asyncio_websockets, pickle_pure_python, tornado_http, unpickle_pure_python, sqlglot_normalize, crypto_pyaes, dask, sqlglot_optimize, mypy2, logging_simple, xml_etree_parse, async_generators, xml_etree_process, sympy_sum, sympy_str, sympy_expand, sqlite_synth, coverage, async_tree_memoization_tg


# HPT report

- Reliability score: 80.94% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x