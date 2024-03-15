# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.01x faster
- HPT reliability: 82.95%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| chameleon      | 7.54 ms                                                                      | 7.83 ms: 1.04x slower                                                         |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (3): 2to3, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|---------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_io             | 1.07 sec                                                                     | 1.08 sec: 1.00x slower                                                        |
| async_tree_none_tg        | 435 ms                                                                       | 438 ms: 1.01x slower                                                          |
| async_tree_io_tg          | 1.07 sec                                                                     | 1.08 sec: 1.01x slower                                                        |
| async_tree_memoization_tg | 545 ms                                                                       | 564 ms: 1.03x slower                                                          |
| Geometric mean            | (ref)                                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody          | 107 ms                                                                       | 98.7 ms: 1.08x faster                                                         |
| float          | 81.7 ms                                                                      | 79.4 ms: 1.03x faster                                                         |
| pidigits       | 263 ms                                                                       | 262 ms: 1.00x faster                                                          |
| Geometric mean | (ref)                                                                        | 1.04x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_effbot   | 3.69 ms                                                                      | 3.46 ms: 1.07x faster                                                         |
| regex_compile  | 146 ms                                                                       | 145 ms: 1.01x faster                                                          |
| regex_v8       | 26.3 ms                                                                      | 26.2 ms: 1.00x faster                                                         |
| regex_dna      | 240 ms                                                                       | 255 ms: 1.06x slower                                                          |
| Geometric mean | (ref)                                                                        | 1.00x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| tomli_loads          | 2.31 sec                                                                     | 2.13 sec: 1.08x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                                       | 102 ms: 1.04x faster                                                          |
| pickle_dict          | 32.7 us                                                                      | 31.9 us: 1.02x faster                                                         |
| pickle_list          | 4.44 us                                                                      | 4.37 us: 1.02x faster                                                         |
| unpickle             | 14.8 us                                                                      | 14.6 us: 1.01x faster                                                         |
| xml_etree_parse      | 148 ms                                                                       | 147 ms: 1.01x faster                                                          |
| json_dumps           | 10.5 ms                                                                      | 10.4 ms: 1.01x faster                                                         |
| xml_etree_process    | 58.2 ms                                                                      | 57.9 ms: 1.01x faster                                                         |
| xml_etree_generate   | 84.5 ms                                                                      | 84.1 ms: 1.01x faster                                                         |
| pickle               | 10.5 us                                                                      | 10.6 us: 1.01x slower                                                         |
| unpickle_pure_python | 228 us                                                                       | 232 us: 1.02x slower                                                          |
| unpickle_list        | 4.66 us                                                                      | 4.77 us: 1.02x slower                                                         |
| pickle_pure_python   | 301 us                                                                       | 314 us: 1.04x slower                                                          |
| Geometric mean       | (ref)                                                                        | 1.01x faster                                                                  |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup_no_site | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                         |
| python_startup         | 12.6 ms                                                                      | 12.6 ms: 1.00x slower                                                         |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 11.8 ms                                                                      | 10.6 ms: 1.12x faster                                                         |

All benchmarks:
===============

| Benchmark                 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|---------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| spectral_norm             | 118 ms                                                                       | 99.8 ms: 1.19x faster                                                         |
| scimark_sparse_mat_mult   | 5.01 ms                                                                      | 4.37 ms: 1.15x faster                                                         |
| mako                      | 11.8 ms                                                                      | 10.6 ms: 1.12x faster                                                         |
| scimark_fft               | 360 ms                                                                       | 325 ms: 1.11x faster                                                          |
| comprehensions            | 20.7 us                                                                      | 19.0 us: 1.09x faster                                                         |
| tomli_loads               | 2.31 sec                                                                     | 2.13 sec: 1.08x faster                                                        |
| nbody                     | 107 ms                                                                       | 98.7 ms: 1.08x faster                                                         |
| regex_effbot              | 3.69 ms                                                                      | 3.46 ms: 1.07x faster                                                         |
| gc_traversal              | 3.64 ms                                                                      | 3.43 ms: 1.06x faster                                                         |
| crypto_pyaes              | 81.5 ms                                                                      | 77.4 ms: 1.05x faster                                                         |
| nqueens                   | 97.4 ms                                                                      | 92.6 ms: 1.05x faster                                                         |
| hexiom                    | 7.70 ms                                                                      | 7.33 ms: 1.05x faster                                                         |
| xml_etree_iterparse       | 107 ms                                                                       | 102 ms: 1.04x faster                                                          |
| fannkuch                  | 406 ms                                                                       | 392 ms: 1.04x faster                                                          |
| chaos                     | 70.3 ms                                                                      | 68.3 ms: 1.03x faster                                                         |
| float                     | 81.7 ms                                                                      | 79.4 ms: 1.03x faster                                                         |
| pycparser                 | 1.31 sec                                                                     | 1.28 sec: 1.03x faster                                                        |
| pickle_dict               | 32.7 us                                                                      | 31.9 us: 1.02x faster                                                         |
| telco                     | 8.15 ms                                                                      | 8.01 ms: 1.02x faster                                                         |
| pickle_list               | 4.44 us                                                                      | 4.37 us: 1.02x faster                                                         |
| unpickle                  | 14.8 us                                                                      | 14.6 us: 1.01x faster                                                         |
| meteor_contest            | 130 ms                                                                       | 128 ms: 1.01x faster                                                          |
| pprint_safe_repr          | 847 ms                                                                       | 837 ms: 1.01x faster                                                          |
| unpack_sequence           | 45.1 ns                                                                      | 44.6 ns: 1.01x faster                                                         |
| dulwich_log               | 69.3 ms                                                                      | 68.5 ms: 1.01x faster                                                         |
| xml_etree_parse           | 148 ms                                                                       | 147 ms: 1.01x faster                                                          |
| coroutines                | 22.4 ms                                                                      | 22.2 ms: 1.01x faster                                                         |
| sqlglot_optimize          | 61.1 ms                                                                      | 60.6 ms: 1.01x faster                                                         |
| sqlglot_normalize         | 119 ms                                                                       | 118 ms: 1.01x faster                                                          |
| json                      | 5.33 ms                                                                      | 5.29 ms: 1.01x faster                                                         |
| go                        | 169 ms                                                                       | 168 ms: 1.01x faster                                                          |
| sqlite_synth              | 2.74 us                                                                      | 2.72 us: 1.01x faster                                                         |
| json_dumps                | 10.5 ms                                                                      | 10.4 ms: 1.01x faster                                                         |
| regex_compile             | 146 ms                                                                       | 145 ms: 1.01x faster                                                          |
| async_generators          | 370 ms                                                                       | 368 ms: 1.01x faster                                                          |
| xml_etree_process         | 58.2 ms                                                                      | 57.9 ms: 1.01x faster                                                         |
| xml_etree_generate        | 84.5 ms                                                                      | 84.1 ms: 1.01x faster                                                         |
| pprint_pformat            | 1.72 sec                                                                     | 1.71 sec: 1.00x faster                                                        |
| regex_v8                  | 26.3 ms                                                                      | 26.2 ms: 1.00x faster                                                         |
| sympy_sum                 | 159 ms                                                                       | 159 ms: 1.00x faster                                                          |
| pidigits                  | 263 ms                                                                       | 262 ms: 1.00x faster                                                          |
| python_startup_no_site    | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                         |
| python_startup            | 12.6 ms                                                                      | 12.6 ms: 1.00x slower                                                         |
| sympy_expand              | 501 ms                                                                       | 504 ms: 1.00x slower                                                          |
| async_tree_io             | 1.07 sec                                                                     | 1.08 sec: 1.00x slower                                                        |
| async_tree_none_tg        | 435 ms                                                                       | 438 ms: 1.01x slower                                                          |
| logging_format            | 7.33 us                                                                      | 7.38 us: 1.01x slower                                                         |
| async_tree_io_tg          | 1.07 sec                                                                     | 1.08 sec: 1.01x slower                                                        |
| richards_super            | 56.9 ms                                                                      | 57.4 ms: 1.01x slower                                                         |
| logging_silent            | 95.1 ns                                                                      | 95.9 ns: 1.01x slower                                                         |
| pickle                    | 10.5 us                                                                      | 10.6 us: 1.01x slower                                                         |
| generators                | 33.6 ms                                                                      | 33.9 ms: 1.01x slower                                                         |
| richards                  | 51.0 ms                                                                      | 51.5 ms: 1.01x slower                                                         |
| dask                      | 403 ms                                                                       | 408 ms: 1.01x slower                                                          |
| typing_runtime_protocols  | 119 us                                                                       | 121 us: 1.01x slower                                                          |
| sqlglot_transpile         | 1.80 ms                                                                      | 1.82 ms: 1.01x slower                                                         |
| unpickle_pure_python      | 228 us                                                                       | 232 us: 1.02x slower                                                          |
| deepcopy                  | 369 us                                                                       | 375 us: 1.02x slower                                                          |
| mdp                       | 2.56 sec                                                                     | 2.60 sec: 1.02x slower                                                        |
| unpickle_list             | 4.66 us                                                                      | 4.77 us: 1.02x slower                                                         |
| logging_simple            | 6.60 us                                                                      | 6.76 us: 1.02x slower                                                         |
| deepcopy_memo             | 37.0 us                                                                      | 37.9 us: 1.02x slower                                                         |
| sqlglot_parse             | 1.37 ms                                                                      | 1.41 ms: 1.03x slower                                                         |
| async_tree_memoization_tg | 545 ms                                                                       | 564 ms: 1.03x slower                                                          |
| scimark_lu                | 97.6 ms                                                                      | 101 ms: 1.04x slower                                                          |
| chameleon                 | 7.54 ms                                                                      | 7.83 ms: 1.04x slower                                                         |
| pickle_pure_python        | 301 us                                                                       | 314 us: 1.04x slower                                                          |
| regex_dna                 | 240 ms                                                                       | 255 ms: 1.06x slower                                                          |
| Geometric mean            | (ref)                                                                        | 1.01x faster                                                                  |

Benchmark hidden because not significant (25): sympy_str, docutils, deltablue, pathlib, 2to3, sympy_integrate, coverage, tornado_http, json_loads, asyncio_tcp_ssl, asyncio_websockets, mypy2, pyflate, deepcopy_reduce, asyncio_tcp, async_tree_memoization, raytrace, scimark_sor, async_tree_cpu_io_mixed, create_gc_cycles, async_tree_none, scimark_monte_carlo, async_tree_cpu_io_mixed_tg, bench_mp_pool, bench_thread_pool


# HPT report

- Reliability score: 82.95% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x