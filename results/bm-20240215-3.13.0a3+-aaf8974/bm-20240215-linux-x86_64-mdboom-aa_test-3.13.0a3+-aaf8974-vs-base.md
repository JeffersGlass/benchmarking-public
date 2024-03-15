# Results vs. base

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.00x faster
- HPT reliability: 99.12%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 261 ms                                                                 | 262 ms: 1.00x slower                                      |
| docutils       | 2.58 sec                                                               | 2.56 sec: 1.01x faster                                    |
| Geometric mean | (ref)                                                                  | 1.00x faster                                              |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_io      | 1.18 sec                                                               | 1.17 sec: 1.01x faster                                    |
| async_tree_io_tg   | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                    |
| async_tree_none_tg | 443 ms                                                                 | 442 ms: 1.00x faster                                      |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                              |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| nbody          | 90.1 ms                                                                | 88.7 ms: 1.02x faster                                     |
| Geometric mean | (ref)                                                                  | 1.01x faster                                              |

Benchmark hidden because not significant (2): float, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| regex_v8       | 26.1 ms                                                                | 23.8 ms: 1.10x faster                                     |
| regex_effbot   | 3.84 ms                                                                | 3.61 ms: 1.06x faster                                     |
| regex_dna      | 233 ms                                                                 | 223 ms: 1.05x faster                                      |
| Geometric mean | (ref)                                                                  | 1.05x faster                                              |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| unpickle_list        | 5.22 us                                                                | 4.98 us: 1.05x faster                                     |
| pickle_dict          | 35.7 us                                                                | 34.0 us: 1.05x faster                                     |
| pickle_list          | 5.00 us                                                                | 4.92 us: 1.02x faster                                     |
| json_dumps           | 10.5 ms                                                                | 10.4 ms: 1.02x faster                                     |
| unpickle_pure_python | 212 us                                                                 | 210 us: 1.01x faster                                      |
| xml_etree_generate   | 84.0 ms                                                                | 84.5 ms: 1.01x slower                                     |
| xml_etree_process    | 57.5 ms                                                                | 57.8 ms: 1.01x slower                                     |
| xml_etree_parse      | 155 ms                                                                 | 156 ms: 1.01x slower                                      |
| pickle               | 11.5 us                                                                | 11.6 us: 1.01x slower                                     |
| json_loads           | 27.7 us                                                                | 28.3 us: 1.02x slower                                     |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                              |

Benchmark hidden because not significant (4): tomli_loads, pickle_pure_python, unpickle, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                     |
| python_startup_no_site | 8.75 ms                                                                | 8.78 ms: 1.00x slower                                     |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 11.0 ms                                                                | 11.1 ms: 1.00x slower                                     |

All benchmarks:
===============

| Benchmark               | bm-20240215-linux-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| regex_v8                | 26.1 ms                                                                | 23.8 ms: 1.10x faster                                     |
| regex_effbot            | 3.84 ms                                                                | 3.61 ms: 1.06x faster                                     |
| unpickle_list           | 5.22 us                                                                | 4.98 us: 1.05x faster                                     |
| pickle_dict             | 35.7 us                                                                | 34.0 us: 1.05x faster                                     |
| regex_dna               | 233 ms                                                                 | 223 ms: 1.05x faster                                      |
| pycparser               | 1.20 sec                                                               | 1.15 sec: 1.04x faster                                    |
| coroutines              | 23.4 ms                                                                | 22.5 ms: 1.04x faster                                     |
| scimark_sparse_mat_mult | 4.75 ms                                                                | 4.56 ms: 1.04x faster                                     |
| logging_silent          | 97.7 ns                                                                | 94.7 ns: 1.03x faster                                     |
| scimark_monte_carlo     | 68.0 ms                                                                | 65.9 ms: 1.03x faster                                     |
| deepcopy_memo           | 37.5 us                                                                | 36.4 us: 1.03x faster                                     |
| gc_traversal            | 3.87 ms                                                                | 3.78 ms: 1.02x faster                                     |
| nqueens                 | 79.7 ms                                                                | 77.9 ms: 1.02x faster                                     |
| richards                | 47.5 ms                                                                | 46.7 ms: 1.02x faster                                     |
| pickle_list             | 5.00 us                                                                | 4.92 us: 1.02x faster                                     |
| nbody                   | 90.1 ms                                                                | 88.7 ms: 1.02x faster                                     |
| json_dumps              | 10.5 ms                                                                | 10.4 ms: 1.02x faster                                     |
| sqlite_synth            | 2.81 us                                                                | 2.77 us: 1.01x faster                                     |
| sympy_str               | 267 ms                                                                 | 264 ms: 1.01x faster                                      |
| deepcopy                | 342 us                                                                 | 338 us: 1.01x faster                                      |
| meteor_contest          | 108 ms                                                                 | 107 ms: 1.01x faster                                      |
| scimark_fft             | 356 ms                                                                 | 352 ms: 1.01x faster                                      |
| comprehensions          | 16.1 us                                                                | 16.0 us: 1.01x faster                                     |
| unpickle_pure_python    | 212 us                                                                 | 210 us: 1.01x faster                                      |
| deepcopy_reduce         | 3.02 us                                                                | 2.99 us: 1.01x faster                                     |
| coverage                | 96.0 ms                                                                | 95.2 ms: 1.01x faster                                     |
| docutils                | 2.58 sec                                                               | 2.56 sec: 1.01x faster                                    |
| sympy_integrate         | 19.5 ms                                                                | 19.4 ms: 1.01x faster                                     |
| sympy_expand            | 449 ms                                                                 | 447 ms: 1.01x faster                                      |
| pprint_safe_repr        | 725 ms                                                                 | 721 ms: 1.01x faster                                      |
| async_tree_io           | 1.18 sec                                                               | 1.17 sec: 1.01x faster                                    |
| async_tree_io_tg        | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                    |
| sqlglot_normalize       | 105 ms                                                                 | 104 ms: 1.00x faster                                      |
| generators              | 29.1 ms                                                                | 28.9 ms: 1.00x faster                                     |
| fannkuch                | 391 ms                                                                 | 390 ms: 1.00x faster                                      |
| hexiom                  | 5.94 ms                                                                | 5.91 ms: 1.00x faster                                     |
| chaos                   | 59.0 ms                                                                | 58.8 ms: 1.00x faster                                     |
| async_tree_none_tg      | 443 ms                                                                 | 442 ms: 1.00x faster                                      |
| dulwich_log             | 65.2 ms                                                                | 65.1 ms: 1.00x faster                                     |
| sqlglot_optimize        | 52.8 ms                                                                | 52.9 ms: 1.00x slower                                     |
| asyncio_tcp_ssl         | 1.78 sec                                                               | 1.79 sec: 1.00x slower                                    |
| bench_thread_pool       | 815 us                                                                 | 816 us: 1.00x slower                                      |
| 2to3                    | 261 ms                                                                 | 262 ms: 1.00x slower                                      |
| python_startup          | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                     |
| python_startup_no_site  | 8.75 ms                                                                | 8.78 ms: 1.00x slower                                     |
| mako                    | 11.0 ms                                                                | 11.1 ms: 1.00x slower                                     |
| xml_etree_generate      | 84.0 ms                                                                | 84.5 ms: 1.01x slower                                     |
| xml_etree_process       | 57.5 ms                                                                | 57.8 ms: 1.01x slower                                     |
| xml_etree_parse         | 155 ms                                                                 | 156 ms: 1.01x slower                                      |
| sqlglot_transpile       | 1.54 ms                                                                | 1.55 ms: 1.01x slower                                     |
| create_gc_cycles        | 1.49 ms                                                                | 1.50 ms: 1.01x slower                                     |
| crypto_pyaes            | 70.0 ms                                                                | 70.6 ms: 1.01x slower                                     |
| logging_simple          | 5.56 us                                                                | 5.61 us: 1.01x slower                                     |
| pickle                  | 11.5 us                                                                | 11.6 us: 1.01x slower                                     |
| raytrace                | 257 ms                                                                 | 260 ms: 1.01x slower                                      |
| sqlglot_parse           | 1.23 ms                                                                | 1.24 ms: 1.01x slower                                     |
| deltablue               | 3.15 ms                                                                | 3.19 ms: 1.01x slower                                     |
| pathlib                 | 17.9 ms                                                                | 18.1 ms: 1.01x slower                                     |
| async_generators        | 442 ms                                                                 | 448 ms: 1.01x slower                                      |
| pyflate                 | 458 ms                                                                 | 466 ms: 1.02x slower                                      |
| mdp                     | 2.67 sec                                                               | 2.72 sec: 1.02x slower                                    |
| json_loads              | 27.7 us                                                                | 28.3 us: 1.02x slower                                     |
| go                      | 136 ms                                                                 | 139 ms: 1.02x slower                                      |
| spectral_norm           | 107 ms                                                                 | 110 ms: 1.02x slower                                      |
| scimark_sor             | 118 ms                                                                 | 129 ms: 1.09x slower                                      |
| unpack_sequence         | 40.3 ns                                                                | 50.1 ns: 1.24x slower                                     |
| Geometric mean          | (ref)                                                                  | 1.00x faster                                              |

Benchmark hidden because not significant (27): async_tree_cpu_io_mixed_tg, dask, async_tree_cpu_io_mixed, telco, async_tree_none, tomli_loads, json, tornado_http, scimark_lu, async_tree_memoization_tg, async_tree_memoization, pickle_pure_python, pprint_pformat, mypy2, richards_super, sympy_sum, float, unpickle, regex_compile, pidigits, bench_mp_pool, logging_format, asyncio_tcp, xml_etree_iterparse, asyncio_websockets, chameleon, typing_runtime_protocols


# HPT report

- Reliability score: 99.12% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x