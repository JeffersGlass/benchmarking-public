# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.00x slower
- HPT reliability: 84.55%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 298 ms                                                                       | 300 ms: 1.01x slower                                                          |
| chameleon      | 7.54 ms                                                                      | 7.81 ms: 1.04x slower                                                         |
| tornado_http   | 124 ms                                                                       | 126 ms: 1.01x slower                                                          |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 701 ms                                                                       | 710 ms: 1.01x slower                                                          |
| async_tree_cpu_io_mixed    | 699 ms                                                                       | 708 ms: 1.01x slower                                                          |
| async_tree_io_tg           | 1.07 sec                                                                     | 1.09 sec: 1.01x slower                                                        |
| async_tree_memoization     | 547 ms                                                                       | 555 ms: 1.01x slower                                                          |
| async_tree_none_tg         | 435 ms                                                                       | 442 ms: 1.02x slower                                                          |
| async_tree_io              | 1.07 sec                                                                     | 1.09 sec: 1.02x slower                                                        |
| async_tree_none            | 431 ms                                                                       | 442 ms: 1.03x slower                                                          |
| async_tree_memoization_tg  | 545 ms                                                                       | 562 ms: 1.03x slower                                                          |
| Geometric mean             | (ref)                                                                        | 1.02x slower                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody          | 107 ms                                                                       | 104 ms: 1.03x faster                                                          |
| float          | 81.7 ms                                                                      | 80.4 ms: 1.02x faster                                                         |
| pidigits       | 263 ms                                                                       | 262 ms: 1.00x faster                                                          |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_effbot   | 3.69 ms                                                                      | 3.41 ms: 1.08x faster                                                         |
| regex_dna      | 240 ms                                                                       | 238 ms: 1.01x faster                                                          |
| regex_v8       | 26.3 ms                                                                      | 26.0 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                                        | 1.03x faster                                                                  |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_dict          | 32.7 us                                                                      | 30.8 us: 1.06x faster                                                         |
| xml_etree_iterparse  | 107 ms                                                                       | 105 ms: 1.02x faster                                                          |
| tomli_loads          | 2.31 sec                                                                     | 2.27 sec: 1.02x faster                                                        |
| xml_etree_parse      | 148 ms                                                                       | 147 ms: 1.01x faster                                                          |
| json_loads           | 25.2 us                                                                      | 25.0 us: 1.01x faster                                                         |
| pickle               | 10.5 us                                                                      | 10.4 us: 1.01x faster                                                         |
| pickle_list          | 4.44 us                                                                      | 4.40 us: 1.01x faster                                                         |
| json_dumps           | 10.5 ms                                                                      | 10.5 ms: 1.01x slower                                                         |
| xml_etree_process    | 58.2 ms                                                                      | 58.6 ms: 1.01x slower                                                         |
| unpickle_pure_python | 228 us                                                                       | 233 us: 1.02x slower                                                          |
| unpickle             | 14.8 us                                                                      | 15.2 us: 1.03x slower                                                         |
| unpickle_list        | 4.66 us                                                                      | 4.83 us: 1.03x slower                                                         |
| pickle_pure_python   | 301 us                                                                       | 314 us: 1.04x slower                                                          |
| Geometric mean       | (ref)                                                                        | 1.00x faster                                                                  |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup_no_site | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                         |
| python_startup         | 12.6 ms                                                                      | 12.7 ms: 1.00x slower                                                         |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 11.8 ms                                                                      | 11.0 ms: 1.08x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf2-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:----------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| spectral_norm              | 118 ms                                                                       | 108 ms: 1.09x faster                                                          |
| regex_effbot               | 3.69 ms                                                                      | 3.41 ms: 1.08x faster                                                         |
| mako                       | 11.8 ms                                                                      | 11.0 ms: 1.08x faster                                                         |
| pickle_dict                | 32.7 us                                                                      | 30.8 us: 1.06x faster                                                         |
| coverage                   | 81.8 ms                                                                      | 78.3 ms: 1.04x faster                                                         |
| comprehensions             | 20.7 us                                                                      | 19.9 us: 1.04x faster                                                         |
| crypto_pyaes               | 81.5 ms                                                                      | 78.3 ms: 1.04x faster                                                         |
| nbody                      | 107 ms                                                                       | 104 ms: 1.03x faster                                                          |
| scimark_sparse_mat_mult    | 5.01 ms                                                                      | 4.89 ms: 1.02x faster                                                         |
| xml_etree_iterparse        | 107 ms                                                                       | 105 ms: 1.02x faster                                                          |
| scimark_fft                | 360 ms                                                                       | 354 ms: 1.02x faster                                                          |
| hexiom                     | 7.70 ms                                                                      | 7.56 ms: 1.02x faster                                                         |
| tomli_loads                | 2.31 sec                                                                     | 2.27 sec: 1.02x faster                                                        |
| float                      | 81.7 ms                                                                      | 80.4 ms: 1.02x faster                                                         |
| pyflate                    | 521 ms                                                                       | 514 ms: 1.01x faster                                                          |
| nqueens                    | 97.4 ms                                                                      | 96.3 ms: 1.01x faster                                                         |
| regex_dna                  | 240 ms                                                                       | 238 ms: 1.01x faster                                                          |
| regex_v8                   | 26.3 ms                                                                      | 26.0 ms: 1.01x faster                                                         |
| xml_etree_parse            | 148 ms                                                                       | 147 ms: 1.01x faster                                                          |
| json_loads                 | 25.2 us                                                                      | 25.0 us: 1.01x faster                                                         |
| pickle                     | 10.5 us                                                                      | 10.4 us: 1.01x faster                                                         |
| mdp                        | 2.56 sec                                                                     | 2.53 sec: 1.01x faster                                                        |
| coroutines                 | 22.4 ms                                                                      | 22.2 ms: 1.01x faster                                                         |
| scimark_monte_carlo        | 78.5 ms                                                                      | 77.8 ms: 1.01x faster                                                         |
| pickle_list                | 4.44 us                                                                      | 4.40 us: 1.01x faster                                                         |
| async_generators           | 370 ms                                                                       | 367 ms: 1.01x faster                                                          |
| richards                   | 51.0 ms                                                                      | 50.6 ms: 1.01x faster                                                         |
| pathlib                    | 19.0 ms                                                                      | 18.9 ms: 1.01x faster                                                         |
| json                       | 5.33 ms                                                                      | 5.29 ms: 1.01x faster                                                         |
| fannkuch                   | 406 ms                                                                       | 405 ms: 1.00x faster                                                          |
| pidigits                   | 263 ms                                                                       | 262 ms: 1.00x faster                                                          |
| python_startup_no_site     | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                         |
| python_startup             | 12.6 ms                                                                      | 12.7 ms: 1.00x slower                                                         |
| sympy_str                  | 299 ms                                                                       | 300 ms: 1.00x slower                                                          |
| sympy_expand               | 501 ms                                                                       | 503 ms: 1.00x slower                                                          |
| json_dumps                 | 10.5 ms                                                                      | 10.5 ms: 1.01x slower                                                         |
| xml_etree_process          | 58.2 ms                                                                      | 58.6 ms: 1.01x slower                                                         |
| sympy_integrate            | 24.3 ms                                                                      | 24.4 ms: 1.01x slower                                                         |
| 2to3                       | 298 ms                                                                       | 300 ms: 1.01x slower                                                          |
| logging_silent             | 95.1 ns                                                                      | 95.8 ns: 1.01x slower                                                         |
| richards_super             | 56.9 ms                                                                      | 57.4 ms: 1.01x slower                                                         |
| typing_runtime_protocols   | 119 us                                                                       | 120 us: 1.01x slower                                                          |
| chaos                      | 70.3 ms                                                                      | 70.9 ms: 1.01x slower                                                         |
| sympy_sum                  | 159 ms                                                                       | 161 ms: 1.01x slower                                                          |
| tornado_http               | 124 ms                                                                       | 126 ms: 1.01x slower                                                          |
| sqlglot_normalize          | 119 ms                                                                       | 120 ms: 1.01x slower                                                          |
| create_gc_cycles           | 1.53 ms                                                                      | 1.55 ms: 1.01x slower                                                         |
| pycparser                  | 1.31 sec                                                                     | 1.33 sec: 1.01x slower                                                        |
| async_tree_cpu_io_mixed_tg | 701 ms                                                                       | 710 ms: 1.01x slower                                                          |
| meteor_contest             | 130 ms                                                                       | 132 ms: 1.01x slower                                                          |
| async_tree_cpu_io_mixed    | 699 ms                                                                       | 708 ms: 1.01x slower                                                          |
| async_tree_io_tg           | 1.07 sec                                                                     | 1.09 sec: 1.01x slower                                                        |
| scimark_sor                | 142 ms                                                                       | 144 ms: 1.01x slower                                                          |
| async_tree_memoization     | 547 ms                                                                       | 555 ms: 1.01x slower                                                          |
| async_tree_none_tg         | 435 ms                                                                       | 442 ms: 1.02x slower                                                          |
| async_tree_io              | 1.07 sec                                                                     | 1.09 sec: 1.02x slower                                                        |
| sqlglot_transpile          | 1.80 ms                                                                      | 1.83 ms: 1.02x slower                                                         |
| go                         | 169 ms                                                                       | 172 ms: 1.02x slower                                                          |
| dask                       | 403 ms                                                                       | 411 ms: 1.02x slower                                                          |
| deepcopy_reduce            | 3.34 us                                                                      | 3.41 us: 1.02x slower                                                         |
| unpickle_pure_python       | 228 us                                                                       | 233 us: 1.02x slower                                                          |
| scimark_lu                 | 97.6 ms                                                                      | 99.9 ms: 1.02x slower                                                         |
| sqlglot_parse              | 1.37 ms                                                                      | 1.40 ms: 1.02x slower                                                         |
| unpickle                   | 14.8 us                                                                      | 15.2 us: 1.03x slower                                                         |
| logging_format             | 7.33 us                                                                      | 7.53 us: 1.03x slower                                                         |
| async_tree_none            | 431 ms                                                                       | 442 ms: 1.03x slower                                                          |
| generators                 | 33.6 ms                                                                      | 34.6 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 545 ms                                                                       | 562 ms: 1.03x slower                                                          |
| logging_simple             | 6.60 us                                                                      | 6.83 us: 1.03x slower                                                         |
| unpickle_list              | 4.66 us                                                                      | 4.83 us: 1.03x slower                                                         |
| deepcopy_memo              | 37.0 us                                                                      | 38.3 us: 1.04x slower                                                         |
| chameleon                  | 7.54 ms                                                                      | 7.81 ms: 1.04x slower                                                         |
| pickle_pure_python         | 301 us                                                                       | 314 us: 1.04x slower                                                          |
| deepcopy                   | 369 us                                                                       | 385 us: 1.04x slower                                                          |
| gc_traversal               | 3.64 ms                                                                      | 3.90 ms: 1.07x slower                                                         |
| Geometric mean             | (ref)                                                                        | 1.00x slower                                                                  |

Benchmark hidden because not significant (18): pprint_safe_repr, telco, asyncio_websockets, unpack_sequence, dulwich_log, regex_compile, asyncio_tcp, sqlite_synth, asyncio_tcp_ssl, xml_etree_generate, docutils, sqlglot_optimize, pprint_pformat, bench_thread_pool, deltablue, mypy2, raytrace, bench_mp_pool


# HPT report

- Reliability score: 84.55% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x