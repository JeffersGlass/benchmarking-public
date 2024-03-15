# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: windows-x86
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.00x slower
- HPT reliability: 85.18%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                                          | 247 ms: 1.01x slower                                                             |
| chameleon      | 6.02 ms                                                                         | 5.91 ms: 1.02x faster                                                            |
| docutils       | 1.78 sec                                                                        | 1.77 sec: 1.01x faster                                                           |
| tornado_http   | 95.7 ms                                                                         | 96.4 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|---------------------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io             | 597 ms                                                                          | 601 ms: 1.01x slower                                                             |
| async_tree_none_tg        | 237 ms                                                                          | 239 ms: 1.01x slower                                                             |
| async_tree_io_tg          | 585 ms                                                                          | 590 ms: 1.01x slower                                                             |
| async_tree_memoization_tg | 298 ms                                                                          | 302 ms: 1.01x slower                                                             |
| Geometric mean            | (ref)                                                                           | 1.01x slower                                                                     |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 203 ms                                                                          | 201 ms: 1.01x faster                                                             |
| nbody          | 90.6 ms                                                                         | 93.5 ms: 1.03x slower                                                            |
| Geometric mean | (ref)                                                                           | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 105 ms                                                                          | 103 ms: 1.01x faster                                                             |
| regex_v8       | 16.0 ms                                                                         | 16.1 ms: 1.01x slower                                                            |
| regex_effbot   | 1.89 ms                                                                         | 1.91 ms: 1.01x slower                                                            |
| regex_dna      | 117 ms                                                                          | 123 ms: 1.05x slower                                                             |
| Geometric mean | (ref)                                                                           | 1.01x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 3.10 us                                                                         | 2.82 us: 1.10x faster                                                            |
| pickle_list          | 3.66 us                                                                         | 3.37 us: 1.09x faster                                                            |
| xml_etree_generate   | 60.4 ms                                                                         | 58.4 ms: 1.03x faster                                                            |
| pickle               | 8.13 us                                                                         | 8.00 us: 1.02x faster                                                            |
| xml_etree_process    | 41.4 ms                                                                         | 41.5 ms: 1.00x slower                                                            |
| json_dumps           | 6.71 ms                                                                         | 6.84 ms: 1.02x slower                                                            |
| pickle_pure_python   | 205 us                                                                          | 210 us: 1.03x slower                                                             |
| unpickle_pure_python | 150 us                                                                          | 155 us: 1.03x slower                                                             |
| xml_etree_iterparse  | 65.5 ms                                                                         | 67.8 ms: 1.04x slower                                                            |
| xml_etree_parse      | 104 ms                                                                          | 109 ms: 1.05x slower                                                             |
| Geometric mean       | (ref)                                                                           | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): unpickle, pickle_dict, tomli_loads, json_loads

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 7.64 ms                                                                         | 7.60 ms: 1.01x faster                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|---------------------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list             | 3.10 us                                                                         | 2.82 us: 1.10x faster                                                            |
| pickle_list               | 3.66 us                                                                         | 3.37 us: 1.09x faster                                                            |
| chaos                     | 61.8 ms                                                                         | 58.5 ms: 1.06x faster                                                            |
| spectral_norm             | 78.4 ms                                                                         | 75.5 ms: 1.04x faster                                                            |
| xml_etree_generate        | 60.4 ms                                                                         | 58.4 ms: 1.03x faster                                                            |
| pyflate                   | 383 ms                                                                          | 372 ms: 1.03x faster                                                             |
| pycparser                 | 843 ms                                                                          | 821 ms: 1.03x faster                                                             |
| raytrace                  | 228 ms                                                                          | 224 ms: 1.02x faster                                                             |
| chameleon                 | 6.02 ms                                                                         | 5.91 ms: 1.02x faster                                                            |
| sqlglot_normalize         | 219 ms                                                                          | 215 ms: 1.02x faster                                                             |
| sqlglot_optimize          | 42.8 ms                                                                         | 42.1 ms: 1.02x faster                                                            |
| bench_mp_pool             | 72.0 ms                                                                         | 70.7 ms: 1.02x faster                                                            |
| sympy_expand              | 372 ms                                                                          | 366 ms: 1.02x faster                                                             |
| pickle                    | 8.13 us                                                                         | 8.00 us: 1.02x faster                                                            |
| sqlglot_transpile         | 1.18 ms                                                                         | 1.16 ms: 1.01x faster                                                            |
| mdp                       | 1.89 sec                                                                        | 1.86 sec: 1.01x faster                                                           |
| sqlglot_parse             | 932 us                                                                          | 920 us: 1.01x faster                                                             |
| regex_compile             | 105 ms                                                                          | 103 ms: 1.01x faster                                                             |
| pidigits                  | 203 ms                                                                          | 201 ms: 1.01x faster                                                             |
| docutils                  | 1.78 sec                                                                        | 1.77 sec: 1.01x faster                                                           |
| dask                      | 298 ms                                                                          | 296 ms: 1.01x faster                                                             |
| meteor_contest            | 82.6 ms                                                                         | 82.0 ms: 1.01x faster                                                            |
| go                        | 116 ms                                                                          | 116 ms: 1.01x faster                                                             |
| pprint_safe_repr          | 674 ms                                                                          | 670 ms: 1.01x faster                                                             |
| mako                      | 7.64 ms                                                                         | 7.60 ms: 1.01x faster                                                            |
| sympy_str                 | 214 ms                                                                          | 213 ms: 1.00x faster                                                             |
| xml_etree_process         | 41.4 ms                                                                         | 41.5 ms: 1.00x slower                                                            |
| logging_simple            | 7.97 us                                                                         | 8.01 us: 1.00x slower                                                            |
| coverage                  | 465 ms                                                                          | 467 ms: 1.01x slower                                                             |
| deepcopy                  | 276 us                                                                          | 277 us: 1.01x slower                                                             |
| asyncio_tcp_ssl           | 16.8 sec                                                                        | 16.9 sec: 1.01x slower                                                           |
| 2to3                      | 246 ms                                                                          | 247 ms: 1.01x slower                                                             |
| tornado_http              | 95.7 ms                                                                         | 96.4 ms: 1.01x slower                                                            |
| async_tree_io             | 597 ms                                                                          | 601 ms: 1.01x slower                                                             |
| scimark_lu                | 60.1 ms                                                                         | 60.5 ms: 1.01x slower                                                            |
| regex_v8                  | 16.0 ms                                                                         | 16.1 ms: 1.01x slower                                                            |
| async_tree_none_tg        | 237 ms                                                                          | 239 ms: 1.01x slower                                                             |
| generators                | 22.4 ms                                                                         | 22.5 ms: 1.01x slower                                                            |
| logging_silent            | 60.5 ns                                                                         | 61.0 ns: 1.01x slower                                                            |
| async_tree_io_tg          | 585 ms                                                                          | 590 ms: 1.01x slower                                                             |
| regex_effbot              | 1.89 ms                                                                         | 1.91 ms: 1.01x slower                                                            |
| scimark_sparse_mat_mult   | 3.19 ms                                                                         | 3.22 ms: 1.01x slower                                                            |
| typing_runtime_protocols  | 93.8 us                                                                         | 94.9 us: 1.01x slower                                                            |
| async_tree_memoization_tg | 298 ms                                                                          | 302 ms: 1.01x slower                                                             |
| crypto_pyaes              | 60.4 ms                                                                         | 61.4 ms: 1.02x slower                                                            |
| comprehensions            | 14.7 us                                                                         | 15.0 us: 1.02x slower                                                            |
| json_dumps                | 6.71 ms                                                                         | 6.84 ms: 1.02x slower                                                            |
| pickle_pure_python        | 205 us                                                                          | 210 us: 1.03x slower                                                             |
| deepcopy_reduce           | 2.37 us                                                                         | 2.43 us: 1.03x slower                                                            |
| json                      | 4.08 ms                                                                         | 4.19 ms: 1.03x slower                                                            |
| asyncio_tcp               | 609 ms                                                                          | 627 ms: 1.03x slower                                                             |
| sqlite_synth              | 1.84 us                                                                         | 1.89 us: 1.03x slower                                                            |
| nbody                     | 90.6 ms                                                                         | 93.5 ms: 1.03x slower                                                            |
| unpickle_pure_python      | 150 us                                                                          | 155 us: 1.03x slower                                                             |
| xml_etree_iterparse       | 65.5 ms                                                                         | 67.8 ms: 1.04x slower                                                            |
| deepcopy_memo             | 22.7 us                                                                         | 23.6 us: 1.04x slower                                                            |
| richards_super            | 32.3 ms                                                                         | 33.5 ms: 1.04x slower                                                            |
| scimark_sor               | 79.9 ms                                                                         | 83.5 ms: 1.04x slower                                                            |
| xml_etree_parse           | 104 ms                                                                          | 109 ms: 1.05x slower                                                             |
| regex_dna                 | 117 ms                                                                          | 123 ms: 1.05x slower                                                             |
| nqueens                   | 86.1 ms                                                                         | 91.6 ms: 1.06x slower                                                            |
| telco                     | 6.11 ms                                                                         | 6.56 ms: 1.07x slower                                                            |
| fannkuch                  | 293 ms                                                                          | 315 ms: 1.08x slower                                                             |
| Geometric mean            | (ref)                                                                           | 1.00x slower                                                                     |

Benchmark hidden because not significant (27): bench_thread_pool, scimark_monte_carlo, unpickle, sympy_sum, pickle_dict, async_generators, deltablue, gc_traversal, python_startup, scimark_fft, pprint_pformat, float, hexiom, sympy_integrate, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, coroutines, tomli_loads, json_loads, unpack_sequence, pathlib, richards, logging_format, python_startup_no_site, async_tree_memoization, create_gc_cycles


# HPT report

- Reliability score: 85.18% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown