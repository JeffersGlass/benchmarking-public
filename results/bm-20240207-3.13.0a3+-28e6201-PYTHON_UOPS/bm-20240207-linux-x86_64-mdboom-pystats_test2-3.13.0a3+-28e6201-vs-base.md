# Results vs. base

- fork: mdboom
- ref: pystats_test2
- machine: linux-x86_64
- commit hash: 28e6201
- commit date: 2024-02-07
- overall geometric mean: 1.00x slower
- HPT reliability: 86.72%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3+-2091fb2 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 281 ms                                                                 | 280 ms: 1.00x faster                                            |
| chameleon      | 7.16 ms                                                                | 7.24 ms: 1.01x slower                                           |
| docutils       | 2.68 sec                                                               | 2.70 sec: 1.01x slower                                          |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_io, async_tree_none_tg, async_tree_none, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3+-2091fb2 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 117 ms                                                                 | 115 ms: 1.02x faster                                            |
| pidigits       | 189 ms                                                                 | 188 ms: 1.01x faster                                            |
| float          | 89.0 ms                                                                | 89.7 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3+-2091fb2 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna      | 226 ms                                                                 | 220 ms: 1.03x faster                                            |
| regex_effbot   | 3.62 ms                                                                | 3.57 ms: 1.01x faster                                           |
| regex_compile  | 147 ms                                                                 | 147 ms: 1.00x faster                                            |
| regex_v8       | 25.0 ms                                                                | 25.3 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3+-2091fb2 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|---------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| xml_etree_generate  | 89.8 ms                                                                | 88.0 ms: 1.02x faster                                           |
| xml_etree_process   | 61.3 ms                                                                | 60.2 ms: 1.02x faster                                           |
| pickle_pure_python  | 305 us                                                                 | 300 us: 1.01x faster                                            |
| xml_etree_iterparse | 109 ms                                                                 | 108 ms: 1.01x faster                                            |
| json_dumps          | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                           |
| pickle_list         | 4.90 us                                                                | 5.06 us: 1.03x slower                                           |
| pickle              | 11.4 us                                                                | 11.7 us: 1.03x slower                                           |
| pickle_dict         | 32.8 us                                                                | 34.0 us: 1.04x slower                                           |
| tomli_loads         | 2.34 sec                                                               | 2.54 sec: 1.08x slower                                          |
| unpickle            | 15.1 us                                                                | 17.1 us: 1.13x slower                                           |
| Geometric mean      | (ref)                                                                  | 1.02x slower                                                    |

Benchmark hidden because not significant (4): unpickle_list, json_loads, xml_etree_parse, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3+-2091fb2 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                           |
| python_startup_no_site | 8.72 ms                                                                | 8.77 ms: 1.01x slower                                           |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3+-2091fb2 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|-----------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 13.2 ms                                                                | 13.1 ms: 1.01x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20240202-linux-x86_64-python-2091fb2a85c1aa2d9b22-3.13.0a3+-2091fb2 | bm-20240207-linux-x86_64-mdboom-pystats_test2-3.13.0a3+-28e6201 |
|--------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| deltablue                | 4.46 ms                                                                | 3.50 ms: 1.28x faster                                           |
| scimark_sor              | 132 ms                                                                 | 124 ms: 1.06x faster                                            |
| regex_dna                | 226 ms                                                                 | 220 ms: 1.03x faster                                            |
| coroutines               | 22.3 ms                                                                | 21.6 ms: 1.03x faster                                           |
| pprint_safe_repr         | 805 ms                                                                 | 783 ms: 1.03x faster                                            |
| spectral_norm            | 141 ms                                                                 | 137 ms: 1.03x faster                                            |
| scimark_sparse_mat_mult  | 5.65 ms                                                                | 5.49 ms: 1.03x faster                                           |
| nqueens                  | 93.6 ms                                                                | 91.6 ms: 1.02x faster                                           |
| pprint_pformat           | 1.66 sec                                                               | 1.62 sec: 1.02x faster                                          |
| xml_etree_generate       | 89.8 ms                                                                | 88.0 ms: 1.02x faster                                           |
| xml_etree_process        | 61.3 ms                                                                | 60.2 ms: 1.02x faster                                           |
| sqlglot_normalize        | 114 ms                                                                 | 112 ms: 1.02x faster                                            |
| richards_super           | 55.2 ms                                                                | 54.3 ms: 1.02x faster                                           |
| nbody                    | 117 ms                                                                 | 115 ms: 1.02x faster                                            |
| logging_silent           | 103 ns                                                                 | 101 ns: 1.02x faster                                            |
| pathlib                  | 18.7 ms                                                                | 18.4 ms: 1.02x faster                                           |
| pickle_pure_python       | 305 us                                                                 | 300 us: 1.01x faster                                            |
| scimark_lu               | 117 ms                                                                 | 116 ms: 1.01x faster                                            |
| scimark_monte_carlo      | 78.5 ms                                                                | 77.5 ms: 1.01x faster                                           |
| regex_effbot             | 3.62 ms                                                                | 3.57 ms: 1.01x faster                                           |
| xml_etree_iterparse      | 109 ms                                                                 | 108 ms: 1.01x faster                                            |
| sqlite_synth             | 2.89 us                                                                | 2.86 us: 1.01x faster                                           |
| mdp                      | 2.67 sec                                                               | 2.64 sec: 1.01x faster                                          |
| async_generators         | 458 ms                                                                 | 453 ms: 1.01x faster                                            |
| sqlglot_optimize         | 57.7 ms                                                                | 57.1 ms: 1.01x faster                                           |
| richards                 | 48.8 ms                                                                | 48.4 ms: 1.01x faster                                           |
| mako                     | 13.2 ms                                                                | 13.1 ms: 1.01x faster                                           |
| pidigits                 | 189 ms                                                                 | 188 ms: 1.01x faster                                            |
| crypto_pyaes             | 80.7 ms                                                                | 80.3 ms: 1.00x faster                                           |
| regex_compile            | 147 ms                                                                 | 147 ms: 1.00x faster                                            |
| bench_thread_pool        | 845 us                                                                 | 842 us: 1.00x faster                                            |
| asyncio_tcp              | 490 ms                                                                 | 489 ms: 1.00x faster                                            |
| create_gc_cycles         | 1.48 ms                                                                | 1.48 ms: 1.00x faster                                           |
| 2to3                     | 281 ms                                                                 | 280 ms: 1.00x faster                                            |
| hexiom                   | 8.02 ms                                                                | 8.04 ms: 1.00x slower                                           |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                           |
| asyncio_tcp_ssl          | 1.79 sec                                                               | 1.80 sec: 1.00x slower                                          |
| deepcopy_memo            | 39.8 us                                                                | 40.0 us: 1.00x slower                                           |
| dulwich_log              | 68.4 ms                                                                | 68.8 ms: 1.01x slower                                           |
| python_startup_no_site   | 8.72 ms                                                                | 8.77 ms: 1.01x slower                                           |
| docutils                 | 2.68 sec                                                               | 2.70 sec: 1.01x slower                                          |
| sympy_integrate          | 20.9 ms                                                                | 21.0 ms: 1.01x slower                                           |
| json_dumps               | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                           |
| float                    | 89.0 ms                                                                | 89.7 ms: 1.01x slower                                           |
| dask                     | 364 ms                                                                 | 368 ms: 1.01x slower                                            |
| regex_v8                 | 25.0 ms                                                                | 25.3 ms: 1.01x slower                                           |
| chameleon                | 7.16 ms                                                                | 7.24 ms: 1.01x slower                                           |
| typing_runtime_protocols | 114 us                                                                 | 116 us: 1.01x slower                                            |
| sympy_sum                | 158 ms                                                                 | 160 ms: 1.01x slower                                            |
| logging_format           | 6.70 us                                                                | 6.80 us: 1.02x slower                                           |
| deepcopy_reduce          | 3.10 us                                                                | 3.20 us: 1.03x slower                                           |
| pickle_list              | 4.90 us                                                                | 5.06 us: 1.03x slower                                           |
| pickle                   | 11.4 us                                                                | 11.7 us: 1.03x slower                                           |
| pickle_dict              | 32.8 us                                                                | 34.0 us: 1.04x slower                                           |
| pycparser                | 1.20 sec                                                               | 1.25 sec: 1.04x slower                                          |
| unpack_sequence          | 38.7 ns                                                                | 41.3 ns: 1.06x slower                                           |
| tomli_loads              | 2.34 sec                                                               | 2.54 sec: 1.08x slower                                          |
| gc_traversal             | 3.49 ms                                                                | 3.81 ms: 1.09x slower                                           |
| go                       | 156 ms                                                                 | 172 ms: 1.11x slower                                            |
| unpickle                 | 15.1 us                                                                | 17.1 us: 1.13x slower                                           |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                    |

Benchmark hidden because not significant (33): unpickle_list, telco, json, sqlglot_parse, logging_simple, sympy_expand, scimark_fft, sqlglot_transpile, comprehensions, asyncio_websockets, async_tree_cpu_io_mixed_tg, meteor_contest, chaos, coverage, bench_mp_pool, async_tree_io_tg, json_loads, sympy_str, xml_etree_parse, fannkuch, raytrace, async_tree_cpu_io_mixed, generators, unpickle_pure_python, async_tree_memoization, async_tree_io, tornado_http, async_tree_none_tg, deepcopy, pyflate, async_tree_none, mypy2, async_tree_memoization_tg


# HPT report

- Reliability score: 86.72% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x