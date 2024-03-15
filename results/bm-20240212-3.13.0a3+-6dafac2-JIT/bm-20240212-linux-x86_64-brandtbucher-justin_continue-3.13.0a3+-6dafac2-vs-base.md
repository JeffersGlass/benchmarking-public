# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 276 ms                                                                 | 274 ms: 1.01x faster                                                    |
| chameleon      | 6.89 ms                                                                | 6.93 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_memoization_tg  | 594 ms                                                                 | 577 ms: 1.03x faster                                                    |
| async_tree_none_tg         | 457 ms                                                                 | 449 ms: 1.02x faster                                                    |
| async_tree_io              | 1.20 sec                                                               | 1.18 sec: 1.01x faster                                                  |
| async_tree_io_tg           | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                  |
| async_tree_memoization     | 572 ms                                                                 | 565 ms: 1.01x faster                                                    |
| async_tree_cpu_io_mixed_tg | 732 ms                                                                 | 723 ms: 1.01x faster                                                    |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 102 ms                                                                 | 93.6 ms: 1.09x faster                                                   |
| float          | 86.6 ms                                                                | 82.8 ms: 1.05x faster                                                   |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                    |
| Geometric mean | (ref)                                                                  | 1.05x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                                 | 137 ms: 1.03x faster                                                    |
| regex_v8       | 25.4 ms                                                                | 25.7 ms: 1.01x slower                                                   |
| regex_effbot   | 3.61 ms                                                                | 3.68 ms: 1.02x slower                                                   |
| regex_dna      | 219 ms                                                                 | 226 ms: 1.03x slower                                                    |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|---------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| tomli_loads         | 2.20 sec                                                               | 2.06 sec: 1.07x faster                                                  |
| pickle              | 11.6 us                                                                | 11.4 us: 1.02x faster                                                   |
| xml_etree_iterparse | 108 ms                                                                 | 106 ms: 1.01x faster                                                    |
| pickle_dict         | 33.3 us                                                                | 32.9 us: 1.01x faster                                                   |
| xml_etree_process   | 58.0 ms                                                                | 57.5 ms: 1.01x faster                                                   |
| xml_etree_generate  | 86.1 ms                                                                | 85.5 ms: 1.01x faster                                                   |
| pickle_list         | 4.91 us                                                                | 4.89 us: 1.01x faster                                                   |
| json_loads          | 27.5 us                                                                | 27.8 us: 1.01x slower                                                   |
| unpickle_list       | 4.85 us                                                                | 5.04 us: 1.04x slower                                                   |
| Geometric mean      | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (5): pickle_pure_python, json_dumps, xml_etree_parse, unpickle_pure_python, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 10.3 ms                                                                | 10.2 ms: 1.00x faster                                                   |
| python_startup_no_site | 8.87 ms                                                                | 8.88 ms: 1.00x slower                                                   |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 12.5 ms                                                                | 11.8 ms: 1.06x faster                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20240212-linux-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| unpack_sequence            | 48.3 ns                                                                | 39.0 ns: 1.24x faster                                                   |
| hexiom                     | 8.00 ms                                                                | 7.31 ms: 1.09x faster                                                   |
| nbody                      | 102 ms                                                                 | 93.6 ms: 1.09x faster                                                   |
| comprehensions             | 19.3 us                                                                | 17.8 us: 1.08x faster                                                   |
| pprint_pformat             | 1.64 sec                                                               | 1.53 sec: 1.08x faster                                                  |
| chaos                      | 70.5 ms                                                                | 65.5 ms: 1.08x faster                                                   |
| tomli_loads                | 2.20 sec                                                               | 2.06 sec: 1.07x faster                                                  |
| mako                       | 12.5 ms                                                                | 11.8 ms: 1.06x faster                                                   |
| pprint_safe_repr           | 788 ms                                                                 | 744 ms: 1.06x faster                                                    |
| nqueens                    | 90.3 ms                                                                | 86.0 ms: 1.05x faster                                                   |
| float                      | 86.6 ms                                                                | 82.8 ms: 1.05x faster                                                   |
| spectral_norm              | 136 ms                                                                 | 130 ms: 1.04x faster                                                    |
| scimark_fft                | 371 ms                                                                 | 357 ms: 1.04x faster                                                    |
| scimark_monte_carlo        | 74.0 ms                                                                | 71.2 ms: 1.04x faster                                                   |
| telco                      | 8.61 ms                                                                | 8.29 ms: 1.04x faster                                                   |
| meteor_contest             | 110 ms                                                                 | 106 ms: 1.04x faster                                                    |
| deepcopy_memo              | 38.4 us                                                                | 37.2 us: 1.03x faster                                                   |
| regex_compile              | 141 ms                                                                 | 137 ms: 1.03x faster                                                    |
| fannkuch                   | 422 ms                                                                 | 410 ms: 1.03x faster                                                    |
| async_tree_memoization_tg  | 594 ms                                                                 | 577 ms: 1.03x faster                                                    |
| typing_runtime_protocols   | 112 us                                                                 | 109 us: 1.03x faster                                                    |
| crypto_pyaes               | 78.0 ms                                                                | 75.8 ms: 1.03x faster                                                   |
| richards_super             | 51.9 ms                                                                | 50.5 ms: 1.03x faster                                                   |
| scimark_sparse_mat_mult    | 5.35 ms                                                                | 5.21 ms: 1.03x faster                                                   |
| pyflate                    | 496 ms                                                                 | 484 ms: 1.02x faster                                                    |
| json                       | 5.14 ms                                                                | 5.03 ms: 1.02x faster                                                   |
| raytrace                   | 280 ms                                                                 | 275 ms: 1.02x faster                                                    |
| deepcopy                   | 346 us                                                                 | 340 us: 1.02x faster                                                    |
| pickle                     | 11.6 us                                                                | 11.4 us: 1.02x faster                                                   |
| deltablue                  | 3.38 ms                                                                | 3.32 ms: 1.02x faster                                                   |
| async_tree_none_tg         | 457 ms                                                                 | 449 ms: 1.02x faster                                                    |
| logging_format             | 6.31 us                                                                | 6.20 us: 1.02x faster                                                   |
| deepcopy_reduce            | 3.08 us                                                                | 3.04 us: 1.01x faster                                                   |
| sympy_expand               | 480 ms                                                                 | 473 ms: 1.01x faster                                                    |
| xml_etree_iterparse        | 108 ms                                                                 | 106 ms: 1.01x faster                                                    |
| sqlglot_optimize           | 56.0 ms                                                                | 55.2 ms: 1.01x faster                                                   |
| async_tree_io              | 1.20 sec                                                               | 1.18 sec: 1.01x faster                                                  |
| richards                   | 45.9 ms                                                                | 45.3 ms: 1.01x faster                                                   |
| go                         | 147 ms                                                                 | 145 ms: 1.01x faster                                                    |
| sympy_sum                  | 160 ms                                                                 | 158 ms: 1.01x faster                                                    |
| async_tree_io_tg           | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                  |
| sqlglot_normalize          | 109 ms                                                                 | 108 ms: 1.01x faster                                                    |
| logging_simple             | 5.67 us                                                                | 5.61 us: 1.01x faster                                                   |
| dulwich_log                | 68.4 ms                                                                | 67.6 ms: 1.01x faster                                                   |
| async_tree_memoization     | 572 ms                                                                 | 565 ms: 1.01x faster                                                    |
| async_tree_cpu_io_mixed_tg | 732 ms                                                                 | 723 ms: 1.01x faster                                                    |
| sqlite_synth               | 2.81 us                                                                | 2.78 us: 1.01x faster                                                   |
| sympy_integrate            | 20.9 ms                                                                | 20.7 ms: 1.01x faster                                                   |
| sqlglot_parse              | 1.29 ms                                                                | 1.28 ms: 1.01x faster                                                   |
| pickle_dict                | 33.3 us                                                                | 32.9 us: 1.01x faster                                                   |
| xml_etree_process          | 58.0 ms                                                                | 57.5 ms: 1.01x faster                                                   |
| bench_thread_pool          | 843 us                                                                 | 836 us: 1.01x faster                                                    |
| xml_etree_generate         | 86.1 ms                                                                | 85.5 ms: 1.01x faster                                                   |
| sympy_str                  | 284 ms                                                                 | 282 ms: 1.01x faster                                                    |
| pickle_list                | 4.91 us                                                                | 4.89 us: 1.01x faster                                                   |
| 2to3                       | 276 ms                                                                 | 274 ms: 1.01x faster                                                    |
| generators                 | 29.2 ms                                                                | 29.1 ms: 1.00x faster                                                   |
| pidigits                   | 188 ms                                                                 | 187 ms: 1.00x faster                                                    |
| create_gc_cycles           | 1.50 ms                                                                | 1.49 ms: 1.00x faster                                                   |
| asyncio_tcp                | 494 ms                                                                 | 493 ms: 1.00x faster                                                    |
| asyncio_tcp_ssl            | 1.81 sec                                                               | 1.80 sec: 1.00x faster                                                  |
| python_startup             | 10.3 ms                                                                | 10.2 ms: 1.00x faster                                                   |
| python_startup_no_site     | 8.87 ms                                                                | 8.88 ms: 1.00x slower                                                   |
| async_generators           | 460 ms                                                                 | 462 ms: 1.01x slower                                                    |
| chameleon                  | 6.89 ms                                                                | 6.93 ms: 1.01x slower                                                   |
| regex_v8                   | 25.4 ms                                                                | 25.7 ms: 1.01x slower                                                   |
| json_loads                 | 27.5 us                                                                | 27.8 us: 1.01x slower                                                   |
| regex_effbot               | 3.61 ms                                                                | 3.68 ms: 1.02x slower                                                   |
| coverage                   | 96.5 ms                                                                | 98.9 ms: 1.02x slower                                                   |
| regex_dna                  | 219 ms                                                                 | 226 ms: 1.03x slower                                                    |
| unpickle_list              | 4.85 us                                                                | 5.04 us: 1.04x slower                                                   |
| scimark_sor                | 119 ms                                                                 | 124 ms: 1.04x slower                                                    |
| pycparser                  | 1.17 sec                                                               | 1.22 sec: 1.05x slower                                                  |
| Geometric mean             | (ref)                                                                  | 1.02x faster                                                            |

Benchmark hidden because not significant (20): async_tree_cpu_io_mixed, async_tree_none, tornado_http, pickle_pure_python, scimark_lu, sqlglot_transpile, json_dumps, dask, mypy2, mdp, gc_traversal, bench_mp_pool, asyncio_websockets, coroutines, docutils, logging_silent, pathlib, xml_etree_parse, unpickle_pure_python, unpickle


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x