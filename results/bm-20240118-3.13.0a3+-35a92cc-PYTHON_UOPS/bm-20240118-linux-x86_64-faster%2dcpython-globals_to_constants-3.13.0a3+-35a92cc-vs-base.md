# Results vs. base

- fork: faster-cpython
- ref: globals_to_constants
- machine: linux-x86_64
- commit hash: 35a92cc
- commit date: 2024-01-18
- overall geometric mean: 1.01x faster
- HPT reliability: 99.87%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 281 ms: 1.01x faster                                                             |
| docutils       | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| tornado_http   | 98.7 ms                                                                | 101 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io    | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| async_tree_io_tg | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| Geometric mean   | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_none_tg, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 119 ms                                                                 | 111 ms: 1.07x faster                                                             |
| float          | 92.8 ms                                                                | 90.0 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.71 ms                                                                | 3.52 ms: 1.05x faster                                                            |
| regex_compile  | 152 ms                                                                 | 149 ms: 1.02x faster                                                             |
| regex_v8       | 24.9 ms                                                                | 25.0 ms: 1.00x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_list          | 5.02 us                                                                | 4.85 us: 1.03x faster                                                            |
| xml_etree_iterparse  | 111 ms                                                                 | 109 ms: 1.02x faster                                                             |
| xml_etree_parse      | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| unpickle             | 15.0 us                                                                | 14.8 us: 1.02x faster                                                            |
| pickle               | 11.6 us                                                                | 11.4 us: 1.01x faster                                                            |
| xml_etree_generate   | 89.0 ms                                                                | 88.0 ms: 1.01x faster                                                            |
| unpickle_pure_python | 234 us                                                                 | 231 us: 1.01x faster                                                             |
| json_loads           | 28.3 us                                                                | 28.1 us: 1.01x faster                                                            |
| xml_etree_process    | 60.9 ms                                                                | 60.4 ms: 1.01x faster                                                            |
| json_dumps           | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| unpickle_list        | 5.35 us                                                                | 5.45 us: 1.02x slower                                                            |
| pickle_dict          | 33.8 us                                                                | 35.1 us: 1.04x slower                                                            |
| tomli_loads          | 2.42 sec                                                               | 2.55 sec: 1.05x slower                                                           |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.72 ms: 1.00x faster                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 13.2 ms: 1.07x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| deltablue                | 4.72 ms                                                                | 3.51 ms: 1.34x faster                                                            |
| unpack_sequence          | 49.3 ns                                                                | 40.7 ns: 1.21x faster                                                            |
| nbody                    | 119 ms                                                                 | 111 ms: 1.07x faster                                                             |
| mako                     | 14.1 ms                                                                | 13.2 ms: 1.07x faster                                                            |
| regex_effbot             | 3.71 ms                                                                | 3.52 ms: 1.05x faster                                                            |
| scimark_sor              | 130 ms                                                                 | 124 ms: 1.05x faster                                                             |
| scimark_sparse_mat_mult  | 6.09 ms                                                                | 5.80 ms: 1.05x faster                                                            |
| scimark_fft              | 455 ms                                                                 | 436 ms: 1.04x faster                                                             |
| hexiom                   | 8.36 ms                                                                | 8.04 ms: 1.04x faster                                                            |
| pprint_safe_repr         | 822 ms                                                                 | 794 ms: 1.04x faster                                                             |
| pickle_list              | 5.02 us                                                                | 4.85 us: 1.03x faster                                                            |
| chaos                    | 74.1 ms                                                                | 71.7 ms: 1.03x faster                                                            |
| float                    | 92.8 ms                                                                | 90.0 ms: 1.03x faster                                                            |
| comprehensions           | 21.3 us                                                                | 20.6 us: 1.03x faster                                                            |
| spectral_norm            | 144 ms                                                                 | 140 ms: 1.03x faster                                                             |
| async_generators         | 464 ms                                                                 | 451 ms: 1.03x faster                                                             |
| pprint_pformat           | 1.70 sec                                                               | 1.66 sec: 1.03x faster                                                           |
| scimark_monte_carlo      | 80.5 ms                                                                | 78.4 ms: 1.03x faster                                                            |
| fannkuch                 | 450 ms                                                                 | 439 ms: 1.03x faster                                                             |
| raytrace                 | 303 ms                                                                 | 296 ms: 1.03x faster                                                             |
| xml_etree_iterparse      | 111 ms                                                                 | 109 ms: 1.02x faster                                                             |
| deepcopy_memo            | 40.9 us                                                                | 40.0 us: 1.02x faster                                                            |
| telco                    | 8.76 ms                                                                | 8.57 ms: 1.02x faster                                                            |
| typing_runtime_protocols | 117 us                                                                 | 114 us: 1.02x faster                                                             |
| xml_etree_parse          | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| asyncio_tcp              | 490 ms                                                                 | 482 ms: 1.02x faster                                                             |
| regex_compile            | 152 ms                                                                 | 149 ms: 1.02x faster                                                             |
| json                     | 5.23 ms                                                                | 5.14 ms: 1.02x faster                                                            |
| unpickle                 | 15.0 us                                                                | 14.8 us: 1.02x faster                                                            |
| pyflate                  | 529 ms                                                                 | 521 ms: 1.02x faster                                                             |
| meteor_contest           | 115 ms                                                                 | 114 ms: 1.01x faster                                                             |
| pickle                   | 11.6 us                                                                | 11.4 us: 1.01x faster                                                            |
| xml_etree_generate       | 89.0 ms                                                                | 88.0 ms: 1.01x faster                                                            |
| crypto_pyaes             | 82.6 ms                                                                | 81.6 ms: 1.01x faster                                                            |
| unpickle_pure_python     | 234 us                                                                 | 231 us: 1.01x faster                                                             |
| json_loads               | 28.3 us                                                                | 28.1 us: 1.01x faster                                                            |
| async_tree_io            | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| xml_etree_process        | 60.9 ms                                                                | 60.4 ms: 1.01x faster                                                            |
| sqlite_synth             | 2.88 us                                                                | 2.86 us: 1.01x faster                                                            |
| async_tree_io_tg         | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| asyncio_tcp_ssl          | 1.81 sec                                                               | 1.79 sec: 1.01x faster                                                           |
| bench_thread_pool        | 846 us                                                                 | 841 us: 1.01x faster                                                             |
| generators               | 29.9 ms                                                                | 29.7 ms: 1.01x faster                                                            |
| logging_format           | 6.80 us                                                                | 6.76 us: 1.01x faster                                                            |
| 2to3                     | 282 ms                                                                 | 281 ms: 1.01x faster                                                             |
| mdp                      | 2.67 sec                                                               | 2.66 sec: 1.00x faster                                                           |
| docutils                 | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                            |
| python_startup_no_site   | 8.73 ms                                                                | 8.72 ms: 1.00x faster                                                            |
| regex_v8                 | 24.9 ms                                                                | 25.0 ms: 1.00x slower                                                            |
| sympy_integrate          | 21.1 ms                                                                | 21.1 ms: 1.00x slower                                                            |
| sqlglot_optimize         | 57.6 ms                                                                | 57.9 ms: 1.01x slower                                                            |
| sympy_expand             | 485 ms                                                                 | 488 ms: 1.01x slower                                                             |
| logging_simple           | 6.05 us                                                                | 6.10 us: 1.01x slower                                                            |
| scimark_lu               | 118 ms                                                                 | 119 ms: 1.01x slower                                                             |
| create_gc_cycles         | 1.48 ms                                                                | 1.49 ms: 1.01x slower                                                            |
| sqlglot_parse            | 1.32 ms                                                                | 1.33 ms: 1.01x slower                                                            |
| deepcopy_reduce          | 3.19 us                                                                | 3.22 us: 1.01x slower                                                            |
| logging_silent           | 104 ns                                                                 | 105 ns: 1.01x slower                                                             |
| json_dumps               | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| sympy_sum                | 159 ms                                                                 | 161 ms: 1.01x slower                                                             |
| unpickle_list            | 5.35 us                                                                | 5.45 us: 1.02x slower                                                            |
| tornado_http             | 98.7 ms                                                                | 101 ms: 1.02x slower                                                             |
| sympy_str                | 294 ms                                                                 | 303 ms: 1.03x slower                                                             |
| coroutines               | 22.0 ms                                                                | 22.6 ms: 1.03x slower                                                            |
| pickle_dict              | 33.8 us                                                                | 35.1 us: 1.04x slower                                                            |
| tomli_loads              | 2.42 sec                                                               | 2.55 sec: 1.05x slower                                                           |
| go                       | 154 ms                                                                 | 174 ms: 1.13x slower                                                             |
| Geometric mean           | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (25): chameleon, async_tree_memoization_tg, richards_super, pickle_pure_python, deepcopy, nqueens, pathlib, asyncio_websockets, gc_traversal, dulwich_log, bench_mp_pool, regex_dna, async_tree_none_tg, pidigits, async_tree_none, pycparser, async_tree_cpu_io_mixed_tg, mypy2, async_tree_cpu_io_mixed, sqlglot_normalize, dask, async_tree_memoization, coverage, richards, sqlglot_transpile


# HPT report

- Reliability score: 99.87% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x