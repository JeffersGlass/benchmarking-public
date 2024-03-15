# Results vs. base

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: 939c26f
- commit date: 2024-02-01
- overall geometric mean: 1.00x faster
- HPT reliability: 99.62%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| docutils       | 2.70 sec                                                               | 2.73 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (3): 2to3, chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io      | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| async_tree_io_tg   | 1.21 sec                                                               | 1.20 sec: 1.00x faster                                                           |
| async_tree_none_tg | 458 ms                                                                 | 459 ms: 1.00x slower                                                             |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 125 ms                                                                 | 119 ms: 1.05x faster                                                             |
| float          | 102 ms                                                                 | 100 ms: 1.02x faster                                                             |
| pidigits       | 189 ms                                                                 | 190 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.69 ms                                                                | 3.65 ms: 1.01x faster                                                            |
| regex_compile  | 156 ms                                                                 | 154 ms: 1.01x faster                                                             |
| regex_dna      | 221 ms                                                                 | 220 ms: 1.00x faster                                                             |
| regex_v8       | 24.5 ms                                                                | 24.6 ms: 1.00x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_list          | 5.19 us                                                                | 4.93 us: 1.05x faster                                                            |
| pickle_dict          | 34.6 us                                                                | 33.2 us: 1.04x faster                                                            |
| pickle_pure_python   | 306 us                                                                 | 298 us: 1.03x faster                                                             |
| unpickle_pure_python | 241 us                                                                 | 237 us: 1.02x faster                                                             |
| json_dumps           | 10.7 ms                                                                | 10.5 ms: 1.02x faster                                                            |
| unpickle_list        | 5.09 us                                                                | 5.01 us: 1.02x faster                                                            |
| pickle               | 11.4 us                                                                | 11.5 us: 1.00x slower                                                            |
| json_loads           | 28.3 us                                                                | 28.5 us: 1.01x slower                                                            |
| xml_etree_iterparse  | 113 ms                                                                 | 114 ms: 1.01x slower                                                             |
| xml_etree_parse      | 156 ms                                                                 | 159 ms: 1.02x slower                                                             |
| unpickle             | 15.0 us                                                                | 15.9 us: 1.07x slower                                                            |
| tomli_loads          | 2.47 sec                                                               | 2.70 sec: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): xml_etree_generate, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.81 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                                | 14.7 ms: 1.00x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240201-linux-x86_64-python-4dbb198d279a06fed74e-3.13.0a3+-4dbb198 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| scimark_fft              | 476 ms                                                                 | 447 ms: 1.06x faster                                                             |
| gc_traversal             | 3.99 ms                                                                | 3.76 ms: 1.06x faster                                                            |
| pickle_list              | 5.19 us                                                                | 4.93 us: 1.05x faster                                                            |
| nbody                    | 125 ms                                                                 | 119 ms: 1.05x faster                                                             |
| scimark_sparse_mat_mult  | 6.49 ms                                                                | 6.18 ms: 1.05x faster                                                            |
| scimark_sor              | 132 ms                                                                 | 126 ms: 1.05x faster                                                             |
| pickle_dict              | 34.6 us                                                                | 33.2 us: 1.04x faster                                                            |
| chaos                    | 76.7 ms                                                                | 74.3 ms: 1.03x faster                                                            |
| spectral_norm            | 156 ms                                                                 | 152 ms: 1.03x faster                                                             |
| pickle_pure_python       | 306 us                                                                 | 298 us: 1.03x faster                                                             |
| comprehensions           | 22.8 us                                                                | 22.3 us: 1.02x faster                                                            |
| coroutines               | 22.8 ms                                                                | 22.4 ms: 1.02x faster                                                            |
| scimark_lu               | 120 ms                                                                 | 118 ms: 1.02x faster                                                             |
| logging_format           | 6.83 us                                                                | 6.71 us: 1.02x faster                                                            |
| unpickle_pure_python     | 241 us                                                                 | 237 us: 1.02x faster                                                             |
| json_dumps               | 10.7 ms                                                                | 10.5 ms: 1.02x faster                                                            |
| telco                    | 8.87 ms                                                                | 8.73 ms: 1.02x faster                                                            |
| unpickle_list            | 5.09 us                                                                | 5.01 us: 1.02x faster                                                            |
| sqlglot_normalize        | 117 ms                                                                 | 115 ms: 1.02x faster                                                             |
| float                    | 102 ms                                                                 | 100 ms: 1.02x faster                                                             |
| scimark_monte_carlo      | 86.0 ms                                                                | 84.8 ms: 1.01x faster                                                            |
| sqlglot_transpile        | 1.69 ms                                                                | 1.67 ms: 1.01x faster                                                            |
| sqlglot_parse            | 1.36 ms                                                                | 1.34 ms: 1.01x faster                                                            |
| regex_effbot             | 3.69 ms                                                                | 3.65 ms: 1.01x faster                                                            |
| sqlglot_optimize         | 59.4 ms                                                                | 58.9 ms: 1.01x faster                                                            |
| regex_compile            | 156 ms                                                                 | 154 ms: 1.01x faster                                                             |
| deepcopy                 | 357 us                                                                 | 354 us: 1.01x faster                                                             |
| pprint_pformat           | 1.75 sec                                                               | 1.74 sec: 1.01x faster                                                           |
| typing_runtime_protocols | 116 us                                                                 | 115 us: 1.01x faster                                                             |
| pyflate                  | 538 ms                                                                 | 534 ms: 1.01x faster                                                             |
| pprint_safe_repr         | 842 ms                                                                 | 837 ms: 1.01x faster                                                             |
| async_tree_io            | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| sympy_sum                | 163 ms                                                                 | 162 ms: 1.01x faster                                                             |
| nqueens                  | 99.1 ms                                                                | 98.6 ms: 1.01x faster                                                            |
| raytrace                 | 306 ms                                                                 | 304 ms: 1.00x faster                                                             |
| asyncio_tcp              | 492 ms                                                                 | 490 ms: 1.00x faster                                                             |
| regex_dna                | 221 ms                                                                 | 220 ms: 1.00x faster                                                             |
| hexiom                   | 9.12 ms                                                                | 9.09 ms: 1.00x faster                                                            |
| mako                     | 14.7 ms                                                                | 14.7 ms: 1.00x faster                                                            |
| async_tree_io_tg         | 1.21 sec                                                               | 1.20 sec: 1.00x faster                                                           |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.79 sec: 1.00x faster                                                           |
| sympy_integrate          | 21.4 ms                                                                | 21.4 ms: 1.00x faster                                                            |
| async_tree_none_tg       | 458 ms                                                                 | 459 ms: 1.00x slower                                                             |
| regex_v8                 | 24.5 ms                                                                | 24.6 ms: 1.00x slower                                                            |
| pidigits                 | 189 ms                                                                 | 190 ms: 1.00x slower                                                             |
| pickle                   | 11.4 us                                                                | 11.5 us: 1.00x slower                                                            |
| pycparser                | 1.24 sec                                                               | 1.25 sec: 1.01x slower                                                           |
| docutils                 | 2.70 sec                                                               | 2.73 sec: 1.01x slower                                                           |
| python_startup           | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site   | 8.73 ms                                                                | 8.81 ms: 1.01x slower                                                            |
| sqlite_synth             | 2.88 us                                                                | 2.91 us: 1.01x slower                                                            |
| json_loads               | 28.3 us                                                                | 28.5 us: 1.01x slower                                                            |
| xml_etree_iterparse      | 113 ms                                                                 | 114 ms: 1.01x slower                                                             |
| go                       | 160 ms                                                                 | 162 ms: 1.01x slower                                                             |
| meteor_contest           | 116 ms                                                                 | 118 ms: 1.01x slower                                                             |
| logging_silent           | 103 ns                                                                 | 105 ns: 1.01x slower                                                             |
| fannkuch                 | 458 ms                                                                 | 463 ms: 1.01x slower                                                             |
| create_gc_cycles         | 1.48 ms                                                                | 1.50 ms: 1.01x slower                                                            |
| unpack_sequence          | 39.0 ns                                                                | 39.6 ns: 1.01x slower                                                            |
| deepcopy_reduce          | 3.12 us                                                                | 3.17 us: 1.02x slower                                                            |
| xml_etree_parse          | 156 ms                                                                 | 159 ms: 1.02x slower                                                             |
| coverage                 | 94.7 ms                                                                | 96.9 ms: 1.02x slower                                                            |
| mdp                      | 2.68 sec                                                               | 2.79 sec: 1.04x slower                                                           |
| unpickle                 | 15.0 us                                                                | 15.9 us: 1.07x slower                                                            |
| tomli_loads              | 2.47 sec                                                               | 2.70 sec: 1.09x slower                                                           |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (28): sympy_str, chameleon, async_tree_cpu_io_mixed, mypy2, json, async_tree_cpu_io_mixed_tg, asyncio_websockets, dask, generators, crypto_pyaes, 2to3, xml_etree_generate, bench_mp_pool, pathlib, dulwich_log, deltablue, async_tree_memoization_tg, bench_thread_pool, async_tree_memoization, richards_super, deepcopy_memo, async_generators, xml_etree_process, sympy_expand, async_tree_none, richards, logging_simple, tornado_http


# HPT report

- Reliability score: 99.62% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x