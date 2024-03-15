# Results vs. base

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.01x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 277 ms                                                                 | 275 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (3): chameleon, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io              | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                               |
| async_tree_memoization     | 572 ms                                                                 | 565 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed    | 720 ms                                                                 | 711 ms: 1.01x faster                                                 |
| async_tree_none_tg         | 453 ms                                                                 | 448 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed_tg | 731 ms                                                                 | 723 ms: 1.01x faster                                                 |
| async_tree_io_tg           | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                               |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (2): async_tree_none, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 102 ms                                                                 | 88.2 ms: 1.16x faster                                                |
| float          | 87.2 ms                                                                | 81.7 ms: 1.07x faster                                                |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.07x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.65 ms                                                                | 3.58 ms: 1.02x faster                                                |
| regex_compile  | 142 ms                                                                 | 140 ms: 1.01x faster                                                 |
| regex_dna      | 222 ms                                                                 | 224 ms: 1.01x slower                                                 |
| regex_v8       | 24.8 ms                                                                | 25.6 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                                | 4.98 us: 1.06x faster                                                |
| unpickle             | 16.3 us                                                                | 15.5 us: 1.05x faster                                                |
| tomli_loads          | 2.21 sec                                                               | 2.14 sec: 1.03x faster                                               |
| xml_etree_iterparse  | 109 ms                                                                 | 106 ms: 1.03x faster                                                 |
| pickle_list          | 5.13 us                                                                | 4.99 us: 1.03x faster                                                |
| xml_etree_parse      | 158 ms                                                                 | 155 ms: 1.02x faster                                                 |
| pickle               | 11.7 us                                                                | 11.5 us: 1.01x faster                                                |
| unpickle_pure_python | 228 us                                                                 | 226 us: 1.01x faster                                                 |
| xml_etree_process    | 58.9 ms                                                                | 58.4 ms: 1.01x faster                                                |
| json_dumps           | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                |
| pickle_dict          | 34.5 us                                                                | 35.1 us: 1.02x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.02x faster                                                         |

Benchmark hidden because not significant (3): xml_etree_generate, json_loads, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.2 ms                                                                | 10.1 ms: 1.01x faster                                                |
| python_startup_no_site | 8.81 ms                                                                | 8.77 ms: 1.01x faster                                                |
| Geometric mean         | (ref)                                                                  | 1.01x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 12.5 ms                                                                | 11.9 ms: 1.05x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20240130-linux-x86_64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| gc_traversal               | 4.31 ms                                                                | 3.59 ms: 1.20x faster                                                |
| nbody                      | 102 ms                                                                 | 88.2 ms: 1.16x faster                                                |
| scimark_sparse_mat_mult    | 5.54 ms                                                                | 4.81 ms: 1.15x faster                                                |
| spectral_norm              | 138 ms                                                                 | 126 ms: 1.09x faster                                                 |
| scimark_fft                | 381 ms                                                                 | 349 ms: 1.09x faster                                                 |
| crypto_pyaes               | 78.8 ms                                                                | 72.5 ms: 1.09x faster                                                |
| pyflate                    | 522 ms                                                                 | 484 ms: 1.08x faster                                                 |
| deltablue                  | 4.06 ms                                                                | 3.78 ms: 1.07x faster                                                |
| fannkuch                   | 443 ms                                                                 | 414 ms: 1.07x faster                                                 |
| float                      | 87.2 ms                                                                | 81.7 ms: 1.07x faster                                                |
| unpickle_list              | 5.29 us                                                                | 4.98 us: 1.06x faster                                                |
| unpickle                   | 16.3 us                                                                | 15.5 us: 1.05x faster                                                |
| comprehensions             | 19.6 us                                                                | 18.6 us: 1.05x faster                                                |
| mako                       | 12.5 ms                                                                | 11.9 ms: 1.05x faster                                                |
| chaos                      | 71.4 ms                                                                | 68.4 ms: 1.04x faster                                                |
| tomli_loads                | 2.21 sec                                                               | 2.14 sec: 1.03x faster                                               |
| scimark_monte_carlo        | 75.6 ms                                                                | 73.2 ms: 1.03x faster                                                |
| xml_etree_iterparse        | 109 ms                                                                 | 106 ms: 1.03x faster                                                 |
| hexiom                     | 8.04 ms                                                                | 7.81 ms: 1.03x faster                                                |
| pickle_list                | 5.13 us                                                                | 4.99 us: 1.03x faster                                                |
| create_gc_cycles           | 1.49 ms                                                                | 1.46 ms: 1.03x faster                                                |
| logging_silent             | 105 ns                                                                 | 102 ns: 1.03x faster                                                 |
| meteor_contest             | 112 ms                                                                 | 109 ms: 1.02x faster                                                 |
| nqueens                    | 88.9 ms                                                                | 87.0 ms: 1.02x faster                                                |
| regex_effbot               | 3.65 ms                                                                | 3.58 ms: 1.02x faster                                                |
| xml_etree_parse            | 158 ms                                                                 | 155 ms: 1.02x faster                                                 |
| scimark_lu                 | 115 ms                                                                 | 113 ms: 1.02x faster                                                 |
| regex_compile              | 142 ms                                                                 | 140 ms: 1.01x faster                                                 |
| async_tree_io              | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                               |
| pickle                     | 11.7 us                                                                | 11.5 us: 1.01x faster                                                |
| pprint_pformat             | 1.71 sec                                                               | 1.69 sec: 1.01x faster                                               |
| async_tree_memoization     | 572 ms                                                                 | 565 ms: 1.01x faster                                                 |
| deepcopy_reduce            | 3.13 us                                                                | 3.09 us: 1.01x faster                                                |
| async_tree_cpu_io_mixed    | 720 ms                                                                 | 711 ms: 1.01x faster                                                 |
| async_tree_none_tg         | 453 ms                                                                 | 448 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed_tg | 731 ms                                                                 | 723 ms: 1.01x faster                                                 |
| unpickle_pure_python       | 228 us                                                                 | 226 us: 1.01x faster                                                 |
| raytrace                   | 284 ms                                                                 | 281 ms: 1.01x faster                                                 |
| xml_etree_process          | 58.9 ms                                                                | 58.4 ms: 1.01x faster                                                |
| 2to3                       | 277 ms                                                                 | 275 ms: 1.01x faster                                                 |
| async_tree_io_tg           | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                               |
| coverage                   | 95.1 ms                                                                | 94.5 ms: 1.01x faster                                                |
| python_startup             | 10.2 ms                                                                | 10.1 ms: 1.01x faster                                                |
| python_startup_no_site     | 8.81 ms                                                                | 8.77 ms: 1.01x faster                                                |
| deepcopy                   | 351 us                                                                 | 349 us: 1.00x faster                                                 |
| sympy_integrate            | 21.0 ms                                                                | 21.0 ms: 1.00x faster                                                |
| pidigits                   | 188 ms                                                                 | 187 ms: 1.00x faster                                                 |
| asyncio_tcp_ssl            | 1.79 sec                                                               | 1.80 sec: 1.00x slower                                               |
| asyncio_tcp                | 490 ms                                                                 | 493 ms: 1.01x slower                                                 |
| richards_super             | 51.7 ms                                                                | 52.0 ms: 1.01x slower                                                |
| dulwich_log                | 68.0 ms                                                                | 68.4 ms: 1.01x slower                                                |
| regex_dna                  | 222 ms                                                                 | 224 ms: 1.01x slower                                                 |
| logging_simple             | 5.84 us                                                                | 5.88 us: 1.01x slower                                                |
| bench_thread_pool          | 834 us                                                                 | 840 us: 1.01x slower                                                 |
| sqlglot_transpile          | 1.61 ms                                                                | 1.62 ms: 1.01x slower                                                |
| generators                 | 29.5 ms                                                                | 29.7 ms: 1.01x slower                                                |
| json_dumps                 | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                |
| richards                   | 45.7 ms                                                                | 46.2 ms: 1.01x slower                                                |
| mdp                        | 2.74 sec                                                               | 2.77 sec: 1.01x slower                                               |
| sympy_expand               | 477 ms                                                                 | 483 ms: 1.01x slower                                                 |
| scimark_sor                | 131 ms                                                                 | 133 ms: 1.01x slower                                                 |
| pickle_dict                | 34.5 us                                                                | 35.1 us: 1.02x slower                                                |
| async_generators           | 458 ms                                                                 | 470 ms: 1.03x slower                                                 |
| typing_runtime_protocols   | 109 us                                                                 | 112 us: 1.03x slower                                                 |
| regex_v8                   | 24.8 ms                                                                | 25.6 ms: 1.03x slower                                                |
| pycparser                  | 1.18 sec                                                               | 1.22 sec: 1.03x slower                                               |
| unpack_sequence            | 41.2 ns                                                                | 47.2 ns: 1.14x slower                                                |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (26): async_tree_none, pprint_safe_repr, telco, xml_etree_generate, sympy_sum, chameleon, docutils, coroutines, asyncio_websockets, sympy_str, pathlib, bench_mp_pool, sqlglot_normalize, async_tree_memoization_tg, sqlglot_optimize, go, mypy2, sqlite_synth, tornado_http, json_loads, pickle_pure_python, logging_format, sqlglot_parse, dask, json, deepcopy_memo


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x