# Results vs. base

- fork: brandtbucher
- ref: justin_nops
- machine: windows-x86
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 266 ms                                                                          | 259 ms: 1.03x faster                                                         |
| chameleon      | 6.00 ms                                                                         | 5.58 ms: 1.08x faster                                                        |
| docutils       | 1.87 sec                                                                        | 1.79 sec: 1.05x faster                                                       |
| html5lib       | 47.6 ms                                                                         | 44.4 ms: 1.07x faster                                                        |
| tornado_http   | 99.9 ms                                                                         | 96.1 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                                           | 1.05x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 325 ms                                                                          | 306 ms: 1.06x faster                                                         |
| async_tree_memoization     | 339 ms                                                                          | 324 ms: 1.05x faster                                                         |
| async_tree_none            | 271 ms                                                                          | 261 ms: 1.04x faster                                                         |
| async_tree_io_tg           | 634 ms                                                                          | 611 ms: 1.04x faster                                                         |
| async_tree_none_tg         | 258 ms                                                                          | 249 ms: 1.04x faster                                                         |
| async_tree_io              | 649 ms                                                                          | 630 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed_tg | 515 ms                                                                          | 509 ms: 1.01x faster                                                         |
| Geometric mean             | (ref)                                                                           | 1.03x faster                                                                 |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 96.7 ms                                                                         | 92.6 ms: 1.04x faster                                                        |
| float          | 56.4 ms                                                                         | 55.0 ms: 1.03x faster                                                        |
| Geometric mean | (ref)                                                                           | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 130 ms                                                                          | 118 ms: 1.10x faster                                                         |
| regex_compile  | 113 ms                                                                          | 107 ms: 1.06x faster                                                         |
| regex_effbot   | 1.96 ms                                                                         | 1.87 ms: 1.05x faster                                                        |
| regex_v8       | 16.1 ms                                                                         | 15.9 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                                           | 1.05x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 228 us                                                                          | 208 us: 1.10x faster                                                         |
| tomli_loads          | 1.77 sec                                                                        | 1.68 sec: 1.05x faster                                                       |
| pickle               | 8.16 us                                                                         | 7.91 us: 1.03x faster                                                        |
| xml_etree_iterparse  | 68.3 ms                                                                         | 67.2 ms: 1.02x faster                                                        |
| pickle_list          | 3.28 us                                                                         | 3.23 us: 1.02x faster                                                        |
| json_loads           | 20.3 us                                                                         | 19.9 us: 1.02x faster                                                        |
| unpickle_pure_python | 170 us                                                                          | 168 us: 1.01x faster                                                         |
| xml_etree_process    | 42.8 ms                                                                         | 42.5 ms: 1.01x faster                                                        |
| unpickle_list        | 2.93 us                                                                         | 2.91 us: 1.01x faster                                                        |
| unpickle             | 10.1 us                                                                         | 10.1 us: 1.00x faster                                                        |
| pickle_dict          | 20.0 us                                                                         | 20.4 us: 1.02x slower                                                        |
| Geometric mean       | (ref)                                                                           | 1.02x faster                                                                 |

Benchmark hidden because not significant (3): json_dumps, xml_etree_parse, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 24.0 ms                                                                         | 24.4 ms: 1.02x slower                                                        |
| python_startup         | 26.0 ms                                                                         | 26.9 ms: 1.03x slower                                                        |
| Geometric mean         | (ref)                                                                           | 1.02x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 31.9 ms                                                                         | 30.2 ms: 1.06x faster                                                        |
| genshi_xml      | 51.0 ms                                                                         | 49.5 ms: 1.03x faster                                                        |
| genshi_text     | 23.9 ms                                                                         | 23.4 ms: 1.02x faster                                                        |
| Geometric mean  | (ref)                                                                           | 1.03x faster                                                                 |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:-------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| deepcopy_memo              | 28.0 us                                                                         | 23.8 us: 1.18x faster                                                        |
| logging_silent             | 68.8 ns                                                                         | 59.6 ns: 1.15x faster                                                        |
| generators                 | 25.0 ms                                                                         | 22.2 ms: 1.12x faster                                                        |
| regex_dna                  | 130 ms                                                                          | 118 ms: 1.10x faster                                                         |
| pickle_pure_python         | 228 us                                                                          | 208 us: 1.10x faster                                                         |
| deepcopy_reduce            | 2.59 us                                                                         | 2.38 us: 1.09x faster                                                        |
| async_generators           | 307 ms                                                                          | 283 ms: 1.08x faster                                                         |
| deltablue                  | 2.75 ms                                                                         | 2.55 ms: 1.08x faster                                                        |
| raytrace                   | 284 ms                                                                          | 263 ms: 1.08x faster                                                         |
| sqlglot_normalize          | 241 ms                                                                          | 223 ms: 1.08x faster                                                         |
| go                         | 130 ms                                                                          | 120 ms: 1.08x faster                                                         |
| chameleon                  | 6.00 ms                                                                         | 5.58 ms: 1.08x faster                                                        |
| sqlglot_transpile          | 1.30 ms                                                                         | 1.21 ms: 1.07x faster                                                        |
| html5lib                   | 47.6 ms                                                                         | 44.4 ms: 1.07x faster                                                        |
| deepcopy                   | 296 us                                                                          | 277 us: 1.07x faster                                                         |
| typing_runtime_protocols   | 101 us                                                                          | 94.0 us: 1.07x faster                                                        |
| coroutines                 | 15.2 ms                                                                         | 14.2 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 325 ms                                                                          | 306 ms: 1.06x faster                                                         |
| chaos                      | 62.4 ms                                                                         | 58.8 ms: 1.06x faster                                                        |
| richards                   | 37.9 ms                                                                         | 35.8 ms: 1.06x faster                                                        |
| scimark_lu                 | 86.9 ms                                                                         | 82.3 ms: 1.06x faster                                                        |
| django_template            | 31.9 ms                                                                         | 30.2 ms: 1.06x faster                                                        |
| regex_compile              | 113 ms                                                                          | 107 ms: 1.06x faster                                                         |
| sympy_integrate            | 16.3 ms                                                                         | 15.4 ms: 1.06x faster                                                        |
| sqlglot_parse              | 1.03 ms                                                                         | 976 us: 1.05x faster                                                         |
| tomli_loads                | 1.77 sec                                                                        | 1.68 sec: 1.05x faster                                                       |
| pycparser                  | 902 ms                                                                          | 857 ms: 1.05x faster                                                         |
| sympy_expand               | 383 ms                                                                          | 364 ms: 1.05x faster                                                         |
| logging_format             | 9.07 us                                                                         | 8.63 us: 1.05x faster                                                        |
| sqlglot_optimize           | 47.8 ms                                                                         | 45.5 ms: 1.05x faster                                                        |
| sympy_str                  | 219 ms                                                                          | 209 ms: 1.05x faster                                                         |
| richards_super             | 42.3 ms                                                                         | 40.3 ms: 1.05x faster                                                        |
| dask                       | 439 ms                                                                          | 418 ms: 1.05x faster                                                         |
| regex_effbot               | 1.96 ms                                                                         | 1.87 ms: 1.05x faster                                                        |
| async_tree_memoization     | 339 ms                                                                          | 324 ms: 1.05x faster                                                         |
| docutils                   | 1.87 sec                                                                        | 1.79 sec: 1.05x faster                                                       |
| nbody                      | 96.7 ms                                                                         | 92.6 ms: 1.04x faster                                                        |
| sympy_sum                  | 112 ms                                                                          | 107 ms: 1.04x faster                                                         |
| pylint                     | 236 ms                                                                          | 227 ms: 1.04x faster                                                         |
| async_tree_none            | 271 ms                                                                          | 261 ms: 1.04x faster                                                         |
| tornado_http               | 99.9 ms                                                                         | 96.1 ms: 1.04x faster                                                        |
| bench_thread_pool          | 1.07 ms                                                                         | 1.03 ms: 1.04x faster                                                        |
| comprehensions             | 14.6 us                                                                         | 14.1 us: 1.04x faster                                                        |
| async_tree_io_tg           | 634 ms                                                                          | 611 ms: 1.04x faster                                                         |
| crypto_pyaes               | 60.8 ms                                                                         | 58.6 ms: 1.04x faster                                                        |
| logging_simple             | 8.37 us                                                                         | 8.07 us: 1.04x faster                                                        |
| async_tree_none_tg         | 258 ms                                                                          | 249 ms: 1.04x faster                                                         |
| hexiom                     | 6.40 ms                                                                         | 6.20 ms: 1.03x faster                                                        |
| nqueens                    | 94.7 ms                                                                         | 91.9 ms: 1.03x faster                                                        |
| async_tree_io              | 649 ms                                                                          | 630 ms: 1.03x faster                                                         |
| pickle                     | 8.16 us                                                                         | 7.91 us: 1.03x faster                                                        |
| thrift                     | 11.0 ms                                                                         | 10.7 ms: 1.03x faster                                                        |
| genshi_xml                 | 51.0 ms                                                                         | 49.5 ms: 1.03x faster                                                        |
| scimark_fft                | 242 ms                                                                          | 235 ms: 1.03x faster                                                         |
| 2to3                       | 266 ms                                                                          | 259 ms: 1.03x faster                                                         |
| float                      | 56.4 ms                                                                         | 55.0 ms: 1.03x faster                                                        |
| fannkuch                   | 347 ms                                                                          | 339 ms: 1.03x faster                                                         |
| json                       | 4.28 ms                                                                         | 4.19 ms: 1.02x faster                                                        |
| scimark_sor                | 102 ms                                                                          | 100 ms: 1.02x faster                                                         |
| pprint_pformat             | 1.52 sec                                                                        | 1.49 sec: 1.02x faster                                                       |
| scimark_monte_carlo        | 66.3 ms                                                                         | 65.1 ms: 1.02x faster                                                        |
| genshi_text                | 23.9 ms                                                                         | 23.4 ms: 1.02x faster                                                        |
| xml_etree_iterparse        | 68.3 ms                                                                         | 67.2 ms: 1.02x faster                                                        |
| meteor_contest             | 85.9 ms                                                                         | 84.5 ms: 1.02x faster                                                        |
| mdp                        | 1.77 sec                                                                        | 1.74 sec: 1.02x faster                                                       |
| pickle_list                | 3.28 us                                                                         | 3.23 us: 1.02x faster                                                        |
| json_loads                 | 20.3 us                                                                         | 19.9 us: 1.02x faster                                                        |
| pprint_safe_repr           | 745 ms                                                                          | 733 ms: 1.02x faster                                                         |
| coverage                   | 497 ms                                                                          | 490 ms: 1.01x faster                                                         |
| unpickle_pure_python       | 170 us                                                                          | 168 us: 1.01x faster                                                         |
| unpack_sequence            | 44.3 ns                                                                         | 43.7 ns: 1.01x faster                                                        |
| async_tree_cpu_io_mixed_tg | 515 ms                                                                          | 509 ms: 1.01x faster                                                         |
| regex_v8                   | 16.1 ms                                                                         | 15.9 ms: 1.01x faster                                                        |
| xml_etree_process          | 42.8 ms                                                                         | 42.5 ms: 1.01x faster                                                        |
| unpickle_list              | 2.93 us                                                                         | 2.91 us: 1.01x faster                                                        |
| pathlib                    | 84.7 ms                                                                         | 84.2 ms: 1.01x faster                                                        |
| pyflate                    | 385 ms                                                                          | 383 ms: 1.01x faster                                                         |
| unpickle                   | 10.1 us                                                                         | 10.1 us: 1.00x faster                                                        |
| python_startup_no_site     | 24.0 ms                                                                         | 24.4 ms: 1.02x slower                                                        |
| pickle_dict                | 20.0 us                                                                         | 20.4 us: 1.02x slower                                                        |
| telco                      | 6.16 ms                                                                         | 6.34 ms: 1.03x slower                                                        |
| python_startup             | 26.0 ms                                                                         | 26.9 ms: 1.03x slower                                                        |
| sqlite_synth               | 1.91 us                                                                         | 1.97 us: 1.03x slower                                                        |
| bench_mp_pool              | 74.5 ms                                                                         | 77.5 ms: 1.04x slower                                                        |
| spectral_norm              | 73.7 ms                                                                         | 77.2 ms: 1.05x slower                                                        |
| Geometric mean             | (ref)                                                                           | 1.04x faster                                                                 |

Benchmark hidden because not significant (11): asyncio_tcp, create_gc_cycles, async_tree_cpu_io_mixed, json_dumps, xml_etree_parse, asyncio_tcp_ssl, mako, pidigits, scimark_sparse_mat_mult, xml_etree_generate, gc_traversal


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown