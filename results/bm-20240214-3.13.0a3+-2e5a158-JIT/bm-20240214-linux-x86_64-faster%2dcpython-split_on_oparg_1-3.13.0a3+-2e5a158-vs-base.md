# Results vs. base

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: 2e5a158
- commit date: 2024-02-14
- overall geometric mean: 1.00x slower
- HPT reliability: 99.19%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| docutils       | 2.64 sec                                                               | 2.65 sec: 1.00x slower                                                       |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (3): 2to3, chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none_tg         | 452 ms                                                                 | 456 ms: 1.01x slower                                                         |
| async_tree_memoization     | 565 ms                                                                 | 571 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed    | 708 ms                                                                 | 717 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed_tg | 720 ms                                                                 | 732 ms: 1.02x slower                                                         |
| async_tree_io              | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                                       |
| async_tree_io_tg           | 1.18 sec                                                               | 1.21 sec: 1.02x slower                                                       |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x faster                                                         |
| nbody          | 101 ms                                                                 | 104 ms: 1.03x slower                                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 225 ms                                                                 | 222 ms: 1.01x faster                                                         |
| regex_compile  | 140 ms                                                                 | 140 ms: 1.01x slower                                                         |
| regex_effbot   | 3.65 ms                                                                | 3.70 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle             | 16.0 us                                                                | 15.1 us: 1.05x faster                                                        |
| pickle               | 11.7 us                                                                | 11.3 us: 1.03x faster                                                        |
| xml_etree_parse      | 158 ms                                                                 | 155 ms: 1.02x faster                                                         |
| pickle_dict          | 34.3 us                                                                | 33.6 us: 1.02x faster                                                        |
| unpickle_list        | 5.10 us                                                                | 5.05 us: 1.01x faster                                                        |
| json_loads           | 27.6 us                                                                | 27.7 us: 1.00x slower                                                        |
| json_dumps           | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                        |
| pickle_pure_python   | 296 us                                                                 | 299 us: 1.01x slower                                                         |
| unpickle_pure_python | 226 us                                                                 | 229 us: 1.01x slower                                                         |
| pickle_list          | 4.98 us                                                                | 5.08 us: 1.02x slower                                                        |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (4): tomli_loads, xml_etree_iterparse, xml_etree_process, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.2 ms                                                                | 10.3 ms: 1.01x slower                                                        |
| python_startup_no_site | 8.82 ms                                                                | 8.91 ms: 1.01x slower                                                        |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 12.3 ms                                                                | 12.2 ms: 1.01x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mdp                        | 2.79 sec                                                               | 2.57 sec: 1.08x faster                                                       |
| unpickle                   | 16.0 us                                                                | 15.1 us: 1.05x faster                                                        |
| pycparser                  | 1.22 sec                                                               | 1.19 sec: 1.03x faster                                                       |
| pickle                     | 11.7 us                                                                | 11.3 us: 1.03x faster                                                        |
| fannkuch                   | 428 ms                                                                 | 418 ms: 1.02x faster                                                         |
| xml_etree_parse            | 158 ms                                                                 | 155 ms: 1.02x faster                                                         |
| coverage                   | 96.6 ms                                                                | 94.8 ms: 1.02x faster                                                        |
| pickle_dict                | 34.3 us                                                                | 33.6 us: 1.02x faster                                                        |
| regex_dna                  | 225 ms                                                                 | 222 ms: 1.01x faster                                                         |
| pyflate                    | 510 ms                                                                 | 504 ms: 1.01x faster                                                         |
| generators                 | 29.5 ms                                                                | 29.2 ms: 1.01x faster                                                        |
| coroutines                 | 23.1 ms                                                                | 22.8 ms: 1.01x faster                                                        |
| unpickle_list              | 5.10 us                                                                | 5.05 us: 1.01x faster                                                        |
| meteor_contest             | 111 ms                                                                 | 110 ms: 1.01x faster                                                         |
| mako                       | 12.3 ms                                                                | 12.2 ms: 1.01x faster                                                        |
| typing_runtime_protocols   | 112 us                                                                 | 111 us: 1.01x faster                                                         |
| comprehensions             | 18.3 us                                                                | 18.2 us: 1.01x faster                                                        |
| dulwich_log                | 68.1 ms                                                                | 67.9 ms: 1.00x faster                                                        |
| pidigits                   | 188 ms                                                                 | 188 ms: 1.00x faster                                                         |
| gc_traversal               | 3.85 ms                                                                | 3.85 ms: 1.00x slower                                                        |
| asyncio_tcp_ssl            | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                       |
| docutils                   | 2.64 sec                                                               | 2.65 sec: 1.00x slower                                                       |
| json_loads                 | 27.6 us                                                                | 27.7 us: 1.00x slower                                                        |
| go                         | 148 ms                                                                 | 149 ms: 1.00x slower                                                         |
| richards                   | 44.9 ms                                                                | 45.1 ms: 1.01x slower                                                        |
| regex_compile              | 140 ms                                                                 | 140 ms: 1.01x slower                                                         |
| json_dumps                 | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                        |
| async_generators           | 457 ms                                                                 | 461 ms: 1.01x slower                                                         |
| async_tree_none_tg         | 452 ms                                                                 | 456 ms: 1.01x slower                                                         |
| bench_thread_pool          | 834 us                                                                 | 842 us: 1.01x slower                                                         |
| sqlglot_normalize          | 107 ms                                                                 | 108 ms: 1.01x slower                                                         |
| python_startup             | 10.2 ms                                                                | 10.3 ms: 1.01x slower                                                        |
| sympy_integrate            | 20.4 ms                                                                | 20.6 ms: 1.01x slower                                                        |
| deltablue                  | 3.35 ms                                                                | 3.39 ms: 1.01x slower                                                        |
| python_startup_no_site     | 8.82 ms                                                                | 8.91 ms: 1.01x slower                                                        |
| async_tree_memoization     | 565 ms                                                                 | 571 ms: 1.01x slower                                                         |
| hexiom                     | 7.77 ms                                                                | 7.86 ms: 1.01x slower                                                        |
| raytrace                   | 279 ms                                                                 | 283 ms: 1.01x slower                                                         |
| pprint_pformat             | 1.61 sec                                                               | 1.63 sec: 1.01x slower                                                       |
| pickle_pure_python         | 296 us                                                                 | 299 us: 1.01x slower                                                         |
| async_tree_cpu_io_mixed    | 708 ms                                                                 | 717 ms: 1.01x slower                                                         |
| scimark_lu                 | 112 ms                                                                 | 113 ms: 1.01x slower                                                         |
| regex_effbot               | 3.65 ms                                                                | 3.70 ms: 1.01x slower                                                        |
| telco                      | 8.53 ms                                                                | 8.65 ms: 1.01x slower                                                        |
| richards_super             | 50.7 ms                                                                | 51.4 ms: 1.01x slower                                                        |
| deepcopy                   | 346 us                                                                 | 351 us: 1.01x slower                                                         |
| unpickle_pure_python       | 226 us                                                                 | 229 us: 1.01x slower                                                         |
| scimark_sor                | 119 ms                                                                 | 121 ms: 1.01x slower                                                         |
| sqlite_synth               | 2.78 us                                                                | 2.82 us: 1.02x slower                                                        |
| nqueens                    | 88.8 ms                                                                | 90.2 ms: 1.02x slower                                                        |
| async_tree_cpu_io_mixed_tg | 720 ms                                                                 | 732 ms: 1.02x slower                                                         |
| scimark_monte_carlo        | 74.2 ms                                                                | 75.5 ms: 1.02x slower                                                        |
| create_gc_cycles           | 1.47 ms                                                                | 1.50 ms: 1.02x slower                                                        |
| pathlib                    | 18.2 ms                                                                | 18.6 ms: 1.02x slower                                                        |
| pickle_list                | 4.98 us                                                                | 5.08 us: 1.02x slower                                                        |
| deepcopy_memo              | 38.3 us                                                                | 39.2 us: 1.02x slower                                                        |
| async_tree_io              | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                                       |
| scimark_fft                | 366 ms                                                                 | 374 ms: 1.02x slower                                                         |
| async_tree_io_tg           | 1.18 sec                                                               | 1.21 sec: 1.02x slower                                                       |
| logging_silent             | 100 ns                                                                 | 103 ns: 1.03x slower                                                         |
| nbody                      | 101 ms                                                                 | 104 ms: 1.03x slower                                                         |
| scimark_sparse_mat_mult    | 5.33 ms                                                                | 5.55 ms: 1.04x slower                                                        |
| unpack_sequence            | 52.7 ns                                                                | 58.0 ns: 1.10x slower                                                        |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (30): tomli_loads, spectral_norm, logging_simple, pprint_safe_repr, mypy2, sqlglot_parse, chameleon, sympy_expand, async_tree_memoization_tg, xml_etree_iterparse, asyncio_websockets, sympy_str, sympy_sum, float, regex_v8, deepcopy_reduce, sqlglot_optimize, sqlglot_transpile, logging_format, bench_mp_pool, json, xml_etree_process, 2to3, tornado_http, asyncio_tcp, dask, xml_etree_generate, crypto_pyaes, chaos, async_tree_none


# HPT report

- Reliability score: 99.19% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x