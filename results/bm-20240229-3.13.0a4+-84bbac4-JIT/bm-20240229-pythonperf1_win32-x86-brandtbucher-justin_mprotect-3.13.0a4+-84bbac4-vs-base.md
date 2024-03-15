# Results vs. base

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-x86
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 266 ms                                                                          | 260 ms: 1.02x faster                                                             |
| chameleon      | 6.00 ms                                                                         | 5.66 ms: 1.06x faster                                                            |
| docutils       | 1.87 sec                                                                        | 1.81 sec: 1.03x faster                                                           |
| tornado_http   | 99.9 ms                                                                         | 96.7 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                                           | 1.04x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 325 ms                                                                          | 304 ms: 1.07x faster                                                             |
| async_tree_none_tg         | 258 ms                                                                          | 242 ms: 1.06x faster                                                             |
| async_tree_memoization     | 339 ms                                                                          | 323 ms: 1.05x faster                                                             |
| async_tree_none            | 271 ms                                                                          | 258 ms: 1.05x faster                                                             |
| async_tree_io_tg           | 634 ms                                                                          | 605 ms: 1.05x faster                                                             |
| async_tree_io              | 649 ms                                                                          | 624 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 529 ms                                                                          | 517 ms: 1.02x faster                                                             |
| async_tree_cpu_io_mixed_tg | 515 ms                                                                          | 504 ms: 1.02x faster                                                             |
| Geometric mean             | (ref)                                                                           | 1.05x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 56.4 ms                                                                         | 54.9 ms: 1.03x faster                                                            |
| nbody          | 96.7 ms                                                                         | 96.4 ms: 1.00x faster                                                            |
| pidigits       | 198 ms                                                                          | 198 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                                           | 1.01x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 130 ms                                                                          | 121 ms: 1.07x faster                                                             |
| regex_effbot   | 1.96 ms                                                                         | 1.89 ms: 1.04x faster                                                            |
| regex_compile  | 113 ms                                                                          | 109 ms: 1.04x faster                                                             |
| regex_v8       | 16.1 ms                                                                         | 16.0 ms: 1.00x faster                                                            |
| Geometric mean | (ref)                                                                           | 1.04x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 228 us                                                                          | 210 us: 1.09x faster                                                             |
| unpickle_list        | 2.93 us                                                                         | 2.81 us: 1.04x faster                                                            |
| xml_etree_generate   | 61.7 ms                                                                         | 59.6 ms: 1.04x faster                                                            |
| pickle_list          | 3.28 us                                                                         | 3.17 us: 1.04x faster                                                            |
| json_dumps           | 7.10 ms                                                                         | 6.86 ms: 1.03x faster                                                            |
| pickle               | 8.16 us                                                                         | 7.94 us: 1.03x faster                                                            |
| tomli_loads          | 1.77 sec                                                                        | 1.72 sec: 1.03x faster                                                           |
| xml_etree_process    | 42.8 ms                                                                         | 42.1 ms: 1.02x faster                                                            |
| xml_etree_iterparse  | 68.3 ms                                                                         | 67.3 ms: 1.01x faster                                                            |
| json_loads           | 20.3 us                                                                         | 20.1 us: 1.01x faster                                                            |
| unpickle_pure_python | 170 us                                                                          | 171 us: 1.01x slower                                                             |
| Geometric mean       | (ref)                                                                           | 1.02x faster                                                                     |

Benchmark hidden because not significant (3): unpickle, pickle_dict, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 24.0 ms                                                                         | 23.6 ms: 1.01x faster                                                            |
| python_startup         | 26.0 ms                                                                         | 25.7 ms: 1.01x faster                                                            |
| Geometric mean         | (ref)                                                                           | 1.01x faster                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 7.19 ms                                                                         | 7.30 ms: 1.01x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:-------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| logging_silent             | 68.8 ns                                                                         | 59.6 ns: 1.15x faster                                                            |
| deepcopy_memo              | 28.0 us                                                                         | 24.3 us: 1.15x faster                                                            |
| sqlglot_normalize          | 241 ms                                                                          | 216 ms: 1.11x faster                                                             |
| typing_runtime_protocols   | 101 us                                                                          | 92.1 us: 1.09x faster                                                            |
| richards                   | 37.9 ms                                                                         | 34.9 ms: 1.09x faster                                                            |
| pickle_pure_python         | 228 us                                                                          | 210 us: 1.09x faster                                                             |
| generators                 | 25.0 ms                                                                         | 23.0 ms: 1.08x faster                                                            |
| richards_super             | 42.3 ms                                                                         | 39.2 ms: 1.08x faster                                                            |
| coroutines                 | 15.2 ms                                                                         | 14.1 ms: 1.08x faster                                                            |
| go                         | 130 ms                                                                          | 120 ms: 1.08x faster                                                             |
| regex_dna                  | 130 ms                                                                          | 121 ms: 1.07x faster                                                             |
| async_tree_memoization_tg  | 325 ms                                                                          | 304 ms: 1.07x faster                                                             |
| async_tree_none_tg         | 258 ms                                                                          | 242 ms: 1.06x faster                                                             |
| deltablue                  | 2.75 ms                                                                         | 2.59 ms: 1.06x faster                                                            |
| deepcopy                   | 296 us                                                                          | 278 us: 1.06x faster                                                             |
| dask                       | 439 ms                                                                          | 413 ms: 1.06x faster                                                             |
| chameleon                  | 6.00 ms                                                                         | 5.66 ms: 1.06x faster                                                            |
| sqlglot_transpile          | 1.30 ms                                                                         | 1.23 ms: 1.06x faster                                                            |
| sympy_integrate            | 16.3 ms                                                                         | 15.4 ms: 1.06x faster                                                            |
| sqlglot_optimize           | 47.8 ms                                                                         | 45.3 ms: 1.05x faster                                                            |
| async_generators           | 307 ms                                                                          | 292 ms: 1.05x faster                                                             |
| sqlglot_parse              | 1.03 ms                                                                         | 979 us: 1.05x faster                                                             |
| pycparser                  | 902 ms                                                                          | 859 ms: 1.05x faster                                                             |
| async_tree_memoization     | 339 ms                                                                          | 323 ms: 1.05x faster                                                             |
| async_tree_none            | 271 ms                                                                          | 258 ms: 1.05x faster                                                             |
| async_tree_io_tg           | 634 ms                                                                          | 605 ms: 1.05x faster                                                             |
| sympy_sum                  | 112 ms                                                                          | 107 ms: 1.05x faster                                                             |
| coverage                   | 497 ms                                                                          | 477 ms: 1.04x faster                                                             |
| sympy_str                  | 219 ms                                                                          | 210 ms: 1.04x faster                                                             |
| unpickle_list              | 2.93 us                                                                         | 2.81 us: 1.04x faster                                                            |
| scimark_lu                 | 86.9 ms                                                                         | 83.5 ms: 1.04x faster                                                            |
| async_tree_io              | 649 ms                                                                          | 624 ms: 1.04x faster                                                             |
| regex_effbot               | 1.96 ms                                                                         | 1.89 ms: 1.04x faster                                                            |
| meteor_contest             | 85.9 ms                                                                         | 82.8 ms: 1.04x faster                                                            |
| logging_format             | 9.07 us                                                                         | 8.74 us: 1.04x faster                                                            |
| sympy_expand               | 383 ms                                                                          | 370 ms: 1.04x faster                                                             |
| nqueens                    | 94.7 ms                                                                         | 91.4 ms: 1.04x faster                                                            |
| xml_etree_generate         | 61.7 ms                                                                         | 59.6 ms: 1.04x faster                                                            |
| spectral_norm              | 73.7 ms                                                                         | 71.2 ms: 1.04x faster                                                            |
| chaos                      | 62.4 ms                                                                         | 60.3 ms: 1.04x faster                                                            |
| scimark_fft                | 242 ms                                                                          | 233 ms: 1.04x faster                                                             |
| bench_thread_pool          | 1.07 ms                                                                         | 1.03 ms: 1.04x faster                                                            |
| pickle_list                | 3.28 us                                                                         | 3.17 us: 1.04x faster                                                            |
| regex_compile              | 113 ms                                                                          | 109 ms: 1.04x faster                                                             |
| json_dumps                 | 7.10 ms                                                                         | 6.86 ms: 1.03x faster                                                            |
| docutils                   | 1.87 sec                                                                        | 1.81 sec: 1.03x faster                                                           |
| raytrace                   | 284 ms                                                                          | 275 ms: 1.03x faster                                                             |
| tornado_http               | 99.9 ms                                                                         | 96.7 ms: 1.03x faster                                                            |
| deepcopy_reduce            | 2.59 us                                                                         | 2.51 us: 1.03x faster                                                            |
| hexiom                     | 6.40 ms                                                                         | 6.21 ms: 1.03x faster                                                            |
| float                      | 56.4 ms                                                                         | 54.9 ms: 1.03x faster                                                            |
| unpack_sequence            | 44.3 ns                                                                         | 43.1 ns: 1.03x faster                                                            |
| pickle                     | 8.16 us                                                                         | 7.94 us: 1.03x faster                                                            |
| logging_simple             | 8.37 us                                                                         | 8.15 us: 1.03x faster                                                            |
| tomli_loads                | 1.77 sec                                                                        | 1.72 sec: 1.03x faster                                                           |
| 2to3                       | 266 ms                                                                          | 260 ms: 1.02x faster                                                             |
| scimark_monte_carlo        | 66.3 ms                                                                         | 64.9 ms: 1.02x faster                                                            |
| async_tree_cpu_io_mixed    | 529 ms                                                                          | 517 ms: 1.02x faster                                                             |
| json                       | 4.28 ms                                                                         | 4.19 ms: 1.02x faster                                                            |
| async_tree_cpu_io_mixed_tg | 515 ms                                                                          | 504 ms: 1.02x faster                                                             |
| scimark_sor                | 102 ms                                                                          | 100 ms: 1.02x faster                                                             |
| xml_etree_process          | 42.8 ms                                                                         | 42.1 ms: 1.02x faster                                                            |
| mdp                        | 1.77 sec                                                                        | 1.74 sec: 1.02x faster                                                           |
| python_startup_no_site     | 24.0 ms                                                                         | 23.6 ms: 1.01x faster                                                            |
| xml_etree_iterparse        | 68.3 ms                                                                         | 67.3 ms: 1.01x faster                                                            |
| pprint_safe_repr           | 745 ms                                                                          | 735 ms: 1.01x faster                                                             |
| python_startup             | 26.0 ms                                                                         | 25.7 ms: 1.01x faster                                                            |
| pyflate                    | 385 ms                                                                          | 382 ms: 1.01x faster                                                             |
| crypto_pyaes               | 60.8 ms                                                                         | 60.3 ms: 1.01x faster                                                            |
| bench_mp_pool              | 74.5 ms                                                                         | 73.9 ms: 1.01x faster                                                            |
| fannkuch                   | 347 ms                                                                          | 344 ms: 1.01x faster                                                             |
| json_loads                 | 20.3 us                                                                         | 20.1 us: 1.01x faster                                                            |
| pathlib                    | 84.7 ms                                                                         | 84.2 ms: 1.01x faster                                                            |
| pprint_pformat             | 1.52 sec                                                                        | 1.51 sec: 1.00x faster                                                           |
| regex_v8                   | 16.1 ms                                                                         | 16.0 ms: 1.00x faster                                                            |
| nbody                      | 96.7 ms                                                                         | 96.4 ms: 1.00x faster                                                            |
| pidigits                   | 198 ms                                                                          | 198 ms: 1.00x faster                                                             |
| scimark_sparse_mat_mult    | 3.14 ms                                                                         | 3.15 ms: 1.00x slower                                                            |
| unpickle_pure_python       | 170 us                                                                          | 171 us: 1.01x slower                                                             |
| sqlite_synth               | 1.91 us                                                                         | 1.93 us: 1.01x slower                                                            |
| mako                       | 7.19 ms                                                                         | 7.30 ms: 1.01x slower                                                            |
| gc_traversal               | 1.40 ms                                                                         | 1.42 ms: 1.01x slower                                                            |
| telco                      | 6.16 ms                                                                         | 6.43 ms: 1.04x slower                                                            |
| Geometric mean             | (ref)                                                                           | 1.03x faster                                                                     |

Benchmark hidden because not significant (7): asyncio_tcp, unpickle, create_gc_cycles, pickle_dict, asyncio_tcp_ssl, comprehensions, xml_etree_parse
Ignored benchmarks (6) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: django_template, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown