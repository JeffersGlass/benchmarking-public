# Results vs. base

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.00x faster
- HPT reliability: 85.70%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| chameleon      | 6.88 ms                                                                | 6.82 ms: 1.01x faster                                     |
| docutils       | 2.64 sec                                                               | 2.63 sec: 1.01x faster                                    |
| Geometric mean | (ref)                                                                  | 1.00x faster                                              |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none_tg | 450 ms                                                                 | 451 ms: 1.00x slower                                      |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                              |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_memoization, async_tree_io, async_tree_none, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| float          | 86.0 ms                                                                | 85.3 ms: 1.01x faster                                     |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                      |
| Geometric mean | (ref)                                                                  | 1.00x faster                                              |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| regex_effbot   | 3.69 ms                                                                | 3.60 ms: 1.02x faster                                     |
| regex_dna      | 221 ms                                                                 | 218 ms: 1.01x faster                                      |
| regex_compile  | 139 ms                                                                 | 140 ms: 1.01x slower                                      |
| regex_v8       | 25.1 ms                                                                | 25.4 ms: 1.01x slower                                     |
| Geometric mean | (ref)                                                                  | 1.00x faster                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| unpickle           | 16.1 us                                                                | 15.0 us: 1.07x faster                                     |
| pickle_list        | 5.25 us                                                                | 5.04 us: 1.04x faster                                     |
| pickle             | 11.7 us                                                                | 11.3 us: 1.03x faster                                     |
| pickle_pure_python | 301 us                                                                 | 294 us: 1.03x faster                                      |
| xml_etree_parse    | 156 ms                                                                 | 154 ms: 1.01x faster                                      |
| pickle_dict        | 34.3 us                                                                | 34.0 us: 1.01x faster                                     |
| xml_etree_process  | 58.6 ms                                                                | 58.2 ms: 1.01x faster                                     |
| json_dumps         | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                     |
| tomli_loads        | 2.20 sec                                                               | 2.21 sec: 1.01x slower                                    |
| json_loads         | 27.5 us                                                                | 28.2 us: 1.02x slower                                     |
| unpickle_list      | 4.97 us                                                                | 5.14 us: 1.03x slower                                     |
| Geometric mean     | (ref)                                                                  | 1.01x faster                                              |

Benchmark hidden because not significant (3): xml_etree_iterparse, unpickle_pure_python, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup_no_site | 8.86 ms                                                                | 8.81 ms: 1.01x faster                                     |
| python_startup         | 10.2 ms                                                                | 10.2 ms: 1.00x faster                                     |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 12.3 ms                                                                | 12.1 ms: 1.02x faster                                     |

All benchmarks:
===============

| Benchmark                | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| gc_traversal             | 3.83 ms                                                                | 3.53 ms: 1.09x faster                                     |
| scimark_sor              | 130 ms                                                                 | 120 ms: 1.08x faster                                      |
| unpickle                 | 16.1 us                                                                | 15.0 us: 1.07x faster                                     |
| pickle_list              | 5.25 us                                                                | 5.04 us: 1.04x faster                                     |
| pickle                   | 11.7 us                                                                | 11.3 us: 1.03x faster                                     |
| pycparser                | 1.22 sec                                                               | 1.18 sec: 1.03x faster                                    |
| logging_format           | 6.40 us                                                                | 6.22 us: 1.03x faster                                     |
| pickle_pure_python       | 301 us                                                                 | 294 us: 1.03x faster                                      |
| regex_effbot             | 3.69 ms                                                                | 3.60 ms: 1.02x faster                                     |
| create_gc_cycles         | 1.49 ms                                                                | 1.46 ms: 1.02x faster                                     |
| mako                     | 12.3 ms                                                                | 12.1 ms: 1.02x faster                                     |
| deepcopy_memo            | 39.0 us                                                                | 38.4 us: 1.02x faster                                     |
| pprint_pformat           | 1.62 sec                                                               | 1.60 sec: 1.01x faster                                    |
| deepcopy_reduce          | 3.10 us                                                                | 3.05 us: 1.01x faster                                     |
| deepcopy                 | 351 us                                                                 | 346 us: 1.01x faster                                      |
| logging_silent           | 101 ns                                                                 | 99.6 ns: 1.01x faster                                     |
| regex_dna                | 221 ms                                                                 | 218 ms: 1.01x faster                                      |
| xml_etree_parse          | 156 ms                                                                 | 154 ms: 1.01x faster                                      |
| pickle_dict              | 34.3 us                                                                | 34.0 us: 1.01x faster                                     |
| nqueens                  | 90.3 ms                                                                | 89.4 ms: 1.01x faster                                     |
| deltablue                | 3.37 ms                                                                | 3.34 ms: 1.01x faster                                     |
| chameleon                | 6.88 ms                                                                | 6.82 ms: 1.01x faster                                     |
| sympy_expand             | 478 ms                                                                 | 474 ms: 1.01x faster                                      |
| float                    | 86.0 ms                                                                | 85.3 ms: 1.01x faster                                     |
| xml_etree_process        | 58.6 ms                                                                | 58.2 ms: 1.01x faster                                     |
| sqlite_synth             | 2.83 us                                                                | 2.81 us: 1.01x faster                                     |
| logging_simple           | 5.75 us                                                                | 5.71 us: 1.01x faster                                     |
| sqlglot_normalize        | 107 ms                                                                 | 106 ms: 1.01x faster                                      |
| python_startup_no_site   | 8.86 ms                                                                | 8.81 ms: 1.01x faster                                     |
| comprehensions           | 18.2 us                                                                | 18.1 us: 1.01x faster                                     |
| docutils                 | 2.64 sec                                                               | 2.63 sec: 1.01x faster                                    |
| hexiom                   | 7.72 ms                                                                | 7.68 ms: 1.01x faster                                     |
| json_dumps               | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                     |
| sqlglot_optimize         | 55.0 ms                                                                | 54.7 ms: 1.01x faster                                     |
| async_generators         | 458 ms                                                                 | 456 ms: 1.01x faster                                      |
| generators               | 29.4 ms                                                                | 29.3 ms: 1.00x faster                                     |
| richards                 | 45.3 ms                                                                | 45.1 ms: 1.00x faster                                     |
| sympy_integrate          | 20.4 ms                                                                | 20.3 ms: 1.00x faster                                     |
| dulwich_log              | 68.1 ms                                                                | 67.9 ms: 1.00x faster                                     |
| python_startup           | 10.2 ms                                                                | 10.2 ms: 1.00x faster                                     |
| pidigits                 | 188 ms                                                                 | 187 ms: 1.00x faster                                      |
| crypto_pyaes             | 78.2 ms                                                                | 78.4 ms: 1.00x slower                                     |
| async_tree_none_tg       | 450 ms                                                                 | 451 ms: 1.00x slower                                      |
| mdp                      | 2.58 sec                                                               | 2.59 sec: 1.00x slower                                    |
| scimark_lu               | 113 ms                                                                 | 114 ms: 1.01x slower                                      |
| regex_compile            | 139 ms                                                                 | 140 ms: 1.01x slower                                      |
| asyncio_tcp              | 499 ms                                                                 | 502 ms: 1.01x slower                                      |
| spectral_norm            | 131 ms                                                                 | 132 ms: 1.01x slower                                      |
| tomli_loads              | 2.20 sec                                                               | 2.21 sec: 1.01x slower                                    |
| meteor_contest           | 108 ms                                                                 | 109 ms: 1.01x slower                                      |
| scimark_sparse_mat_mult  | 5.30 ms                                                                | 5.36 ms: 1.01x slower                                     |
| typing_runtime_protocols | 112 us                                                                 | 113 us: 1.01x slower                                      |
| regex_v8                 | 25.1 ms                                                                | 25.4 ms: 1.01x slower                                     |
| json_loads               | 27.5 us                                                                | 28.2 us: 1.02x slower                                     |
| unpickle_list            | 4.97 us                                                                | 5.14 us: 1.03x slower                                     |
| chaos                    | 69.1 ms                                                                | 71.4 ms: 1.03x slower                                     |
| unpack_sequence          | 42.6 ns                                                                | 52.7 ns: 1.24x slower                                     |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                              |

Benchmark hidden because not significant (36): fannkuch, xml_etree_iterparse, sympy_sum, telco, coroutines, pyflate, raytrace, dask, tornado_http, sqlglot_transpile, nbody, go, pprint_safe_repr, asyncio_tcp_ssl, async_tree_memoization_tg, json, scimark_monte_carlo, async_tree_memoization, async_tree_io, sympy_str, sqlglot_parse, bench_thread_pool, asyncio_websockets, mypy2, async_tree_none, bench_mp_pool, pathlib, 2to3, unpickle_pure_python, async_tree_io_tg, xml_etree_generate, richards_super, coverage, async_tree_cpu_io_mixed_tg, scimark_fft, async_tree_cpu_io_mixed


# HPT report

- Reliability score: 85.70% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x