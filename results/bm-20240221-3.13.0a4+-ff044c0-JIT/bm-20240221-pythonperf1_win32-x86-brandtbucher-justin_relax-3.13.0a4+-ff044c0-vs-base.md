# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: windows-x86
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 268 ms                                                                          | 262 ms: 1.02x faster                                                          |
| chameleon      | 5.74 ms                                                                         | 5.99 ms: 1.04x slower                                                         |
| docutils       | 1.92 sec                                                                        | 1.85 sec: 1.03x faster                                                        |
| tornado_http   | 100 ms                                                                          | 97.8 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                                           | 1.01x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 543 ms                                                                          | 511 ms: 1.06x faster                                                          |
| async_tree_cpu_io_mixed_tg | 527 ms                                                                          | 497 ms: 1.06x faster                                                          |
| async_tree_none            | 267 ms                                                                          | 259 ms: 1.03x faster                                                          |
| async_tree_io              | 639 ms                                                                          | 621 ms: 1.03x faster                                                          |
| async_tree_io_tg           | 617 ms                                                                          | 604 ms: 1.02x faster                                                          |
| async_tree_memoization_tg  | 314 ms                                                                          | 307 ms: 1.02x faster                                                          |
| async_tree_memoization     | 330 ms                                                                          | 323 ms: 1.02x faster                                                          |
| async_tree_none_tg         | 248 ms                                                                          | 244 ms: 1.02x faster                                                          |
| Geometric mean             | (ref)                                                                           | 1.03x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 203 ms                                                                          | 199 ms: 1.02x faster                                                          |
| nbody          | 93.3 ms                                                                         | 94.5 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                                  |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 132 ms                                                                          | 117 ms: 1.13x faster                                                          |
| regex_dna      | 123 ms                                                                          | 118 ms: 1.05x faster                                                          |
| regex_v8       | 16.2 ms                                                                         | 16.0 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                                           | 1.05x faster                                                                  |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 7.26 ms                                                                         | 6.90 ms: 1.05x faster                                                         |
| xml_etree_process    | 44.5 ms                                                                         | 42.7 ms: 1.04x faster                                                         |
| json_loads           | 20.8 us                                                                         | 20.1 us: 1.04x faster                                                         |
| xml_etree_generate   | 62.4 ms                                                                         | 60.5 ms: 1.03x faster                                                         |
| pickle_pure_python   | 231 us                                                                          | 228 us: 1.01x faster                                                          |
| tomli_loads          | 1.73 sec                                                                        | 1.71 sec: 1.01x faster                                                        |
| pickle_dict          | 20.0 us                                                                         | 19.8 us: 1.01x faster                                                         |
| unpickle_pure_python | 183 us                                                                          | 181 us: 1.01x faster                                                          |
| xml_etree_parse      | 109 ms                                                                          | 108 ms: 1.00x faster                                                          |
| unpickle             | 9.92 us                                                                         | 10.0 us: 1.01x slower                                                         |
| unpickle_list        | 2.80 us                                                                         | 2.85 us: 1.02x slower                                                         |
| Geometric mean       | (ref)                                                                           | 1.01x faster                                                                  |

Benchmark hidden because not significant (3): pickle, xml_etree_iterparse, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup_no_site | 23.6 ms                                                                         | 23.8 ms: 1.01x slower                                                         |
| python_startup         | 25.9 ms                                                                         | 26.3 ms: 1.01x slower                                                         |
| Geometric mean         | (ref)                                                                           | 1.01x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 7.40 ms                                                                         | 7.25 ms: 1.02x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20240221-pythonperf1_win32-x86-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| unpack_sequence            | 87.0 ns                                                                         | 64.6 ns: 1.35x faster                                                         |
| scimark_monte_carlo        | 79.1 ms                                                                         | 65.5 ms: 1.21x faster                                                         |
| hexiom                     | 7.73 ms                                                                         | 6.47 ms: 1.19x faster                                                         |
| scimark_sor                | 126 ms                                                                          | 107 ms: 1.18x faster                                                          |
| regex_compile              | 132 ms                                                                          | 117 ms: 1.13x faster                                                          |
| go                         | 138 ms                                                                          | 123 ms: 1.12x faster                                                          |
| mdp                        | 1.90 sec                                                                        | 1.74 sec: 1.09x faster                                                        |
| scimark_lu                 | 92.1 ms                                                                         | 85.7 ms: 1.07x faster                                                         |
| raytrace                   | 282 ms                                                                          | 263 ms: 1.07x faster                                                          |
| richards_super             | 46.7 ms                                                                         | 43.7 ms: 1.07x faster                                                         |
| pyflate                    | 411 ms                                                                          | 384 ms: 1.07x faster                                                          |
| meteor_contest             | 87.6 ms                                                                         | 82.1 ms: 1.07x faster                                                         |
| richards                   | 41.6 ms                                                                         | 39.1 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 543 ms                                                                          | 511 ms: 1.06x faster                                                          |
| async_tree_cpu_io_mixed_tg | 527 ms                                                                          | 497 ms: 1.06x faster                                                          |
| chaos                      | 60.5 ms                                                                         | 57.3 ms: 1.06x faster                                                         |
| json_dumps                 | 7.26 ms                                                                         | 6.90 ms: 1.05x faster                                                         |
| sympy_expand               | 403 ms                                                                          | 384 ms: 1.05x faster                                                          |
| comprehensions             | 15.5 us                                                                         | 14.7 us: 1.05x faster                                                         |
| regex_dna                  | 123 ms                                                                          | 118 ms: 1.05x faster                                                          |
| sympy_sum                  | 115 ms                                                                          | 109 ms: 1.05x faster                                                          |
| sympy_str                  | 228 ms                                                                          | 218 ms: 1.05x faster                                                          |
| pycparser                  | 907 ms                                                                          | 869 ms: 1.04x faster                                                          |
| xml_etree_process          | 44.5 ms                                                                         | 42.7 ms: 1.04x faster                                                         |
| scimark_fft                | 247 ms                                                                          | 237 ms: 1.04x faster                                                          |
| pprint_pformat             | 1.52 sec                                                                        | 1.46 sec: 1.04x faster                                                        |
| json_loads                 | 20.8 us                                                                         | 20.1 us: 1.04x faster                                                         |
| docutils                   | 1.92 sec                                                                        | 1.85 sec: 1.03x faster                                                        |
| xml_etree_generate         | 62.4 ms                                                                         | 60.5 ms: 1.03x faster                                                         |
| async_tree_none            | 267 ms                                                                          | 259 ms: 1.03x faster                                                          |
| sqlglot_optimize           | 47.3 ms                                                                         | 46.0 ms: 1.03x faster                                                         |
| async_tree_io              | 639 ms                                                                          | 621 ms: 1.03x faster                                                          |
| pprint_safe_repr           | 740 ms                                                                          | 719 ms: 1.03x faster                                                          |
| async_generators           | 302 ms                                                                          | 294 ms: 1.03x faster                                                          |
| deepcopy_reduce            | 2.66 us                                                                         | 2.59 us: 1.03x faster                                                         |
| sympy_integrate            | 16.4 ms                                                                         | 16.0 ms: 1.03x faster                                                         |
| fannkuch                   | 339 ms                                                                          | 330 ms: 1.02x faster                                                          |
| gc_traversal               | 1.41 ms                                                                         | 1.38 ms: 1.02x faster                                                         |
| spectral_norm              | 72.4 ms                                                                         | 70.7 ms: 1.02x faster                                                         |
| tornado_http               | 100 ms                                                                          | 97.8 ms: 1.02x faster                                                         |
| 2to3                       | 268 ms                                                                          | 262 ms: 1.02x faster                                                          |
| async_tree_io_tg           | 617 ms                                                                          | 604 ms: 1.02x faster                                                          |
| nqueens                    | 93.3 ms                                                                         | 91.3 ms: 1.02x faster                                                         |
| pidigits                   | 203 ms                                                                          | 199 ms: 1.02x faster                                                          |
| async_tree_memoization_tg  | 314 ms                                                                          | 307 ms: 1.02x faster                                                          |
| sqlglot_parse              | 1.03 ms                                                                         | 1.01 ms: 1.02x faster                                                         |
| async_tree_memoization     | 330 ms                                                                          | 323 ms: 1.02x faster                                                          |
| mako                       | 7.40 ms                                                                         | 7.25 ms: 1.02x faster                                                         |
| sqlglot_transpile          | 1.30 ms                                                                         | 1.28 ms: 1.02x faster                                                         |
| async_tree_none_tg         | 248 ms                                                                          | 244 ms: 1.02x faster                                                          |
| pickle_pure_python         | 231 us                                                                          | 228 us: 1.01x faster                                                          |
| tomli_loads                | 1.73 sec                                                                        | 1.71 sec: 1.01x faster                                                        |
| regex_v8                   | 16.2 ms                                                                         | 16.0 ms: 1.01x faster                                                         |
| scimark_sparse_mat_mult    | 3.14 ms                                                                         | 3.11 ms: 1.01x faster                                                         |
| pickle_dict                | 20.0 us                                                                         | 19.8 us: 1.01x faster                                                         |
| unpickle_pure_python       | 183 us                                                                          | 181 us: 1.01x faster                                                          |
| crypto_pyaes               | 61.2 ms                                                                         | 60.8 ms: 1.01x faster                                                         |
| sqlglot_normalize          | 229 ms                                                                          | 227 ms: 1.01x faster                                                          |
| coverage                   | 480 ms                                                                          | 478 ms: 1.00x faster                                                          |
| xml_etree_parse            | 109 ms                                                                          | 108 ms: 1.00x faster                                                          |
| deltablue                  | 2.73 ms                                                                         | 2.74 ms: 1.00x slower                                                         |
| sqlite_synth               | 1.96 us                                                                         | 1.97 us: 1.00x slower                                                         |
| python_startup_no_site     | 23.6 ms                                                                         | 23.8 ms: 1.01x slower                                                         |
| asyncio_tcp_ssl            | 16.8 sec                                                                        | 16.9 sec: 1.01x slower                                                        |
| deepcopy                   | 296 us                                                                          | 298 us: 1.01x slower                                                          |
| logging_silent             | 68.4 ns                                                                         | 69.0 ns: 1.01x slower                                                         |
| json                       | 4.25 ms                                                                         | 4.28 ms: 1.01x slower                                                         |
| unpickle                   | 9.92 us                                                                         | 10.0 us: 1.01x slower                                                         |
| nbody                      | 93.3 ms                                                                         | 94.5 ms: 1.01x slower                                                         |
| python_startup             | 25.9 ms                                                                         | 26.3 ms: 1.01x slower                                                         |
| telco                      | 6.34 ms                                                                         | 6.46 ms: 1.02x slower                                                         |
| unpickle_list              | 2.80 us                                                                         | 2.85 us: 1.02x slower                                                         |
| logging_simple             | 8.35 us                                                                         | 8.50 us: 1.02x slower                                                         |
| typing_runtime_protocols   | 97.3 us                                                                         | 99.3 us: 1.02x slower                                                         |
| logging_format             | 8.90 us                                                                         | 9.08 us: 1.02x slower                                                         |
| generators                 | 23.9 ms                                                                         | 24.6 ms: 1.03x slower                                                         |
| coroutines                 | 14.8 ms                                                                         | 15.3 ms: 1.03x slower                                                         |
| chameleon                  | 5.74 ms                                                                         | 5.99 ms: 1.04x slower                                                         |
| Geometric mean             | (ref)                                                                           | 1.03x faster                                                                  |

Benchmark hidden because not significant (11): bench_thread_pool, asyncio_tcp, pickle, bench_mp_pool, pathlib, xml_etree_iterparse, pickle_list, float, create_gc_cycles, deepcopy_memo, regex_effbot


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown