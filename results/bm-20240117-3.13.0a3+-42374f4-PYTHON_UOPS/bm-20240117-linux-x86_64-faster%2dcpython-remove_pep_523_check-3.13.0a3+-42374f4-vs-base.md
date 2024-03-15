# Results vs. base

- fork: faster-cpython
- ref: remove_pep_523_check
- machine: linux-x86_64
- commit hash: 42374f4
- commit date: 2024-01-17
- overall geometric mean: 1.00x faster
- HPT reliability: 98.95%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 281 ms                                                                 | 282 ms: 1.00x slower                                                             |
| chameleon      | 7.38 ms                                                                | 7.31 ms: 1.01x faster                                                            |
| docutils       | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg     | 455 ms                                                                 | 457 ms: 1.01x slower                                                             |
| async_tree_io          | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                           |
| async_tree_memoization | 570 ms                                                                 | 576 ms: 1.01x slower                                                             |
| async_tree_io_tg       | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                           |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (4): async_tree_none, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 116 ms                                                                 | 114 ms: 1.01x faster                                                             |
| float          | 91.2 ms                                                                | 90.3 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_v8       | 27.3 ms                                                                | 24.9 ms: 1.10x faster                                                            |
| regex_effbot   | 3.64 ms                                                                | 3.52 ms: 1.03x faster                                                            |
| regex_compile  | 150 ms                                                                 | 149 ms: 1.01x faster                                                             |
| regex_dna      | 218 ms                                                                 | 223 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.27 us                                                                | 5.06 us: 1.04x faster                                                            |
| tomli_loads          | 2.39 sec                                                               | 2.34 sec: 1.02x faster                                                           |
| xml_etree_generate   | 89.2 ms                                                                | 88.2 ms: 1.01x faster                                                            |
| pickle               | 11.7 us                                                                | 11.6 us: 1.01x faster                                                            |
| xml_etree_process    | 60.8 ms                                                                | 60.3 ms: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                                 | 158 ms: 1.01x faster                                                             |
| json_loads           | 28.5 us                                                                | 28.3 us: 1.01x faster                                                            |
| pickle_pure_python   | 302 us                                                                 | 300 us: 1.01x faster                                                             |
| unpickle_pure_python | 235 us                                                                 | 234 us: 1.00x faster                                                             |
| json_dumps           | 10.5 ms                                                                | 10.7 ms: 1.02x slower                                                            |
| pickle_dict          | 33.2 us                                                                | 35.0 us: 1.05x slower                                                            |
| pickle_list          | 4.91 us                                                                | 5.27 us: 1.07x slower                                                            |
| unpickle             | 15.0 us                                                                | 16.4 us: 1.10x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| python_startup_no_site | 8.74 ms                                                                | 8.78 ms: 1.00x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 13.6 ms                                                                | 13.2 ms: 1.03x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_v8                 | 27.3 ms                                                                | 24.9 ms: 1.10x faster                                                            |
| pyflate                  | 528 ms                                                                 | 504 ms: 1.05x faster                                                             |
| sympy_str                | 303 ms                                                                 | 289 ms: 1.05x faster                                                             |
| unpickle_list            | 5.27 us                                                                | 5.06 us: 1.04x faster                                                            |
| nqueens                  | 94.6 ms                                                                | 91.1 ms: 1.04x faster                                                            |
| pycparser                | 1.24 sec                                                               | 1.20 sec: 1.03x faster                                                           |
| logging_silent           | 107 ns                                                                 | 103 ns: 1.03x faster                                                             |
| regex_effbot             | 3.64 ms                                                                | 3.52 ms: 1.03x faster                                                            |
| sympy_expand             | 502 ms                                                                 | 487 ms: 1.03x faster                                                             |
| mako                     | 13.6 ms                                                                | 13.2 ms: 1.03x faster                                                            |
| logging_simple           | 6.23 us                                                                | 6.05 us: 1.03x faster                                                            |
| richards                 | 48.9 ms                                                                | 47.5 ms: 1.03x faster                                                            |
| richards_super           | 55.3 ms                                                                | 53.9 ms: 1.03x faster                                                            |
| logging_format           | 6.91 us                                                                | 6.74 us: 1.03x faster                                                            |
| typing_runtime_protocols | 117 us                                                                 | 114 us: 1.03x faster                                                             |
| tomli_loads              | 2.39 sec                                                               | 2.34 sec: 1.02x faster                                                           |
| scimark_monte_carlo      | 80.5 ms                                                                | 78.9 ms: 1.02x faster                                                            |
| sqlglot_normalize        | 116 ms                                                                 | 113 ms: 1.02x faster                                                             |
| fannkuch                 | 439 ms                                                                 | 431 ms: 1.02x faster                                                             |
| sqlglot_optimize         | 58.4 ms                                                                | 57.4 ms: 1.02x faster                                                            |
| scimark_sor              | 134 ms                                                                 | 132 ms: 1.02x faster                                                             |
| sqlite_synth             | 2.93 us                                                                | 2.88 us: 1.02x faster                                                            |
| pprint_safe_repr         | 816 ms                                                                 | 805 ms: 1.01x faster                                                             |
| hexiom                   | 8.15 ms                                                                | 8.05 ms: 1.01x faster                                                            |
| meteor_contest           | 114 ms                                                                 | 112 ms: 1.01x faster                                                             |
| coroutines               | 22.1 ms                                                                | 21.8 ms: 1.01x faster                                                            |
| xml_etree_generate       | 89.2 ms                                                                | 88.2 ms: 1.01x faster                                                            |
| nbody                    | 116 ms                                                                 | 114 ms: 1.01x faster                                                             |
| raytrace                 | 298 ms                                                                 | 295 ms: 1.01x faster                                                             |
| deepcopy_memo            | 41.5 us                                                                | 41.0 us: 1.01x faster                                                            |
| float                    | 91.2 ms                                                                | 90.3 ms: 1.01x faster                                                            |
| chameleon                | 7.38 ms                                                                | 7.31 ms: 1.01x faster                                                            |
| pickle                   | 11.7 us                                                                | 11.6 us: 1.01x faster                                                            |
| comprehensions           | 20.6 us                                                                | 20.4 us: 1.01x faster                                                            |
| sympy_sum                | 160 ms                                                                 | 159 ms: 1.01x faster                                                             |
| xml_etree_process        | 60.8 ms                                                                | 60.3 ms: 1.01x faster                                                            |
| deltablue                | 4.51 ms                                                                | 4.47 ms: 1.01x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                                | 1.32 ms: 1.01x faster                                                            |
| generators               | 29.7 ms                                                                | 29.5 ms: 1.01x faster                                                            |
| xml_etree_parse          | 159 ms                                                                 | 158 ms: 1.01x faster                                                             |
| go                       | 155 ms                                                                 | 153 ms: 1.01x faster                                                             |
| json_loads               | 28.5 us                                                                | 28.3 us: 1.01x faster                                                            |
| pickle_pure_python       | 302 us                                                                 | 300 us: 1.01x faster                                                             |
| regex_compile            | 150 ms                                                                 | 149 ms: 1.01x faster                                                             |
| chaos                    | 71.9 ms                                                                | 71.5 ms: 1.01x faster                                                            |
| sympy_integrate          | 21.1 ms                                                                | 21.0 ms: 1.01x faster                                                            |
| sqlglot_transpile        | 1.66 ms                                                                | 1.65 ms: 1.01x faster                                                            |
| pprint_pformat           | 1.69 sec                                                               | 1.68 sec: 1.01x faster                                                           |
| docutils                 | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| unpickle_pure_python     | 235 us                                                                 | 234 us: 1.00x faster                                                             |
| bench_thread_pool        | 849 us                                                                 | 846 us: 1.00x faster                                                             |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                           |
| 2to3                     | 281 ms                                                                 | 282 ms: 1.00x slower                                                             |
| deepcopy                 | 357 us                                                                 | 358 us: 1.00x slower                                                             |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| python_startup_no_site   | 8.74 ms                                                                | 8.78 ms: 1.00x slower                                                            |
| async_tree_none_tg       | 455 ms                                                                 | 457 ms: 1.01x slower                                                             |
| deepcopy_reduce          | 3.14 us                                                                | 3.16 us: 1.01x slower                                                            |
| crypto_pyaes             | 81.2 ms                                                                | 81.6 ms: 1.01x slower                                                            |
| create_gc_cycles         | 1.48 ms                                                                | 1.49 ms: 1.01x slower                                                            |
| async_tree_io            | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                           |
| gc_traversal             | 3.72 ms                                                                | 3.76 ms: 1.01x slower                                                            |
| async_tree_memoization   | 570 ms                                                                 | 576 ms: 1.01x slower                                                             |
| coverage                 | 95.2 ms                                                                | 96.4 ms: 1.01x slower                                                            |
| async_tree_io_tg         | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                           |
| async_generators         | 452 ms                                                                 | 458 ms: 1.01x slower                                                             |
| scimark_fft              | 443 ms                                                                 | 450 ms: 1.02x slower                                                             |
| json_dumps               | 10.5 ms                                                                | 10.7 ms: 1.02x slower                                                            |
| regex_dna                | 218 ms                                                                 | 223 ms: 1.02x slower                                                             |
| scimark_sparse_mat_mult  | 5.74 ms                                                                | 5.93 ms: 1.03x slower                                                            |
| mdp                      | 2.63 sec                                                               | 2.75 sec: 1.05x slower                                                           |
| pickle_dict              | 33.2 us                                                                | 35.0 us: 1.05x slower                                                            |
| pickle_list              | 4.91 us                                                                | 5.27 us: 1.07x slower                                                            |
| unpickle                 | 15.0 us                                                                | 16.4 us: 1.10x slower                                                            |
| unpack_sequence          | 38.0 ns                                                                | 43.1 ns: 1.13x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (18): pathlib, tornado_http, dask, spectral_norm, bench_mp_pool, asyncio_websockets, json, mypy2, dulwich_log, pidigits, telco, scimark_lu, asyncio_tcp, async_tree_none, xml_etree_iterparse, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg


# HPT report

- Reliability score: 98.95% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x