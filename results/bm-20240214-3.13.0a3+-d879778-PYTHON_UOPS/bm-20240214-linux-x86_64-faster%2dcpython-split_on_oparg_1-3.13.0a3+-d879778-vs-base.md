# Results vs. base

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: d879778
- commit date: 2024-02-14
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                                 | 284 ms: 1.01x faster                                                         |
| docutils       | 2.72 sec                                                               | 2.68 sec: 1.01x faster                                                       |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_memoization_tg | 595 ms                                                                 | 584 ms: 1.02x faster                                                         |
| async_tree_memoization    | 575 ms                                                                 | 569 ms: 1.01x faster                                                         |
| async_tree_none_tg        | 458 ms                                                                 | 453 ms: 1.01x faster                                                         |
| async_tree_io             | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                       |
| Geometric mean            | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (4): async_tree_none, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 145 ms                                                                 | 121 ms: 1.20x faster                                                         |
| float          | 99.4 ms                                                                | 93.5 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                                  | 1.08x faster                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 155 ms                                                                 | 150 ms: 1.03x faster                                                         |
| regex_v8       | 26.6 ms                                                                | 26.3 ms: 1.01x faster                                                        |
| regex_dna      | 229 ms                                                                 | 228 ms: 1.00x faster                                                         |
| regex_effbot   | 3.72 ms                                                                | 3.75 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 2.76 sec                                                               | 2.61 sec: 1.06x faster                                                       |
| json_loads           | 28.3 us                                                                | 27.5 us: 1.03x faster                                                        |
| unpickle_pure_python | 238 us                                                                 | 232 us: 1.03x faster                                                         |
| xml_etree_iterparse  | 113 ms                                                                 | 110 ms: 1.03x faster                                                         |
| xml_etree_generate   | 90.5 ms                                                                | 88.8 ms: 1.02x faster                                                        |
| unpickle_list        | 5.06 us                                                                | 4.97 us: 1.02x faster                                                        |
| xml_etree_process    | 61.6 ms                                                                | 60.6 ms: 1.02x faster                                                        |
| pickle_pure_python   | 301 us                                                                 | 299 us: 1.00x faster                                                         |
| json_dumps           | 10.5 ms                                                                | 10.6 ms: 1.00x slower                                                        |
| pickle_dict          | 33.7 us                                                                | 34.8 us: 1.03x slower                                                        |
| pickle               | 11.5 us                                                                | 12.0 us: 1.04x slower                                                        |
| pickle_list          | 4.88 us                                                                | 5.23 us: 1.07x slower                                                        |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (2): unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 8.84 ms                                                                | 8.88 ms: 1.00x slower                                                        |
| python_startup         | 10.2 ms                                                                | 10.3 ms: 1.01x slower                                                        |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 15.0 ms                                                                | 13.9 ms: 1.08x faster                                                        |

All benchmarks:
===============

| Benchmark                 | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody                     | 145 ms                                                                 | 121 ms: 1.20x faster                                                         |
| unpack_sequence           | 49.3 ns                                                                | 42.9 ns: 1.15x faster                                                        |
| hexiom                    | 9.27 ms                                                                | 8.40 ms: 1.10x faster                                                        |
| nqueens                   | 104 ms                                                                 | 94.8 ms: 1.09x faster                                                        |
| spectral_norm             | 151 ms                                                                 | 139 ms: 1.09x faster                                                         |
| pyflate                   | 562 ms                                                                 | 518 ms: 1.08x faster                                                         |
| scimark_monte_carlo       | 87.9 ms                                                                | 81.3 ms: 1.08x faster                                                        |
| mako                      | 15.0 ms                                                                | 13.9 ms: 1.08x faster                                                        |
| mdp                       | 2.81 sec                                                               | 2.62 sec: 1.07x faster                                                       |
| comprehensions            | 21.7 us                                                                | 20.3 us: 1.07x faster                                                        |
| crypto_pyaes              | 89.0 ms                                                                | 83.4 ms: 1.07x faster                                                        |
| scimark_fft               | 461 ms                                                                 | 433 ms: 1.07x faster                                                         |
| chaos                     | 77.4 ms                                                                | 72.8 ms: 1.06x faster                                                        |
| float                     | 99.4 ms                                                                | 93.5 ms: 1.06x faster                                                        |
| tomli_loads               | 2.76 sec                                                               | 2.61 sec: 1.06x faster                                                       |
| fannkuch                  | 469 ms                                                                 | 444 ms: 1.06x faster                                                         |
| go                        | 162 ms                                                                 | 155 ms: 1.04x faster                                                         |
| meteor_contest            | 118 ms                                                                 | 113 ms: 1.04x faster                                                         |
| deltablue                 | 3.62 ms                                                                | 3.50 ms: 1.03x faster                                                        |
| pprint_pformat            | 1.72 sec                                                               | 1.66 sec: 1.03x faster                                                       |
| regex_compile             | 155 ms                                                                 | 150 ms: 1.03x faster                                                         |
| raytrace                  | 308 ms                                                                 | 298 ms: 1.03x faster                                                         |
| pprint_safe_repr          | 825 ms                                                                 | 799 ms: 1.03x faster                                                         |
| json_loads                | 28.3 us                                                                | 27.5 us: 1.03x faster                                                        |
| deepcopy_memo             | 41.8 us                                                                | 40.6 us: 1.03x faster                                                        |
| unpickle_pure_python      | 238 us                                                                 | 232 us: 1.03x faster                                                         |
| xml_etree_iterparse       | 113 ms                                                                 | 110 ms: 1.03x faster                                                         |
| richards_super            | 55.3 ms                                                                | 53.9 ms: 1.03x faster                                                        |
| richards                  | 48.9 ms                                                                | 47.8 ms: 1.02x faster                                                        |
| sympy_sum                 | 162 ms                                                                 | 159 ms: 1.02x faster                                                         |
| logging_silent            | 104 ns                                                                 | 102 ns: 1.02x faster                                                         |
| generators                | 29.7 ms                                                                | 29.1 ms: 1.02x faster                                                        |
| sqlglot_parse             | 1.36 ms                                                                | 1.33 ms: 1.02x faster                                                        |
| typing_runtime_protocols  | 117 us                                                                 | 115 us: 1.02x faster                                                         |
| json                      | 5.21 ms                                                                | 5.11 ms: 1.02x faster                                                        |
| async_tree_memoization_tg | 595 ms                                                                 | 584 ms: 1.02x faster                                                         |
| xml_etree_generate        | 90.5 ms                                                                | 88.8 ms: 1.02x faster                                                        |
| unpickle_list             | 5.06 us                                                                | 4.97 us: 1.02x faster                                                        |
| xml_etree_process         | 61.6 ms                                                                | 60.6 ms: 1.02x faster                                                        |
| sympy_str                 | 295 ms                                                                 | 290 ms: 1.02x faster                                                         |
| logging_format            | 6.87 us                                                                | 6.76 us: 1.02x faster                                                        |
| sqlglot_optimize          | 58.6 ms                                                                | 57.6 ms: 1.02x faster                                                        |
| sqlglot_transpile         | 1.69 ms                                                                | 1.67 ms: 1.01x faster                                                        |
| docutils                  | 2.72 sec                                                               | 2.68 sec: 1.01x faster                                                       |
| 2to3                      | 287 ms                                                                 | 284 ms: 1.01x faster                                                         |
| async_tree_memoization    | 575 ms                                                                 | 569 ms: 1.01x faster                                                         |
| regex_v8                  | 26.6 ms                                                                | 26.3 ms: 1.01x faster                                                        |
| async_tree_none_tg        | 458 ms                                                                 | 453 ms: 1.01x faster                                                         |
| telco                     | 8.80 ms                                                                | 8.71 ms: 1.01x faster                                                        |
| pycparser                 | 1.29 sec                                                               | 1.28 sec: 1.01x faster                                                       |
| sympy_integrate           | 20.9 ms                                                                | 20.7 ms: 1.01x faster                                                        |
| bench_thread_pool         | 852 us                                                                 | 845 us: 1.01x faster                                                         |
| deepcopy                  | 360 us                                                                 | 357 us: 1.01x faster                                                         |
| dulwich_log               | 69.4 ms                                                                | 69.0 ms: 1.01x faster                                                        |
| deepcopy_reduce           | 3.16 us                                                                | 3.14 us: 1.01x faster                                                        |
| pickle_pure_python        | 301 us                                                                 | 299 us: 1.00x faster                                                         |
| sqlglot_normalize         | 113 ms                                                                 | 112 ms: 1.00x faster                                                         |
| regex_dna                 | 229 ms                                                                 | 228 ms: 1.00x faster                                                         |
| create_gc_cycles          | 1.50 ms                                                                | 1.50 ms: 1.00x faster                                                        |
| asyncio_tcp_ssl           | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                       |
| python_startup_no_site    | 8.84 ms                                                                | 8.88 ms: 1.00x slower                                                        |
| json_dumps                | 10.5 ms                                                                | 10.6 ms: 1.00x slower                                                        |
| asyncio_tcp               | 489 ms                                                                 | 491 ms: 1.00x slower                                                         |
| python_startup            | 10.2 ms                                                                | 10.3 ms: 1.01x slower                                                        |
| async_tree_io             | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                       |
| regex_effbot              | 3.72 ms                                                                | 3.75 ms: 1.01x slower                                                        |
| scimark_lu                | 118 ms                                                                 | 119 ms: 1.01x slower                                                         |
| coverage                  | 95.3 ms                                                                | 96.9 ms: 1.02x slower                                                        |
| gc_traversal              | 3.78 ms                                                                | 3.89 ms: 1.03x slower                                                        |
| pickle_dict               | 33.7 us                                                                | 34.8 us: 1.03x slower                                                        |
| pickle                    | 11.5 us                                                                | 12.0 us: 1.04x slower                                                        |
| pickle_list               | 4.88 us                                                                | 5.23 us: 1.07x slower                                                        |
| Geometric mean            | (ref)                                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (21): async_tree_none, mypy2, logging_simple, tornado_http, async_tree_cpu_io_mixed, unpickle, scimark_sor, chameleon, scimark_sparse_mat_mult, sqlite_synth, bench_mp_pool, asyncio_websockets, pidigits, sympy_expand, coroutines, async_tree_io_tg, dask, async_tree_cpu_io_mixed_tg, pathlib, async_generators, xml_etree_parse


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x