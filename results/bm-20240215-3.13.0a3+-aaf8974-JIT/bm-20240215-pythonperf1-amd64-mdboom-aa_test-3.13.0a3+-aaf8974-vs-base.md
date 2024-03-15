# Results vs. base

- fork: mdboom
- ref: aa_test
- machine: windows-amd64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.00x slower
- HPT reliability: 80.20%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------------------:|:--------------------------------------------------------------:|
| docutils       | 1.56 sec                                                                    | 1.56 sec: 1.00x slower                                         |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                   |

Benchmark hidden because not significant (3): 2to3, chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------|:---------------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io      | 709 ms                                                                      | 720 ms: 1.02x slower                                           |
| async_tree_none_tg | 266 ms                                                                      | 271 ms: 1.02x slower                                           |
| Geometric mean     | (ref)                                                                       | 1.01x slower                                                   |

Benchmark hidden because not significant (6): async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

Benchmark hidden because not significant (3): nbody, float, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 119 ms                                                                      | 115 ms: 1.03x faster                                           |
| regex_effbot   | 1.57 ms                                                                     | 1.56 ms: 1.01x faster                                          |
| regex_v8       | 14.5 ms                                                                     | 14.4 ms: 1.01x faster                                          |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                   |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:---------------------------------------------------------------------------:|:--------------------------------------------------------------:|
| unpickle_list        | 2.92 us                                                                     | 2.76 us: 1.06x faster                                          |
| pickle_dict          | 17.6 us                                                                     | 17.4 us: 1.01x faster                                          |
| pickle_pure_python   | 176 us                                                                      | 175 us: 1.01x faster                                           |
| unpickle_pure_python | 126 us                                                                      | 127 us: 1.01x slower                                           |
| xml_etree_iterparse  | 63.3 ms                                                                     | 63.8 ms: 1.01x slower                                          |
| json_loads           | 13.6 us                                                                     | 13.7 us: 1.01x slower                                          |
| tomli_loads          | 1.29 sec                                                                    | 1.30 sec: 1.01x slower                                         |
| xml_etree_parse      | 91.5 ms                                                                     | 93.1 ms: 1.02x slower                                          |
| unpickle             | 8.46 us                                                                     | 8.63 us: 1.02x slower                                          |
| pickle_list          | 2.73 us                                                                     | 2.78 us: 1.02x slower                                          |
| Geometric mean       | (ref)                                                                       | 1.00x slower                                                   |

Benchmark hidden because not significant (4): json_dumps, xml_etree_generate, pickle, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:---------------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 20.5 ms                                                                     | 20.1 ms: 1.02x faster                                          |
| python_startup_no_site | 18.3 ms                                                                     | 18.1 ms: 1.01x faster                                          |
| Geometric mean         | (ref)                                                                       | 1.02x faster                                                   |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:---------------------------------------------------------------------------:|:--------------------------------------------------------------:|
| unpickle_list           | 2.92 us                                                                     | 2.76 us: 1.06x faster                                          |
| unpack_sequence         | 41.6 ns                                                                     | 39.3 ns: 1.06x faster                                          |
| deepcopy_memo           | 22.8 us                                                                     | 21.6 us: 1.06x faster                                          |
| fannkuch                | 241 ms                                                                      | 234 ms: 1.03x faster                                           |
| regex_dna               | 119 ms                                                                      | 115 ms: 1.03x faster                                           |
| mdp                     | 1.60 sec                                                                    | 1.55 sec: 1.03x faster                                         |
| coroutines              | 13.1 ms                                                                     | 12.8 ms: 1.03x faster                                          |
| python_startup          | 20.5 ms                                                                     | 20.1 ms: 1.02x faster                                          |
| deepcopy_reduce         | 1.94 us                                                                     | 1.91 us: 1.01x faster                                          |
| pprint_safe_repr        | 486 ms                                                                      | 480 ms: 1.01x faster                                           |
| meteor_contest          | 77.3 ms                                                                     | 76.3 ms: 1.01x faster                                          |
| python_startup_no_site  | 18.3 ms                                                                     | 18.1 ms: 1.01x faster                                          |
| pickle_dict             | 17.6 us                                                                     | 17.4 us: 1.01x faster                                          |
| logging_simple          | 5.95 us                                                                     | 5.89 us: 1.01x faster                                          |
| regex_effbot            | 1.57 ms                                                                     | 1.56 ms: 1.01x faster                                          |
| logging_format          | 6.45 us                                                                     | 6.39 us: 1.01x faster                                          |
| sympy_integrate         | 13.0 ms                                                                     | 12.9 ms: 1.01x faster                                          |
| coverage                | 46.3 ms                                                                     | 45.9 ms: 1.01x faster                                          |
| pathlib                 | 75.4 ms                                                                     | 74.8 ms: 1.01x faster                                          |
| deepcopy                | 220 us                                                                      | 219 us: 1.01x faster                                           |
| regex_v8                | 14.5 ms                                                                     | 14.4 ms: 1.01x faster                                          |
| logging_silent          | 54.6 ns                                                                     | 54.2 ns: 1.01x faster                                          |
| deltablue               | 1.99 ms                                                                     | 1.98 ms: 1.01x faster                                          |
| pickle_pure_python      | 176 us                                                                      | 175 us: 1.01x faster                                           |
| pprint_pformat          | 988 ms                                                                      | 983 ms: 1.01x faster                                           |
| dulwich_log             | 40.5 ms                                                                     | 40.3 ms: 1.00x faster                                          |
| docutils                | 1.56 sec                                                                    | 1.56 sec: 1.00x slower                                         |
| chaos                   | 41.9 ms                                                                     | 42.2 ms: 1.01x slower                                          |
| unpickle_pure_python    | 126 us                                                                      | 127 us: 1.01x slower                                           |
| xml_etree_iterparse     | 63.3 ms                                                                     | 63.8 ms: 1.01x slower                                          |
| json_loads              | 13.6 us                                                                     | 13.7 us: 1.01x slower                                          |
| tomli_loads             | 1.29 sec                                                                    | 1.30 sec: 1.01x slower                                         |
| create_gc_cycles        | 732 us                                                                      | 741 us: 1.01x slower                                           |
| scimark_lu              | 56.4 ms                                                                     | 57.2 ms: 1.01x slower                                          |
| scimark_sor             | 77.8 ms                                                                     | 78.9 ms: 1.01x slower                                          |
| nqueens                 | 59.3 ms                                                                     | 60.2 ms: 1.02x slower                                          |
| async_tree_io           | 709 ms                                                                      | 720 ms: 1.02x slower                                           |
| xml_etree_parse         | 91.5 ms                                                                     | 93.1 ms: 1.02x slower                                          |
| sqlglot_optimize        | 33.3 ms                                                                     | 33.9 ms: 1.02x slower                                          |
| async_generators        | 236 ms                                                                      | 241 ms: 1.02x slower                                           |
| async_tree_none_tg      | 266 ms                                                                      | 271 ms: 1.02x slower                                           |
| unpickle                | 8.46 us                                                                     | 8.63 us: 1.02x slower                                          |
| pickle_list             | 2.73 us                                                                     | 2.78 us: 1.02x slower                                          |
| sqlglot_normalize       | 170 ms                                                                      | 174 ms: 1.02x slower                                           |
| richards                | 25.8 ms                                                                     | 26.4 ms: 1.02x slower                                          |
| hexiom                  | 5.15 ms                                                                     | 5.29 ms: 1.03x slower                                          |
| scimark_sparse_mat_mult | 2.63 ms                                                                     | 2.71 ms: 1.03x slower                                          |
| sympy_sum               | 85.4 ms                                                                     | 87.9 ms: 1.03x slower                                          |
| generators              | 19.9 ms                                                                     | 20.6 ms: 1.04x slower                                          |
| sympy_str               | 158 ms                                                                      | 164 ms: 1.04x slower                                           |
| json                    | 2.89 ms                                                                     | 3.12 ms: 1.08x slower                                          |
| pycparser               | 691 ms                                                                      | 748 ms: 1.08x slower                                           |
| Geometric mean          | (ref)                                                                       | 1.00x slower                                                   |

Benchmark hidden because not significant (40): asyncio_tcp_ssl, nbody, comprehensions, raytrace, asyncio_tcp, async_tree_memoization, typing_runtime_protocols, chameleon, async_tree_cpu_io_mixed_tg, 2to3, float, telco, sympy_expand, go, json_dumps, sqlglot_parse, async_tree_cpu_io_mixed, bench_mp_pool, scimark_monte_carlo, tornado_http, pidigits, xml_etree_generate, gc_traversal, mypy2, pyflate, pickle, sqlglot_transpile, dask, sqlite_synth, xml_etree_process, richards_super, regex_compile, async_tree_none, crypto_pyaes, async_tree_memoization_tg, mako, scimark_fft, async_tree_io_tg, bench_thread_pool, spectral_norm


# HPT report

- Reliability score: 80.20% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown