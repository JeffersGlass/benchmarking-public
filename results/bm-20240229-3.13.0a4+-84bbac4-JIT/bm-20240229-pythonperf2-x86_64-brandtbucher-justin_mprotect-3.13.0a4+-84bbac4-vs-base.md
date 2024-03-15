# Results vs. base

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster \*
- HPT reliability: 75.06%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 306 ms                                                                       | 305 ms: 1.00x faster                                                          |
| chameleon      | 7.45 ms                                                                      | 7.52 ms: 1.01x slower                                                         |
| docutils       | 2.91 sec                                                                     | 2.93 sec: 1.01x slower                                                        |
| mdp            | 2.59 sec                                                                     | 2.57 sec: 1.01x faster                                                        |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                                  |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_memoization | 555 ms                                                                       | 549 ms: 1.01x faster                                                          |
| async_tree_none_tg     | 438 ms                                                                       | 434 ms: 1.01x faster                                                          |
| async_tree_io_tg       | 1.09 sec                                                                     | 1.08 sec: 1.00x faster                                                        |
| Geometric mean         | (ref)                                                                        | 1.01x faster                                                                  |

Benchmark hidden because not significant (5): async_tree_memoization_tg, async_tree_none, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody          | 105 ms                                                                       | 98.0 ms: 1.08x faster                                                         |
| float          | 77.6 ms                                                                      | 78.5 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                                        | 1.02x faster                                                                  |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_v8       | 25.4 ms                                                                      | 26.0 ms: 1.03x slower                                                         |
| regex_effbot   | 3.46 ms                                                                      | 3.63 ms: 1.05x slower                                                         |
| regex_dna      | 235 ms                                                                       | 248 ms: 1.05x slower                                                          |
| Geometric mean | (ref)                                                                        | 1.03x slower                                                                  |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| unpickle_list        | 4.72 us                                                                      | 4.58 us: 1.03x faster                                                         |
| pickle               | 10.4 us                                                                      | 10.1 us: 1.02x faster                                                         |
| unpickle             | 15.2 us                                                                      | 14.9 us: 1.02x faster                                                         |
| pickle_dict          | 30.5 us                                                                      | 30.6 us: 1.00x slower                                                         |
| json_loads           | 25.0 us                                                                      | 25.2 us: 1.01x slower                                                         |
| xml_etree_parse      | 144 ms                                                                       | 145 ms: 1.01x slower                                                          |
| xml_etree_process    | 57.6 ms                                                                      | 58.2 ms: 1.01x slower                                                         |
| unpickle_pure_python | 230 us                                                                       | 234 us: 1.01x slower                                                          |
| tomli_loads          | 2.13 sec                                                                     | 2.17 sec: 1.02x slower                                                        |
| pickle_pure_python   | 311 us                                                                       | 319 us: 1.03x slower                                                          |
| pickle_list          | 4.21 us                                                                      | 4.43 us: 1.05x slower                                                         |
| Geometric mean       | (ref)                                                                        | 1.00x slower                                                                  |

Benchmark hidden because not significant (4): xml_etree_iterparse, mypy2, xml_etree_generate, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup_no_site | 14.0 ms                                                                      | 13.3 ms: 1.05x faster                                                         |
| python_startup         | 15.5 ms                                                                      | 14.8 ms: 1.05x faster                                                         |
| Geometric mean         | (ref)                                                                        | 1.05x faster                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 9.93 ms                                                                      | 9.96 ms: 1.00x slower                                                         |

All benchmarks:
===============

| Benchmark               | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| bench_mp_pool           | 6.88 ms                                                                      | 4.77 ms: 1.44x faster                                                         |
| nbody                   | 105 ms                                                                       | 98.0 ms: 1.08x faster                                                         |
| python_startup_no_site  | 14.0 ms                                                                      | 13.3 ms: 1.05x faster                                                         |
| python_startup          | 15.5 ms                                                                      | 14.8 ms: 1.05x faster                                                         |
| pycparser               | 1.35 sec                                                                     | 1.31 sec: 1.04x faster                                                        |
| logging_simple          | 6.69 us                                                                      | 6.47 us: 1.03x faster                                                         |
| unpickle_list           | 4.72 us                                                                      | 4.58 us: 1.03x faster                                                         |
| pickle                  | 10.4 us                                                                      | 10.1 us: 1.02x faster                                                         |
| pprint_pformat          | 1.74 sec                                                                     | 1.70 sec: 1.02x faster                                                        |
| logging_format          | 7.34 us                                                                      | 7.18 us: 1.02x faster                                                         |
| pprint_safe_repr        | 844 ms                                                                       | 827 ms: 1.02x faster                                                          |
| unpickle                | 15.2 us                                                                      | 14.9 us: 1.02x faster                                                         |
| coverage                | 81.9 ms                                                                      | 80.4 ms: 1.02x faster                                                         |
| fannkuch                | 394 ms                                                                       | 387 ms: 1.02x faster                                                          |
| go                      | 174 ms                                                                       | 171 ms: 1.02x faster                                                          |
| async_tree_memoization  | 555 ms                                                                       | 549 ms: 1.01x faster                                                          |
| async_generators        | 384 ms                                                                       | 381 ms: 1.01x faster                                                          |
| json                    | 5.37 ms                                                                      | 5.31 ms: 1.01x faster                                                         |
| mdp                     | 2.59 sec                                                                     | 2.57 sec: 1.01x faster                                                        |
| pathlib                 | 19.4 ms                                                                      | 19.3 ms: 1.01x faster                                                         |
| async_tree_none_tg      | 438 ms                                                                       | 434 ms: 1.01x faster                                                          |
| unpack_sequence         | 61.9 ns                                                                      | 61.4 ns: 1.01x faster                                                         |
| deepcopy                | 376 us                                                                       | 374 us: 1.01x faster                                                          |
| generators              | 34.0 ms                                                                      | 33.8 ms: 1.01x faster                                                         |
| dulwich_log             | 69.1 ms                                                                      | 68.8 ms: 1.00x faster                                                         |
| async_tree_io_tg        | 1.09 sec                                                                     | 1.08 sec: 1.00x faster                                                        |
| 2to3                    | 306 ms                                                                       | 305 ms: 1.00x faster                                                          |
| spectral_norm           | 92.4 ms                                                                      | 92.7 ms: 1.00x slower                                                         |
| asyncio_tcp_ssl         | 1.57 sec                                                                     | 1.58 sec: 1.00x slower                                                        |
| mako                    | 9.93 ms                                                                      | 9.96 ms: 1.00x slower                                                         |
| pickle_dict             | 30.5 us                                                                      | 30.6 us: 1.00x slower                                                         |
| sympy_sum               | 159 ms                                                                       | 160 ms: 1.00x slower                                                          |
| nqueens                 | 101 ms                                                                       | 102 ms: 1.00x slower                                                          |
| sympy_integrate         | 24.5 ms                                                                      | 24.6 ms: 1.01x slower                                                         |
| logging_silent          | 97.1 ns                                                                      | 97.7 ns: 1.01x slower                                                         |
| richards                | 50.1 ms                                                                      | 50.4 ms: 1.01x slower                                                         |
| asyncio_tcp             | 368 ms                                                                       | 371 ms: 1.01x slower                                                          |
| sqlglot_normalize       | 119 ms                                                                       | 120 ms: 1.01x slower                                                          |
| docutils                | 2.91 sec                                                                     | 2.93 sec: 1.01x slower                                                        |
| json_loads              | 25.0 us                                                                      | 25.2 us: 1.01x slower                                                         |
| xml_etree_parse         | 144 ms                                                                       | 145 ms: 1.01x slower                                                          |
| sympy_str               | 302 ms                                                                       | 305 ms: 1.01x slower                                                          |
| hexiom                  | 7.37 ms                                                                      | 7.43 ms: 1.01x slower                                                         |
| sqlglot_optimize        | 62.8 ms                                                                      | 63.4 ms: 1.01x slower                                                         |
| chameleon               | 7.45 ms                                                                      | 7.52 ms: 1.01x slower                                                         |
| deepcopy_reduce         | 3.34 us                                                                      | 3.37 us: 1.01x slower                                                         |
| comprehensions          | 18.8 us                                                                      | 19.0 us: 1.01x slower                                                         |
| xml_etree_process       | 57.6 ms                                                                      | 58.2 ms: 1.01x slower                                                         |
| richards_super          | 56.7 ms                                                                      | 57.3 ms: 1.01x slower                                                         |
| float                   | 77.6 ms                                                                      | 78.5 ms: 1.01x slower                                                         |
| scimark_sor             | 151 ms                                                                       | 153 ms: 1.01x slower                                                          |
| unpickle_pure_python    | 230 us                                                                       | 234 us: 1.01x slower                                                          |
| tomli_loads             | 2.13 sec                                                                     | 2.17 sec: 1.02x slower                                                        |
| gc_traversal            | 3.67 ms                                                                      | 3.75 ms: 1.02x slower                                                         |
| pickle_pure_python      | 311 us                                                                       | 319 us: 1.03x slower                                                          |
| scimark_fft             | 316 ms                                                                       | 324 ms: 1.03x slower                                                          |
| regex_v8                | 25.4 ms                                                                      | 26.0 ms: 1.03x slower                                                         |
| scimark_monte_carlo     | 77.5 ms                                                                      | 80.0 ms: 1.03x slower                                                         |
| regex_effbot            | 3.46 ms                                                                      | 3.63 ms: 1.05x slower                                                         |
| pickle_list             | 4.21 us                                                                      | 4.43 us: 1.05x slower                                                         |
| scimark_sparse_mat_mult | 4.20 ms                                                                      | 4.42 ms: 1.05x slower                                                         |
| scimark_lu              | 115 ms                                                                       | 121 ms: 1.05x slower                                                          |
| regex_dna               | 235 ms                                                                       | 248 ms: 1.05x slower                                                          |
| Geometric mean          | (ref)                                                                        | 1.00x faster                                                                  |

Benchmark hidden because not significant (30): telco, async_tree_memoization_tg, chaos, async_tree_none, async_tree_cpu_io_mixed, sqlglot_transpile, async_tree_cpu_io_mixed_tg, regex_compile, asyncio_websockets, bench_thread_pool, raytrace, sqlite_synth, xml_etree_iterparse, mypy2, pyflate, deltablue, meteor_contest, sqlglot_parse, pidigits, xml_etree_generate, json_dumps, typing_runtime_protocols, async_tree_io, coroutines, crypto_pyaes, sympy_expand, dask, tornado_http, create_gc_cycles, deepcopy_memo
Ignored benchmarks (8) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: aiohttp, django_template, genshi_text, genshi_xml, gunicorn, html5lib, pylint, thrift


# HPT report

- Reliability score: 75.06% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x