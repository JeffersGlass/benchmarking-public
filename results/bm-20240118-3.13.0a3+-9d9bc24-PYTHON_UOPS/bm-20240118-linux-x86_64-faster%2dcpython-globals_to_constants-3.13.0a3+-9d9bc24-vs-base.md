# Results vs. base

- fork: faster-cpython
- ref: globals_to_constants
- machine: linux-x86_64
- commit hash: 9d9bc24
- commit date: 2024-01-18
- overall geometric mean: 1.00x faster
- HPT reliability: 76.61%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| docutils       | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| tornado_http   | 98.7 ms                                                                | 101 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): 2to3, chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io_tg   | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| async_tree_none_tg | 457 ms                                                                 | 455 ms: 1.00x faster                                                             |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 92.8 ms                                                                | 91.1 ms: 1.02x faster                                                            |
| nbody          | 119 ms                                                                 | 118 ms: 1.00x faster                                                             |
| pidigits       | 188 ms                                                                 | 189 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.71 ms                                                                | 3.53 ms: 1.05x faster                                                            |
| regex_v8       | 24.9 ms                                                                | 24.8 ms: 1.00x faster                                                            |
| regex_compile  | 152 ms                                                                 | 151 ms: 1.00x faster                                                             |
| regex_dna      | 219 ms                                                                 | 225 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_dict          | 33.8 us                                                                | 33.0 us: 1.02x faster                                                            |
| pickle               | 11.6 us                                                                | 11.3 us: 1.02x faster                                                            |
| xml_etree_parse      | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| tomli_loads          | 2.42 sec                                                               | 2.39 sec: 1.02x faster                                                           |
| pickle_list          | 5.02 us                                                                | 4.95 us: 1.01x faster                                                            |
| xml_etree_iterparse  | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| unpickle_list        | 5.35 us                                                                | 5.33 us: 1.00x faster                                                            |
| json_loads           | 28.3 us                                                                | 28.2 us: 1.00x faster                                                            |
| unpickle             | 15.0 us                                                                | 15.0 us: 1.00x faster                                                            |
| json_dumps           | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| xml_etree_process    | 60.9 ms                                                                | 61.4 ms: 1.01x slower                                                            |
| xml_etree_generate   | 89.0 ms                                                                | 90.1 ms: 1.01x slower                                                            |
| unpickle_pure_python | 234 us                                                                 | 237 us: 1.01x slower                                                             |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 8.73 ms                                                                | 8.73 ms: 1.00x faster                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 14.0 ms: 1.01x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence          | 49.3 ns                                                                | 40.3 ns: 1.23x faster                                                            |
| regex_effbot             | 3.71 ms                                                                | 3.53 ms: 1.05x faster                                                            |
| pycparser                | 1.25 sec                                                               | 1.21 sec: 1.03x faster                                                           |
| scimark_sparse_mat_mult  | 6.09 ms                                                                | 5.91 ms: 1.03x faster                                                            |
| telco                    | 8.76 ms                                                                | 8.56 ms: 1.02x faster                                                            |
| pickle_dict              | 33.8 us                                                                | 33.0 us: 1.02x faster                                                            |
| pickle                   | 11.6 us                                                                | 11.3 us: 1.02x faster                                                            |
| float                    | 92.8 ms                                                                | 91.1 ms: 1.02x faster                                                            |
| deepcopy_reduce          | 3.19 us                                                                | 3.14 us: 1.02x faster                                                            |
| mdp                      | 2.67 sec                                                               | 2.63 sec: 1.02x faster                                                           |
| xml_etree_parse          | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| async_generators         | 464 ms                                                                 | 457 ms: 1.02x faster                                                             |
| tomli_loads              | 2.42 sec                                                               | 2.39 sec: 1.02x faster                                                           |
| asyncio_tcp              | 490 ms                                                                 | 483 ms: 1.02x faster                                                             |
| typing_runtime_protocols | 117 us                                                                 | 115 us: 1.02x faster                                                             |
| pickle_list              | 5.02 us                                                                | 4.95 us: 1.01x faster                                                            |
| raytrace                 | 303 ms                                                                 | 300 ms: 1.01x faster                                                             |
| xml_etree_iterparse      | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| create_gc_cycles         | 1.48 ms                                                                | 1.47 ms: 1.01x faster                                                            |
| mako                     | 14.1 ms                                                                | 14.0 ms: 1.01x faster                                                            |
| async_tree_io_tg         | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| pathlib                  | 18.5 ms                                                                | 18.4 ms: 1.01x faster                                                            |
| chaos                    | 74.1 ms                                                                | 73.7 ms: 1.01x faster                                                            |
| pprint_safe_repr         | 822 ms                                                                 | 818 ms: 1.00x faster                                                             |
| regex_v8                 | 24.9 ms                                                                | 24.8 ms: 1.00x faster                                                            |
| unpickle_list            | 5.35 us                                                                | 5.33 us: 1.00x faster                                                            |
| docutils                 | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| nbody                    | 119 ms                                                                 | 118 ms: 1.00x faster                                                             |
| async_tree_none_tg       | 457 ms                                                                 | 455 ms: 1.00x faster                                                             |
| json_loads               | 28.3 us                                                                | 28.2 us: 1.00x faster                                                            |
| regex_compile            | 152 ms                                                                 | 151 ms: 1.00x faster                                                             |
| asyncio_tcp_ssl          | 1.81 sec                                                               | 1.80 sec: 1.00x faster                                                           |
| unpickle                 | 15.0 us                                                                | 15.0 us: 1.00x faster                                                            |
| python_startup_no_site   | 8.73 ms                                                                | 8.73 ms: 1.00x faster                                                            |
| pidigits                 | 188 ms                                                                 | 189 ms: 1.00x slower                                                             |
| bench_thread_pool        | 846 us                                                                 | 848 us: 1.00x slower                                                             |
| sqlglot_normalize        | 114 ms                                                                 | 115 ms: 1.00x slower                                                             |
| sqlglot_optimize         | 57.6 ms                                                                | 57.9 ms: 1.00x slower                                                            |
| deltablue                | 4.72 ms                                                                | 4.74 ms: 1.00x slower                                                            |
| sympy_integrate          | 21.1 ms                                                                | 21.1 ms: 1.00x slower                                                            |
| crypto_pyaes             | 82.6 ms                                                                | 83.0 ms: 1.01x slower                                                            |
| sympy_sum                | 159 ms                                                                 | 160 ms: 1.01x slower                                                             |
| pyflate                  | 529 ms                                                                 | 532 ms: 1.01x slower                                                             |
| hexiom                   | 8.36 ms                                                                | 8.42 ms: 1.01x slower                                                            |
| json_dumps               | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| xml_etree_process        | 60.9 ms                                                                | 61.4 ms: 1.01x slower                                                            |
| generators               | 29.9 ms                                                                | 30.1 ms: 1.01x slower                                                            |
| go                       | 154 ms                                                                 | 155 ms: 1.01x slower                                                             |
| nqueens                  | 93.5 ms                                                                | 94.6 ms: 1.01x slower                                                            |
| xml_etree_generate       | 89.0 ms                                                                | 90.1 ms: 1.01x slower                                                            |
| fannkuch                 | 450 ms                                                                 | 455 ms: 1.01x slower                                                             |
| unpickle_pure_python     | 234 us                                                                 | 237 us: 1.01x slower                                                             |
| sqlite_synth             | 2.88 us                                                                | 2.92 us: 1.01x slower                                                            |
| logging_format           | 6.80 us                                                                | 6.90 us: 1.01x slower                                                            |
| spectral_norm            | 144 ms                                                                 | 147 ms: 1.02x slower                                                             |
| logging_silent           | 104 ns                                                                 | 107 ns: 1.02x slower                                                             |
| scimark_lu               | 118 ms                                                                 | 121 ms: 1.02x slower                                                             |
| tornado_http             | 98.7 ms                                                                | 101 ms: 1.03x slower                                                             |
| regex_dna                | 219 ms                                                                 | 225 ms: 1.03x slower                                                             |
| coroutines               | 22.0 ms                                                                | 22.8 ms: 1.04x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (33): richards_super, sympy_str, chameleon, async_tree_memoization_tg, sqlglot_transpile, scimark_monte_carlo, dask, pprint_pformat, json, asyncio_websockets, async_tree_io, async_tree_cpu_io_mixed_tg, meteor_contest, gc_traversal, deepcopy_memo, bench_mp_pool, python_startup, comprehensions, deepcopy, async_tree_memoization, sympy_expand, sqlglot_parse, async_tree_cpu_io_mixed, 2to3, dulwich_log, pickle_pure_python, async_tree_none, coverage, richards, scimark_fft, mypy2, logging_simple, scimark_sor


# HPT report

- Reliability score: 76.61% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x