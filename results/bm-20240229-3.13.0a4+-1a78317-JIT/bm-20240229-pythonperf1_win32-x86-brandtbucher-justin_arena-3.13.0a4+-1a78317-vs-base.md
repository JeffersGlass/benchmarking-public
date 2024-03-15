# Results vs. base

- fork: brandtbucher
- ref: justin_arena
- machine: windows-x86
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 266 ms                                                                          | 260 ms: 1.02x faster                                                          |
| chameleon      | 6.00 ms                                                                         | 5.71 ms: 1.05x faster                                                         |
| docutils       | 1.87 sec                                                                        | 1.80 sec: 1.04x faster                                                        |
| html5lib       | 47.6 ms                                                                         | 45.3 ms: 1.05x faster                                                         |
| tornado_http   | 99.9 ms                                                                         | 95.9 ms: 1.04x faster                                                         |
| Geometric mean | (ref)                                                                           | 1.04x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 325 ms                                                                          | 303 ms: 1.07x faster                                                          |
| async_tree_none_tg         | 258 ms                                                                          | 242 ms: 1.06x faster                                                          |
| async_tree_memoization     | 339 ms                                                                          | 320 ms: 1.06x faster                                                          |
| async_tree_none            | 271 ms                                                                          | 257 ms: 1.06x faster                                                          |
| async_tree_io_tg           | 634 ms                                                                          | 605 ms: 1.05x faster                                                          |
| async_tree_io              | 649 ms                                                                          | 621 ms: 1.05x faster                                                          |
| async_tree_cpu_io_mixed    | 529 ms                                                                          | 518 ms: 1.02x faster                                                          |
| async_tree_cpu_io_mixed_tg | 515 ms                                                                          | 509 ms: 1.01x faster                                                          |
| Geometric mean             | (ref)                                                                           | 1.05x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 56.4 ms                                                                         | 55.1 ms: 1.03x faster                                                         |
| pidigits       | 198 ms                                                                          | 198 ms: 1.00x faster                                                          |
| Geometric mean | (ref)                                                                           | 1.01x faster                                                                  |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_dna      | 130 ms                                                                          | 116 ms: 1.11x faster                                                          |
| regex_compile  | 113 ms                                                                          | 107 ms: 1.06x faster                                                          |
| regex_effbot   | 1.96 ms                                                                         | 1.88 ms: 1.04x faster                                                         |
| Geometric mean | (ref)                                                                           | 1.05x faster                                                                  |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_pure_python   | 228 us                                                                          | 209 us: 1.09x faster                                                          |
| tomli_loads          | 1.77 sec                                                                        | 1.70 sec: 1.04x faster                                                        |
| unpickle_list        | 2.93 us                                                                         | 2.82 us: 1.04x faster                                                         |
| pickle               | 8.16 us                                                                         | 7.89 us: 1.03x faster                                                         |
| json_dumps           | 7.10 ms                                                                         | 6.87 ms: 1.03x faster                                                         |
| xml_etree_iterparse  | 68.3 ms                                                                         | 66.5 ms: 1.03x faster                                                         |
| json_loads           | 20.3 us                                                                         | 19.8 us: 1.02x faster                                                         |
| pickle_list          | 3.28 us                                                                         | 3.23 us: 1.02x faster                                                         |
| unpickle             | 10.1 us                                                                         | 10.0 us: 1.01x faster                                                         |
| pickle_dict          | 20.0 us                                                                         | 19.9 us: 1.01x faster                                                         |
| unpickle_pure_python | 170 us                                                                          | 171 us: 1.01x slower                                                          |
| xml_etree_generate   | 61.7 ms                                                                         | 62.5 ms: 1.01x slower                                                         |
| Geometric mean       | (ref)                                                                           | 1.02x faster                                                                  |

Benchmark hidden because not significant (2): xml_etree_process, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup_no_site | 24.0 ms                                                                         | 23.6 ms: 1.02x faster                                                         |
| python_startup         | 26.0 ms                                                                         | 25.7 ms: 1.01x faster                                                         |
| Geometric mean         | (ref)                                                                           | 1.01x faster                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| django_template | 31.9 ms                                                                         | 29.9 ms: 1.06x faster                                                         |
| genshi_text     | 23.9 ms                                                                         | 22.5 ms: 1.06x faster                                                         |
| genshi_xml      | 51.0 ms                                                                         | 50.1 ms: 1.02x faster                                                         |
| mako            | 7.19 ms                                                                         | 7.12 ms: 1.01x faster                                                         |
| Geometric mean  | (ref)                                                                           | 1.04x faster                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| logging_silent             | 68.8 ns                                                                         | 59.6 ns: 1.15x faster                                                         |
| deepcopy_memo              | 28.0 us                                                                         | 24.4 us: 1.15x faster                                                         |
| generators                 | 25.0 ms                                                                         | 22.1 ms: 1.13x faster                                                         |
| richards                   | 37.9 ms                                                                         | 33.6 ms: 1.13x faster                                                         |
| richards_super             | 42.3 ms                                                                         | 37.7 ms: 1.12x faster                                                         |
| regex_dna                  | 130 ms                                                                          | 116 ms: 1.11x faster                                                          |
| go                         | 130 ms                                                                          | 118 ms: 1.10x faster                                                          |
| pickle_pure_python         | 228 us                                                                          | 209 us: 1.09x faster                                                          |
| deepcopy_reduce            | 2.59 us                                                                         | 2.36 us: 1.09x faster                                                         |
| deltablue                  | 2.75 ms                                                                         | 2.52 ms: 1.09x faster                                                         |
| sqlglot_normalize          | 241 ms                                                                          | 221 ms: 1.09x faster                                                          |
| sqlglot_transpile          | 1.30 ms                                                                         | 1.21 ms: 1.07x faster                                                         |
| deepcopy                   | 296 us                                                                          | 276 us: 1.07x faster                                                          |
| pycparser                  | 902 ms                                                                          | 842 ms: 1.07x faster                                                          |
| async_tree_memoization_tg  | 325 ms                                                                          | 303 ms: 1.07x faster                                                          |
| sqlglot_parse              | 1.03 ms                                                                         | 965 us: 1.07x faster                                                          |
| django_template            | 31.9 ms                                                                         | 29.9 ms: 1.06x faster                                                         |
| async_tree_none_tg         | 258 ms                                                                          | 242 ms: 1.06x faster                                                          |
| unpack_sequence            | 44.3 ns                                                                         | 41.7 ns: 1.06x faster                                                         |
| genshi_text                | 23.9 ms                                                                         | 22.5 ms: 1.06x faster                                                         |
| regex_compile              | 113 ms                                                                          | 107 ms: 1.06x faster                                                          |
| async_tree_memoization     | 339 ms                                                                          | 320 ms: 1.06x faster                                                          |
| sympy_integrate            | 16.3 ms                                                                         | 15.4 ms: 1.06x faster                                                         |
| coroutines                 | 15.2 ms                                                                         | 14.4 ms: 1.06x faster                                                         |
| sqlglot_optimize           | 47.8 ms                                                                         | 45.3 ms: 1.06x faster                                                         |
| async_tree_none            | 271 ms                                                                          | 257 ms: 1.06x faster                                                          |
| sympy_str                  | 219 ms                                                                          | 209 ms: 1.05x faster                                                          |
| chameleon                  | 6.00 ms                                                                         | 5.71 ms: 1.05x faster                                                         |
| html5lib                   | 47.6 ms                                                                         | 45.3 ms: 1.05x faster                                                         |
| chaos                      | 62.4 ms                                                                         | 59.5 ms: 1.05x faster                                                         |
| async_tree_io_tg           | 634 ms                                                                          | 605 ms: 1.05x faster                                                          |
| sympy_expand               | 383 ms                                                                          | 366 ms: 1.05x faster                                                          |
| dask                       | 439 ms                                                                          | 419 ms: 1.05x faster                                                          |
| async_tree_io              | 649 ms                                                                          | 621 ms: 1.05x faster                                                          |
| pylint                     | 236 ms                                                                          | 226 ms: 1.05x faster                                                          |
| sympy_sum                  | 112 ms                                                                          | 107 ms: 1.05x faster                                                          |
| regex_effbot               | 1.96 ms                                                                         | 1.88 ms: 1.04x faster                                                         |
| tornado_http               | 99.9 ms                                                                         | 95.9 ms: 1.04x faster                                                         |
| docutils                   | 1.87 sec                                                                        | 1.80 sec: 1.04x faster                                                        |
| tomli_loads                | 1.77 sec                                                                        | 1.70 sec: 1.04x faster                                                        |
| raytrace                   | 284 ms                                                                          | 273 ms: 1.04x faster                                                          |
| unpickle_list              | 2.93 us                                                                         | 2.82 us: 1.04x faster                                                         |
| scimark_sor                | 102 ms                                                                          | 98.4 ms: 1.04x faster                                                         |
| pickle                     | 8.16 us                                                                         | 7.89 us: 1.03x faster                                                         |
| json_dumps                 | 7.10 ms                                                                         | 6.87 ms: 1.03x faster                                                         |
| thrift                     | 11.0 ms                                                                         | 10.7 ms: 1.03x faster                                                         |
| typing_runtime_protocols   | 101 us                                                                          | 97.7 us: 1.03x faster                                                         |
| xml_etree_iterparse        | 68.3 ms                                                                         | 66.5 ms: 1.03x faster                                                         |
| coverage                   | 497 ms                                                                          | 484 ms: 1.03x faster                                                          |
| float                      | 56.4 ms                                                                         | 55.1 ms: 1.03x faster                                                         |
| 2to3                       | 266 ms                                                                          | 260 ms: 1.02x faster                                                          |
| json_loads                 | 20.3 us                                                                         | 19.8 us: 1.02x faster                                                         |
| logging_format             | 9.07 us                                                                         | 8.87 us: 1.02x faster                                                         |
| async_tree_cpu_io_mixed    | 529 ms                                                                          | 518 ms: 1.02x faster                                                          |
| bench_mp_pool              | 74.5 ms                                                                         | 73.1 ms: 1.02x faster                                                         |
| scimark_monte_carlo        | 66.3 ms                                                                         | 65.1 ms: 1.02x faster                                                         |
| pickle_list                | 3.28 us                                                                         | 3.23 us: 1.02x faster                                                         |
| python_startup_no_site     | 24.0 ms                                                                         | 23.6 ms: 1.02x faster                                                         |
| hexiom                     | 6.40 ms                                                                         | 6.29 ms: 1.02x faster                                                         |
| genshi_xml                 | 51.0 ms                                                                         | 50.1 ms: 1.02x faster                                                         |
| async_generators           | 307 ms                                                                          | 302 ms: 1.02x faster                                                          |
| create_gc_cycles           | 668 us                                                                          | 658 us: 1.02x faster                                                          |
| logging_simple             | 8.37 us                                                                         | 8.26 us: 1.01x faster                                                         |
| python_startup             | 26.0 ms                                                                         | 25.7 ms: 1.01x faster                                                         |
| pyflate                    | 385 ms                                                                          | 380 ms: 1.01x faster                                                          |
| async_tree_cpu_io_mixed_tg | 515 ms                                                                          | 509 ms: 1.01x faster                                                          |
| unpickle                   | 10.1 us                                                                         | 10.0 us: 1.01x faster                                                         |
| json                       | 4.28 ms                                                                         | 4.24 ms: 1.01x faster                                                         |
| mako                       | 7.19 ms                                                                         | 7.12 ms: 1.01x faster                                                         |
| pickle_dict                | 20.0 us                                                                         | 19.9 us: 1.01x faster                                                         |
| scimark_fft                | 242 ms                                                                          | 240 ms: 1.01x faster                                                          |
| crypto_pyaes               | 60.8 ms                                                                         | 60.3 ms: 1.01x faster                                                         |
| mdp                        | 1.77 sec                                                                        | 1.75 sec: 1.01x faster                                                        |
| pprint_pformat             | 1.52 sec                                                                        | 1.51 sec: 1.01x faster                                                        |
| fannkuch                   | 347 ms                                                                          | 345 ms: 1.01x faster                                                          |
| pidigits                   | 198 ms                                                                          | 198 ms: 1.00x faster                                                          |
| spectral_norm              | 73.7 ms                                                                         | 74.0 ms: 1.00x slower                                                         |
| unpickle_pure_python       | 170 us                                                                          | 171 us: 1.01x slower                                                          |
| gc_traversal               | 1.40 ms                                                                         | 1.41 ms: 1.01x slower                                                         |
| sqlite_synth               | 1.91 us                                                                         | 1.92 us: 1.01x slower                                                         |
| xml_etree_generate         | 61.7 ms                                                                         | 62.5 ms: 1.01x slower                                                         |
| scimark_sparse_mat_mult    | 3.14 ms                                                                         | 3.18 ms: 1.01x slower                                                         |
| comprehensions             | 14.6 us                                                                         | 14.9 us: 1.02x slower                                                         |
| telco                      | 6.16 ms                                                                         | 6.35 ms: 1.03x slower                                                         |
| Geometric mean             | (ref)                                                                           | 1.04x faster                                                                  |

Benchmark hidden because not significant (12): bench_thread_pool, asyncio_tcp, pathlib, nqueens, nbody, pprint_safe_repr, xml_etree_process, xml_etree_parse, meteor_contest, asyncio_tcp_ssl, regex_v8, scimark_lu


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown